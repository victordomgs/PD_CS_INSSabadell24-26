<h1 align="center">2.1. Organización de computadores
<div align="center">

</div>

## Introducción

Von Newman, el año 1945 plantea la **arquitectura básica de las computadoras digitales**. Estas máquinas, eran capaces de ejecutar una serie de instrucciones y ordenes elementales llamadas intrucciones máquina, que quedan almacenadas en lo que se conoce como memoria principal a la espera de ser leídas y ejecutadas por la Unidad Central de Procesamiento. La comunicación de estos dos elementos con el exterior se realiza a través de lo que se conoce como unidad de entrada y salida. 

## Contenido:

- [2.1.1. La unidad central de procesamiento y sus elementos](#211-la-unidad-central-de-procesamiento-y-sus-elementos)
- [2.1.2. Memoria principal](#212-memoria-principal)
- [2.1.3. Memoria caché](#213-memoria-caché)
- [2.1.4. Ciclo de instrucción de la CPU](#214-ciclo-de-instrucción-de-la-CPU) 
- [2.1.5. Memoria secundaria](#215-memoria-secundaria) 
- [2.1.6. Funciones de un sistema operativo](#216-funciones-de-un-sistema-operativo)
- [2.1.7. Programas de aplicación](#217-programas-de-aplicación)
- [2.1.8. Características comunes de las aplicaciones](#218-características-comunes-de-las-aplicaciones)
- [2.1.9. Bit, byte, binario, decimal y hexadecimal](#219-bit-byte-binario-decimal-y-hexadecimal)
- [2.1.10. Representación de datos](#2110-representación-de-datos)
- [2.1.11. Operadores lógicos](#2111-operadores-lógicos)
- [2.1.12. Tablas de la verdad](#2112-tablas-de-la-verdad)
- [2.1.13. Diagrama lógico y diagrama de Venn](#2113-diagrama-lógico-y-diagrama-de-Venn)

## 2.1.1. La unidad central de procesamiento y sus elementos

### Unidad aritmética lógica

La **Unidad Aritmética Lógica (UAL)** es la parte del procesador encargada de ejecutar las operaciones matemáticas y lógicas necesarias para el procesamiento de datos. Esta unidad actua en conjunto con la Unidad de Control (UC), que le indica que operaciones tiene que realizar y sobre que operandos. 

Las operaciones básicas que puede ejecutar la UAL son: 
- **Operaciones aritméticas:** suma, resta, multiplicación y división.
- **Operaciones lógicas:** AND, OR, XOR y NOT.
- **Operaciones de desplazamiento:** ya sean operaciones lógicas o aritméticas.
- **Operaciones de comparación:** para determinar relaciones entre nombres. 

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.1-Arquitectura-de-computadores/images/Esquema%20de%20ALU.png" alt="Esquema de la ALU" width="670" height="auto"/>
    <p><em>Figura 1: Esquema de la ALU. Fuente: Abacus</em></p>
  </div>

  A continuación, se explican las partes fundamentales de la ALU:

  - **Circuito combinacional:** se encarga de realizar las operaciones con los datos procedentes de los registros de entrada: REN1 y REN2. Las entradas de ordenes que aparecen a la derecha sirven para indicar el tipo de operación necesaria.
  - **Registro de entrada:** se encarga de almacenar los datos y operandos de entrada encargados de realizar la instrucción. También se utilizan para almacenar resultados intermedios o finales de las operaciones.
  - **Registro acumulador:** en este registro se almacenan los resultados de las operaciones realizadas en el circuito combinacional. Y además, esta conectado con el registro de entrada REN2 para poder realizar operaciones concatenadas si es necesario.
  - **Registro de estado:** segun el valor marcado en este registro el procesador ejecutara la operación que más convenga. En realidad, cada uno de los biestables que componen este registro informarán del último valor escrito en el acumulador. Los valores más típicos son los siguientes:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.1-Arquitectura-de-computadores/images/Registro%20de%20estado.png" alt="Registro de estado" width="670" height="auto"/>
    <p><em>Figura 2: Registro de estado. Fuente: Abacus</em></p>
  </div>

  - NU: No utilizado.
  - Z: Indica cuando el resultado es 0. Devuelve 1 cuando este es 0.
  - N: Devuelve 1 cuando el resultado es negativo.
  - C: Biestable indicador de accarreo.
  - O: Biestable indicador de desbordamiento.
  - P: Biestable indicador de paridad.
  - CP: Biestable de acarreo parcial.

### Unidad de Control

La **Unidad de Control (UC)** se encarga de la interpretación y ejecución de las instrucciones recibidas desde la memoria principal, así como del control de todos los componentes del sistema. Su función principal es dirigir el funcionamiento de todos los componentes del procesador y coordinar el movimiento de datos entre los diferentes elementos de la CPU y la memoria.

Las funciones esenciales de a UC son: 

- **Contro del flujo de ejecución:** interpreta las instrucciones y las ejecuta en el orden correcto.
- **Generación de señal de control:** envia señales para activar o desactivar los diferentes componentes de la UAL.
- **Gestión de buses de datos y de buses de direcciones:** determina que datos se leen o escriben y hacia donde se deben enviar.
- **Sincronización con el reloj del sistema:** controla el tiempo de ejecución de las instrucciones para mantener el ritmo de trabajo del procesador.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.1-Arquitectura-de-computadores/images/Esquema%20de%20la%20UC.png" alt="Esquema de la UC" width="670" height="auto"/>
    <p><em>Figura 3: Esquema de la UC. Fuente: Abacus</em></p>
  </div>

  A continuación, se explican las partes fundamentales de la UC:

  - **Registro de instrucción:** este registro almacena la instrucción que se está ejecutando en este momento, procedente de la memoria principal. Este registro se divide en tres campos:
    - *CO (código de operación):* se encarga de indicar la operación a realizar (suma, resta, multiplicación, etc).
    - *MD (modo de direccionamiento):* se encarga de indicar el modo de acceder a la memoria para buscar el dato o la dirección para ejecutar determinadas instrucciones.
    - *CDE (campo de dirección efectivo):* contiene a información necesaria para que se pueda acceder al dato.
  - **Registro contador de programa (CP):** este registro contiene la dirección de la siguiente instrucción a ejecutar. Al finalizar una instrucción el CP deberá incrementar su valor en uno, con tal de así ejecutar la siguiente instrucción que marque el reloj.
  - **Registro de direcciones de memoria (RDM):** en él se almacenan las direcciones de memoria en las cuales se van a leer o escribir datos.
  - **Registro de datos de memoria (RIM):** almacena temporalmente los datos que se intercambian con la memoria en las operaciones de lectura y escritura.
  - **Decodificador:** es el circuito computacional que toma como entrada los campos CO + MD del registro de instrucciones y activa un conjunto de salidas conectadas directamente como entradas al controlador. Simplifica el trabajo de esté, ya que cada salida del decodificador estará asociada directamente con una instrucción y un modo de direccionamiento determinados, mientras que a su entrada esa misma información está codificada para ahorrar bits de memoria.
  - **Controlador:** este es el verdadero núcleo o cerebro de operaciones del ordenador. Se puede definir como un circuito secuencial, cuyas entradas corresponden a los códigos de operación del repertorio de instrucciones, los modos de direccionamiento de la instrucción a ejecutar y el estado de la máquina, representado por los registros indicadores (flags), y que porpocionan como salida las microórdenes que gobiernan el funcionamiento del ordenador, estas microórdenes son as que activarán las ordenes de lectura o escritura de os registros, las operaciones a realizar en la ALU, la memoria, etc.
    - *Salidas del codificador:* le indican el tipo de instrucción y modo de direccionamiento asociados.
    - *Reloj del sistema:* el controlador debe tener información acerca de los pulsos del reloj para así poder controlar las ordenes.
    - *Registro de estado:* conoce en todo momento el estado de este registro para así poder gobernar adecuadamente las instrucciones de salto. 

El proceso que sigue a la Unidad de Control para ejecutar una instrucción se puede dividir en dos fases principales: 

#### Fase de búsqueda (fetch)

- La UC envía una orden para leer la siguiente instrucción desde la memória central.
- La dirección de esta instrucción esta almacenada en el contrador del programa (CP).
- La instrucción se carga en el registro de instrucciones (RI) y el CP se incrementa para apuntar a la siguiente instrucción.

#### Fase de ejecución (execute)

- La UC interpreta la instrucción cargada en el RI mediante el decodificador.
- Genera las microordenes necesarias para activar la UAL, los registros y los buses según sea necesario.
- Si la operación requiere datos de la memória, las carga al RIM antes de ser procesadas.
- Una vez ejecutada la instrucción, la UC pasa a la siguiente instrucción.

## 2.1.2. Memoria principal

La memoria de un sistema informático se define como el medio físico capaz de almacenar la información de forma temporal o permanente. Esta información puede ser leída o escrita segun las características de cada tipo de memoria. 

### Características principales
Las características principales de la memoria estan determinadas por los siguientes factores: 

#### Duración de la información

- **Memorias volátiles:** la información se mantiene solo mientras hay subministramiento eléctrico (por ejemplo, la RAM).
- **Memorias no volátiles:** la información persiste después de apagar el equipo (por ejemplo, la ROM o las memorias flash).
- **Memorias permanentes:** no pueden ser modificadas una vez grabadas (por ejemplo, algunas ROM de fábrica).
- **Memorias con refresco:** necesitan una operación periódica para evitar la pérdida de datos (por ejemplo, DRAM).

#### Capacidad de almacenamiento

Determinada por el número de posiciones de almacenamiento y la canditat de bits por posición. 

Expresada en bytes (B), kilbytes (KB), megabytes (MB), gigabytes (GB), etc. 

| Amplada       | Nom              |
|---------------|------------------|
| 1 bit         | (b)              |
| 4 bits        | nibble           |
| 8 bits        | byte (B)         |
| 16 bits       | palabra          |
| 32 bits       | doble palabra    |

| Unitat | Equivalència                         |
|--------|--------------------------------------|
| 1K     | Kilo = 2¹⁰ = 1024                    |
| 1M     | Mega = 2²⁰ = 1024 K                  |
| 1G     | Giga = 2³⁰ = 1024 M                  |
| 1T     | Tera = 2⁴⁰ = 1024 G                  |
| 1P     | Peta = 2⁵⁰ = 1024 T                  |

#### Velocidad

- **Tiempo de acceso (TA)**: Tiempo necesario para leer o escribir un dato en una posición determinada.
- **Tiempo de ciclo (TC)**: Tiempo mínimo entre dos operaciones sucesivas sobre la memoria.
- **Frecuencia de acceso (FA)**: Número de lecturas/escrituras que se pueden realizar por unidad de tiempo.

#### Unidad de transferencia

- **Acceso por palabra**: Se transfiere una única palabra de memoria por operación.
- **Acceso por bloque**: Se transfiere un conjunto de palabras de memoria.

#### Modo de acceso

- **Acceso aleatorio**: Se puede acceder directamente a cualquier posición de memoria (por ejemplo, la RAM).
- **Acceso secuencial**: Es necesario recorrer la memoria en orden hasta llegar a la posición deseada (por ejemplo, cintas magnéticas).

### Memoria RAM
La **RAM** es un área de almacenamiento de propósito general, lo que significa que los datos almacenados pueden sobrescribirse. Esto permite que los datos e instrucciones se carguen para su ejecución y uso siempre que sea necesario. Sin embargo, la RAM es volátil, lo que significa que cuando se pierde la energía, el contenido de su memoria se borra (por ejemplo, si un documento no guardado con cambios está abierto cuando se corta la energía, todos los cambios que se habían hecho se perderán).

### Memoria ROM
La **ROM** se utiliza para almacenar instrucciones y datos que no pueden sobrescribirse. Esto significa que las instrucciones que están integradas en la ROM no pueden modificarse, incluso si se pierde la energía, y por lo tanto se considera memoria no volátil. La ROM se utiliza para almacenar programas e instrucciones que no necesitan actualizarse ni cambiarse (por ejemplo, las instrucciones de inicio del sistema operativo).

## 2.1.3. Memoria caché

Existen dos tipos de memoria RAM:

- Dynamic RAM (DRAM)
- Static RAM (SRAM)

La **SRAM** es más rápida pero más cara que la **DRAM**, y por lo tanto se prefiere la DRAM como memoria RAM principal de un sistema informático. Sin embargo, una pequeña cantidad de SRAM se coloca entre la RAM principal y el procesador, y se denomina **caché** (Figura 4). Así, la caché es una RAM más pequeña y más rápida (SRAM) que almacena temporalmente instrucciones y datos, de modo que el procesador no necesita acceder a la memoria principal más lenta (DRAM).

La **caché** guarda la información de la RAM que se utiliza con mayor frecuencia y que se accede más habitualmente. El sistema informático funcionará más rápido, ya que se accederá con menor frecuencia a la memoria principal, que es más lenta. Cuando el procesador necesita leer de la memoria principal, primero verifica si existe una copia de los datos en la caché. Si es así, el procesador lee desde la caché en lugar de hacerlo desde la memoria principal. Esta acción acelera el proceso. Si los datos que se van a leer no existen en la caché, los datos se copian primero a la caché y luego se utilizan. Cuando el procesador necesita escribir en la memoria principal, lo hace a través de la memoria caché.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%201.%20Organizaci%C3%B3n%20de%20computadores.png" alt="Memoria Cache" width="670" height="auto"/>
    <p><em>Figura 4: Memoria Cache. Fuente: Kostas Dimitriou, Markos Hatzitaskos</em></p>
  </div>

## 2.1.4. Ciclo de instrucción de la CPU

Los programas informáticos se almacenan en la memoria primaria como una serie de instrucciones en código máquina. Estas instrucciones, así como cualquier otro dato necesario, deben trasladarse desde la memoria primaria hasta la CPU para que el programa pueda funcionar. Para que esto ocurra, se siguen pasos específicos. Las siguientes funciones son realizadas por la CPU para ejecutar un programa informático:

### 1. Captar la instrucción desde la memoria primaria hacia la unidad de control
La CPU es responsable de saber qué instrucción debe tomar de la memoria primaria para poder operar correctamente. Para ello, envía la dirección apropiada a través del bus de direcciones hacia la memoria primaria. La instrucción que se encuentra en la dirección específica se copia entonces en el bus de datos y se envía a la unidad de control (CU).

### 2. Decodificar la instrucción en la unidad de control
La instrucción recibida por la CU se decodifica a continuación. La decodificación de la instrucción permite a la CPU conocer cualquier dato adicional que sea necesario para la ejecución de la instrucción. Si se necesitan datos adicionales de la memoria primaria para que la instrucción pueda ejecutarse, estos se cargan en este momento. Las direcciones de esos datos se colocan en el bus de direcciones y los datos de esas direcciones son recibidos por la CPU a través del bus de datos.

### 3. Ejecutar la instrucción
La CPU ejecuta la instrucción utilizando los datos necesarios que han sido cargados y calcula un resultado. Dependiendo del resultado, pueden necesitarse datos adicionales. Estos datos se obtienen de la memoria primaria para realizar cálculos adicionales. Como antes, las direcciones de esos datos se colocan en el bus de direcciones y los datos de esas direcciones son recibidos por la CPU a través del bus de datos.

### 4. Almacenar el resultado de la ejecución y comprobar la siguiente instrucción
Después de ejecutar la instrucción y calcular el resultado, la CPU almacena dicho resultado en la memoria primaria. Para hacerlo, especifica la dirección en la que residirá el resultado dentro de la memoria primaria, utilizando el bus de direcciones, y envía los datos a través del bus de datos. La CPU comprueba entonces la siguiente instrucción y repite los pasos descritos anteriormente: captar, decodificar, ejecutar y finalmente almacenar el resultado.

## 2.1.5. Memoria secundaria

La memoria secundaria, también conocida como almacenamiento masivo, cumple una función vital en los sistemas informáticos: el almacenamiento permanente de datos. A diferencia de la memoria principal (RAM), los datos no se pierden cuando el sistema se apaga. Esta memoria es más lenta, pero ofrece una gran capacidad de almacenamiento a un coste relativamente bajo.

### Características principales

- **Capacidad**: Las memorias secundarias pueden alcanzar capacidades de varios terabytes (TB), lo que las hace adecuadas para almacenar grandes volúmenes de datos como bases de datos, vídeos, copias de seguridad, etc.
- **Persistencia**: Una de sus principales ventajas es la retención de datos sin necesidad de energía eléctrica. Esto es fundamental para la integridad y conservación de la información.
- **Velocidad**: Aunque son más lentas que la memoria RAM, las tecnologías actuales como las SSD han reducido esta brecha significativamente.
- **Costo**: Su precio por gigabyte es considerablemente más bajo que el de la memoria principal, lo que las hace idóneas para almacenamiento a largo plazo.

### Tipos de memoria secundaria

- **Discos duros (HDD)**: Utilizan platos magnéticos giratorios y cabezales de lectura/escritura. Son ideales para almacenamiento masivo a bajo costo. Sin embargo, presentan mayor latencia debido a las partes mecánicas.
- **Unidades de estado sólido (SSD)**: Basadas en memoria flash, ofrecen velocidades de lectura y escritura muy superiores a los HDD. No tienen partes móviles, lo que reduce su desgaste y mejora su resistencia a impactos.
- **Memorias USB (pendrives)**: Utilizadas habitualmente para transferencias rápidas de datos entre dispositivos. Aunque su velocidad puede ser limitada, destacan por su portabilidad y facilidad de uso.
- **Tarjetas de memoria**: Comunes en cámaras digitales, teléfonos y dispositivos portátiles. Utilizan también tecnología flash y presentan diversas capacidades y velocidades.
- **Cintas magnéticas**: Aunque han caído en desuso en el ámbito doméstico, siguen siendo una solución viable para almacenamiento masivo a largo plazo en entornos empresariales, especialmente para copias de seguridad.

### Importancia en los sistemas informáticos

La memoria secundaria es esencial en múltiples aspectos del funcionamiento de un sistema informático:

- Almacena el sistema operativo, que se carga en la memoria principal al arrancar.
- Guarda las aplicaciones y los archivos del usuario.
- Permite realizar copias de seguridad para evitar la pérdida de información crítica.
- Facilita la gestión de grandes volúmenes de datos de forma estructurada (por ejemplo, en servidores y bases de datos).

### Evolución tecnológica

La evolución de la memoria secundaria ha sido constante, con mejoras notables en capacidad, velocidad y fiabilidad:

- De los antiguos disquetes a los actuales discos duros y SSD.
- Disminución del tamaño físico con aumento de capacidad (por ejemplo, microSD de 1 TB).
- Avances como NVMe y PCIe han incrementado significativamente la velocidad de acceso en los SSD modernos.
- Aparición del almacenamiento en la nube como forma de memoria secundaria accesible remotamente.

### Comparación entre tipos de almacenamiento

| Tipo             | Capacidad típica | Velocidad      | Precio por GB | Durabilidad | Portabilidad |
|------------------|------------------|----------------|---------------|-------------|--------------|
| HDD              | 500 GB – 16 TB   | Media          | Bajo          | Moderada    | Baja         |
| SSD (SATA/NVMe)  | 120 GB – 8 TB    | Alta           | Medio         | Alta        | Media        |
| USB              | 8 GB – 2 TB      | Variable       | Medio         | Alta        | Alta         |
| Tarjeta de memoria | 4 GB – 1 TB     | Variable       | Medio         | Alta        | Alta         |
| Cinta magnética  | Hasta 30 TB      | Muy baja       | Muy bajo      | Alta        | Baja         |

Cada tipo de memoria secundaria tiene su contexto de uso ideal, por lo que es habitual encontrar varios tipos coexistiendo en un mismo entorno informático.

A continuación, se muestra un diagrama con las jerarquias de memoria: 

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.2-Memoria-secundaria/images/jerarquiamemoria.png" alt="Jerarquía de memoria" width="750" height="auto"/>
    <p><em>Figura 5: Jerarquía de memoria. Fuente: Abacus</em></p>
  </div>
