<img width="678" height="715" alt="image" src="https://github.com/user-attachments/assets/bc6cae2d-a1ae-4214-b146-5322904ec911" /><h1 align="center">2.1. Organización de computadores
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
- [2.1.6. El sistema operativo](#216-el-sistema-operativo)
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

## 2.1.6. El sistema operativo

El **sistema operativo** es un tipo de software base que permite la interacción entre el usuario y las aplicaciones con el hardware del sistema informático. Es el software más importante de un sistema informático, ya que además de permitir la comunicación entre el usuario y el hardware, gestiona todos los recursos del sistema, como los procesos, archivos y directorios.

El **sistema operativo** es el software más importante de un sistema informático. Este software ofrece al usuario la posibilidad de interactuar con el sistema informático de forma sencilla, permitiéndole gestionar la información y los recursos disponibles.

Podemos definir los sistemas operativos atendiendo a sus dos funciones básicas:

1. Proporcionar a los usuarios y aplicaciones una **interfaz de acceso** a los recursos de hardware.
2. Gestionar dichos **recursos**.

El sistema operativo **administra todos los recursos del hardware**, proporciona la base para la ejecución del software de aplicación y actúa como **interfaz entre el equipo y los usuarios**.

La interfaz de acceso a los recursos de hardware que proporciona el sistema operativo permite tanto a usuarios como a aplicaciones acceder al hardware del sistema informático.
La interfaz más conocida es la **interfaz gráfica de usuario**, que permite al usuario convencional interactuar con el sistema de forma amigable y representa la imagen visual del sistema operativo que utilizamos.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.3-Sistemas-operativos-y-sistemas-de-aplicacion/images/interfaz-de-Windows.jpg" alt="Superordenador MareNostrum" width="550" height="auto"/>
    <p><em>Figura 6: Interfaz gráfica de un sistema Windows. Fuente: NetView</em></p>
  </div>
  
En cuanto a la gestión de recursos del hardware —entendiendo "recurso" como cualquier componente físico del sistema informático—, el sistema operativo se encarga de **planificar los accesos a dichos componentes** y de **almacenar la información** en ellos.

### Elementos y estructura del sistema operativo

Un sistema operativo está formado por varios elementos que, unidos entre sí, dan forma a la estructura básica del sistema informático. Los principales elementos que lo componen son los siguientes:

- **Procesos**: Un proceso es, esencialmente, un programa en ejecución. Por ejemplo, cuando un usuario ejecuta la calculadora de Windows, el programa se carga en memoria y se convierte en un proceso. Cada proceso mantiene una lista de ubicaciones en memoria donde se almacena, conocida como su **espacio de direcciones de memoria**.
- **Espacio de direcciones**: La memoria principal de un sistema informático es limitada. Solo los programas y datos almacenados en ella pueden estar en ejecución. El sistema operativo gestiona esta memoria y asigna a cada programa un conjunto de ubicaciones o espacio de direcciones que define cuánta memoria puede usar.
- **Sistema de archivos**: Es una parte clave de cualquier sistema informático. Permite al sistema leer, crear, escribir y eliminar archivos. El sistema operativo organiza esta información en estructuras de **directorios**, normalmente en forma de árbol, para agrupar los archivos.
- **Sistema de entrada/salida**: Los sistemas informáticos tienen dispositivos físicos para recibir información (entrada) y mostrarla (salida). El sistema operativo gestiona esta entrada/salida mediante un sistema compuesto por una parte común para todos los dispositivos y una parte específica para cada uno, conocida como controlador.
- **Sistema de protección**: Es fundamental garantizar que la información esté correctamente protegida y que solo los procesos autorizados puedan acceder a ella. La administración segura de los datos es responsabilidad del sistema operativo.
- **Intérprete de órdenes (Shell) e interfaz gráfica de usuario (GUI)**: El intérprete de órdenes es la interfaz principal entre el usuario y el sistema operativo, permitiendo dar instrucciones en modo texto. En los sistemas modernos se utiliza una **interfaz gráfica de usuario (GUI)**, que es un programa ejecutado sobre el sistema operativo que permite al usuario interactuar con él de forma más sencilla y visual.

### Clasificación de los sistemas operativos

Los sistemas operativos han experimentado un gran crecimiento desde la década de 1950 hasta la actualidad. Durante este tiempo se ha desarrollado una gran variedad de sistemas, cada uno con sus propias características y técnicas clave para mejorar su rendimiento.

Debido a esta variedad, los sistemas operativos pueden clasificarse según distintos criterios. Uno de los criterios más habituales es el número de **usuarios simultáneos**, lo que nos permite distinguir entre:

- **Monousuario**: Este tipo de sistema solo puede atender a un único usuario a la vez. Todos los recursos están disponibles para ese usuario y no pueden ser utilizados por nadie más hasta que finalice la sesión.
Ejemplos: MS-DOS (Microsoft), OS/2 (IBM), Windows 9x (Microsoft).
- **Multiusuario**: Este tipo de sistema permite que varios usuarios utilicen los recursos del sistema **simultáneamente**. Cada usuario puede tener su propia configuración personalizada.
Ejemplos: UNIX y sus variantes, macOS (Apple Inc.), Windows 10 (Microsoft).

### Funciones del sistema operativo

El **sistema operativo** se encarga de **gestionar los recursos del equipo** para optimizar su funcionamiento y permitir la ejecución de otras aplicaciones. Esta gestión se puede dividir en los siguientes bloques:

- **Ayuda al usuario**: El sistema operativo facilita el uso del sistema informático proporcionando un entorno de fácil utilización, lo que mejora la productividad y simplifica la comunicación con el hardware.
- **Gestión de procesos**: Permite que los programas se ejecuten e interactúen con el hardware. Se encarga de controlar el estado de los procesos y planificar el uso del procesador para obtener el máximo rendimiento.
- **Gestión de dispositivos de entrada/salida**: El sistema operativo debe ser capaz de enviar y recibir órdenes desde y hacia los dispositivos periféricos.
- **Gestión del sistema de archivos**: Permite la realización de operaciones como la creación, eliminación o modificación de archivos y directorios, entre otras.
- **Gestión de la memoria**: Administra la memoria del sistema asignándola a los distintos programas que se están ejecutando para optimizar su uso.
- **Protección del sistema**: Debe garantizar la seguridad de la información de los usuarios y prevenir accesos no autorizados, ya sean intencionados o accidentales.
- **Monitorización interna**: Supervisa todas las operaciones realizadas en el sistema para detectar posibles errores en dispositivos, memoria, ejecución de programas o el sistema de archivos. Ante cualquier error, debe notificar al usuario y continuar funcionando.

En resumen, se pueden distinguir tres funciones básicas de los sistemas operativos:

1. **Ayudar al usuario**.
2. **Monitorizar y proteger el sistema**.
3. **Gestionar los recursos** del sistema informático.

Los **recursos** de un sistema informático incluyen los componentes físicos como el procesador, la memoria y los dispositivos de entrada/salida. El sistema operativo los asigna a los distintos programas que los solicitan, incluso cuando lo hacen de forma simultánea.

Además, los sistemas operativos disponen de **mecanismos de control de recursos** para resolver conflictos y administrar la carga de trabajo, adaptándose así a las necesidades del usuario.

#### Gestión de archivos

Dentro de un sistema informático, la información se almacena en los **dispositivos de almacenamiento** en bloques, de forma que los procesos que ejecuta el sistema pueden realizar dos operaciones principales: **leer el bloque** o **escribir en él**.

Esta información, habitualmente, se **estructura lógicamente** mediante archivos y directorios. Los **archivos y directorios** son una **abstracción** que permite a los procesos y a los usuarios trabajar con los datos contenidos en los bloques de una forma mucho más sencilla.

Un **archivo** es un conjunto lógico de datos con los que trabajan los procesos. Los archivos pueden **crearse, leerse, eliminarse, reubicarse, comprimirse, ejecutarse, etc**. Existen diferentes tipos de archivos, según el contenido que almacenen, desde **archivos de programas** hasta **archivos de datos comunes**.

El sistema también permite **proteger los archivos** mediante una serie de **permisos** que determinan qué operaciones pueden realizarse sobre ellos.

Cada sistema operativo utiliza su **propio sistema de archivos**, el cual permite organizar la información de forma lógica, facilitando una gestión más **rápida y sencilla**.

El sistema de archivos determina **cómo se almacena la información** en un dispositivo de almacenamiento y **qué operaciones pueden realizarse** con ella.

Para gestionar adecuadamente el sistema de archivos, el sistema operativo debe llevar a cabo las siguientes funciones:

- Gestión de **directorios, archivos y rutas de acceso**.
- Gestión de las **operaciones y permisos** sobre archivos y directorios.
- Gestión de **accesos simultáneos** a un mismo archivo o directorio.
- Gestión del **espacio de almacenamiento**.
- Gestión de **errores** y mantenimiento de la **consistencia** del sistema de archivos.

#### Gestión de la memoria

Uno de los componentes más importantes de un equipo informático es la **memoria**. Esta debería ser rápida, tener gran capacidad de almacenamiento y ser económica. Sin embargo, actualmente ninguna tecnología cumple con las tres características al mismo tiempo. Por ello, se ha adoptado un **sistema jerárquico de memoria por capas**.

Para que un proceso pueda ejecutarse, debe estar **almacenado en la memoria principal**. Los programas y datos no necesarios inmediatamente se guardan en **memoria secundaria** hasta que se requieran.

##### Funciones de gestión de memoria del sistema operativo:

- **Asignación de memoria** para la ejecución de procesos y aplicaciones. La memoria puede ser contigua o no.
- **Liberación de memoria** una vez ya no se necesita, dejándola disponible para otros procesos.
- **Gestión de programas simultáneos en memoria**: controla cuántos programas están cargados al mismo tiempo.
- **Gestión entre memoria principal y secundaria**: permite la ejecución de programas que no caben completamente en memoria, dividiéndolos entre RAM y almacenamiento secundario.

#### Gestión de procesos

Uno de los elementos principales de los sistemas operativos son los **procesos**, y una de las tareas fundamentales del sistema operativo es **gestionar esos procesos** y su acceso al procesador.

La principal diferencia entre un **programa** y un **proceso** es que el programa es un conjunto de instrucciones, mientras que un proceso es ese conjunto de instrucciones en **ejecución**.
Un proceso no está formado solo por el código ejecutable, sino también por otra información necesaria para su ejecución, como los valores de los registros del procesador, los datos de entrada, etc.

Un **proceso** es una **secuencia de acciones derivadas de la ejecución de instrucciones**. Un proceso puede requerir ejecutar uno o varios programas, y un mismo programa puede formar parte de distintos procesos.

Cuando se inicia el sistema operativo, este pone en marcha sus **procesos principales**, encargados de crear el resto de procesos del sistema, llamados **procesos hijos**. La estructura de los procesos en un sistema operativo es **jerárquica**, en forma de árbol: todos los procesos (excepto los iniciales) tienen un **proceso padre**, y pueden tener uno o más **procesos hijos**.

##### Información que el sistema operativo mantiene sobre cada proceso:

- **Identificador del proceso (PID)**: número entero único para identificar cada proceso.
- **Estado del proceso**: refleja en qué fase del ciclo de vida se encuentra.
- **Uso de recursos**: incluye datos como tiempo de ejecución, prioridad, quántum, etc., útil para planificar qué proceso se ejecutará a continuación.
- **Contexto del proceso**: guarda el estado del procesador, información de memoria y peticiones de entrada/salida.

Esta información se guarda en una estructura llamada **Bloque de Control del Proceso (PCB, Process Control Block)**.

##### Estados del proceso

Los procesos pueden encontrarse en distintos **estados** durante su ciclo de vida. Aunque el modelo más simple contempla solo dos (en ejecución o finalizado), los sistemas operativos modernos suelen utilizar un modelo de **cinco estados**:

1. **Nuevo**: el proceso ha sido creado pero aún no está preparado para ejecutarse. Solo puede encontrarse una vez en este estado.
2. **Preparado**: el proceso está listo para ejecutarse. Puede llegar aquí desde el estado Nuevo, o tras regresar desde Bloqueado o Ejecución.
3. **Ejecución**: el procesador está ejecutando el proceso. Si el tiempo asignado finaliza sin haber completado su ejecución, vuelve al estado Preparado.
4. **Bloqueado**: el proceso espera un evento (como una entrada/salida), por lo que deja de ejecutarse temporalmente.
5. **Finalizado**: el proceso ha terminado su ejecución y se liberan los recursos que estaba utilizando.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.3-Sistemas-operativos-y-sistemas-de-aplicacion/images/transici%C3%B3n_estados.png" alt="Transición de estados" width="550" height="auto"/>
    <p><em>Figura 7: Transición de estados. Fuente: IOC</em></p>
  </div>

#### Gestión de entrada/salida

Una de las funciones del sistema operativo es **gestionar la comunicación con los dispositivos de entrada/salida** de forma **paralela a la CPU**, con el fin de mejorar el rendimiento del equipo.

En un sistema informático, un **dispositivo de entrada/salida** puede ser:

- Un **dispositivo de almacenamiento secundario**, como un disco duro.
- Un **dispositivo de comunicación**, como una tarjeta de red.
- Un **dispositivo clásico**, como el teclado, el ratón o el monitor.

Aunque estos dispositivos son muy diversos, todos comparten algunas **características comunes**:

- **Unidad de transferencia**: algunos dispositivos transfieren datos en unidades pequeñas como caracteres (ej. teclado o ratón), mientras que otros lo hacen por **bloques** (ej. discos duros).
- **Velocidad**: varía mucho entre dispositivos. Por ejemplo, los dispositivos de comunicación pueden transferir datos constantemente, mientras que el teclado o el ratón lo hacen en momentos concretos y en pequeñas cantidades.
- **Comunicación con la CPU**: cada dispositivo utiliza un **protocolo distinto** para comunicarse con la CPU, lo cual depende del tipo de dispositivo y del **bus de comunicación** (las conexiones físicas entre los dispositivos y la CPU).

##### Controlador de dispositivo

Un **controlador de dispositivo** es un **programa** que permite al sistema operativo comunicarse con un determinado dispositivo de entrada/salida.

Gracias a los controladores:

El sistema operativo **no necesita conocer el funcionamiento específico** de cada dispositivo.
Solo debe comunicarse con el **controlador correspondiente**, que actúa como intermediario.
Estos controladores suelen tener una **interfaz estandarizada**, lo que facilita su gestión por parte del sistema operativo.

La **comunicación con los controladores** suele ser responsabilidad del **núcleo (kernel)** del sistema operativo.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.3-Sistemas-operativos-y-sistemas-de-aplicacion/images/conexi%C3%B3nes.png" alt="Conexión del dispositivo E/S" width="550" height="auto"/>
    <p><em>Figura 8: Conexión del dispositivo E/S. Fuente: IOC</em></p>
  </div>

## 2.1.7. Programas de aplicación

Un sistema informático tiene la capacidad de ejecutar al menos una aplicación de software, que ha sido instalada por el fabricante para completar algunas tareas predefinidas. Por ejemplo, una cámara digital es por sí sola un sistema informático. Consta tanto de componentes de hardware como de software y sigue el modelo de entrada, proceso, salida y almacenamiento descrito en el ejemplo de la sección 2.1.1. Los componentes de software de la cámara digital están preinstalados en el momento de su fabricación y completan tareas predefinidas (por ejemplo, cuando se presiona el botón del obturador, se ejecuta el software responsable de capturar la imagen en formato digital y almacenarla en memoria después de procesarla). Estos componentes de software de la cámara digital solo pueden modificarse recibiendo versiones actualizadas del fabricante.

Sin embargo, los sistemas informáticos incluyen dispositivos como ordenadores de sobremesa y portátiles, tabletas, teléfonos inteligentes, etc. Estos permiten al usuario instalar una gran cantidad de aplicaciones de software en ellos. Esto posibilita el uso de una variedad de aplicaciones en lugar de limitarse a completar una única tarea predefinida. Las principales aplicaciones de software que pueden instalarse en dichos sistemas informáticos incluyen:

- Procesadores de texto
- Hojas de cálculo
- Sistemas de gestión de bases de datos
- Navegadores web
- Correo electrónico
- Diseño asistido por computadora (CAD)
- Software de procesamiento gráfico

## 2.1.8. Características comunes de las aplicaciones

Las aplicaciones de software instaladas en los sistemas informáticos suelen incluir una **interfaz gráfica de usuario (GUI)** para permitir que el usuario interactúe con ellas de varias formas, en lugar de solo escribir comandos. Una GUI incluye componentes como íconos gráficos e indicadores visuales, así como barras de herramientas, menús y cuadros de diálogo. Estos permiten que la interacción entre el usuario y la aplicación de software se realice de manera más fluida mediante la manipulación directa de los elementos gráficos.

Las aplicaciones de software han mejorado enormemente a lo largo de los años. Las primeras aplicaciones de software funcionaban con comandos que debían escribirse, lo que llamamos interfaces de **línea de comandos (CLI)**. Más tarde se aprovecharon las ventajas de las GUI.

| Interfaces de Línea de Comandos (CLI) | Interfaces Gráficas de Usuario (GUI) |
|---------------------------------------|---------------------------------------|
| **Ventajas**                          | **Ventajas**                          |
| • Más fáciles de implementar por un programador | • Los usuarios no necesitan recordar comandos específicos – más fácil para usuarios nuevos |
| • Requieren menos memoria para ejecutarse | • Los usuarios usan íconos para recordar comandos |
| • Pueden ejecutarse en sistemas sin monitor gráfico | • Los comandos están agrupados en menús y barras de herramientas |
| • Más rápido escribir un comando que usar un ratón – los usuarios experimentados pueden encontrarlo útil | |
| **Desventajas**                       | **Desventajas**                       |
| • Los usuarios deben recordar comandos específicos – difícil para usuarios nuevos | • Más complejas de implementar por un programador |
|                                       | • Requieren más memoria               |
|                                       | • Requieren un monitor gráfico y un dispositivo apuntador |

## 2.1.9. Bit, byte, binario, decimal y hexadecimal

En informática, toda la información, ya sean números, texto, imágenes o sonidos, se representa internamente mediante códigos numéricos. Esta representación permite que los sistemas informáticos almacenen, procesen y transmitan datos de manera eficiente y precisa. Los sistemas binario y hexadecimal son fundamentales para esta representación.

### Sistema Binario

El **sistema binario** es el más básico y esencial en la informática. Está compuesto solo por dos dígitos: `0` y `1`. Estos dígitos, conocidos como bits, son la base del almacenamiento y procesamiento de datos en los ordenadores. Cada bit representa un estado de encendido (`1`) o apagado (`0`), lo que se relaciona directamente con los circuitos electrónicos del hardware de los dispositivos.

En informática, los datos más complejos, como caracteres y números, se construyen a partir de combinaciones de bits. Por ejemplo, un byte (8 bits) puede representar valores en un rango de `0` a `255`, permitiendo representar caracteres según códigos específicos, como ASCII o Unicode.

### Sistema Hexadecimal

El **sistema hexadecimal** es una extensión conveniente del binario, que utiliza 16 dígitos: del `0` al `9` y las letras `A` a `F`. Cada dígito hexadecimal representa exactamente 4 bits (un "nibble") en binario, lo cual facilita la lectura y escritura de datos binarios largos.

Por ejemplo:
- `A` en hexadecimal es igual a `1010` en binario.
- `F` en hexadecimal es igual a `1111` en binario.

El sistema hexadecimal es ampliamente utilizado en programación y diseño de sistemas debido a su capacidad para condensar grandes cadenas de bits en una forma más compacta y comprensible.

### Relación entre los Códigos Binario y Hexadecimal

En informática, los códigos binario y hexadecimal son complementarios:
- **Binario** es el formato de representación que entienden los circuitos electrónicos de los ordenadores. Es esencial en el nivel más bajo, donde se realizan operaciones lógicas y aritméticas.
- **Hexadecimal** simplifica la manipulación y visualización de datos binarios, permitiendo a los desarrolladores representar grupos de 4 bits con un solo dígito. Esto es especialmente útil para direcciones de memoria y valores de color en gráficos.

Gracias a esta relación, el sistema hexadecimal sirve como una "capa intermedia" que permite representar la información de manera más legible sin perder la precisión del código binario.

### ¿Qué es el código binario?

El **código binario** es un sistema numérico en el que solo se emplean dos dígitos: **0** y **1**. Cada posición en un número binario representa una potencia de 2, de forma similar a cómo el sistema decimal utiliza potencias de 10. Por ejemplo, el número binario **101** en el sistema decimal se lee como:

  ```1 × 2² + 0 × 2¹ + 1 × 2⁰ = 4 + 0 + 1 = 5```

### Conceptos básicos del sistema binario
El sistema binario es la base de la informática y los sistemas digitales, ya que permite representar y procesar información de manera eficiente. Al comprender cómo funciona el sistema binario y su relación con el sistema decimal, podemos entender cómo se almacenan y transmiten datos en los dispositivos electrónicos.

### Sistema de numeración binario vs. sistema decimal
El **sistema binario** y el **sistema decimal** son dos sistemas de numeración que utilizan diferentes bases:

- **Sistema decimal (base 10):** Es el sistema que usamos habitualmente y se compone de diez dígitos (0, 1, 2, 3, 4, 5, 6, 7, 8 y 9). Cada posición en un número decimal representa una potencia de 10, lo que significa que el valor total se calcula multiplicando cada dígito por una potencia de 10 en función de su posición.

  ```3 × 10² + 4 × 10¹ + 5 × 10⁰ = 300 + 40 + 5 = 345```

- **Sistema binario (base 2):** Este sistema utiliza solo dos dígitos, 0 y 1. Cada posición en un número binario representa una potencia de 2. Este sistema es ideal para la computación porque los circuitos electrónicos solo necesitan dos estados (por ejemplo, encendido y apagado) para procesar los datos.

  ```1 × 2⁸ + 0 × 2⁷ + 1 × 2⁶ + 0 × 2⁵ + 1 × 2⁴ + 1 × 2³ + 0 × 2² + 0 × 2¹ + 1 × 2⁰ = 256 + 0 + 64 + 0 + 16 + 8 + 0 + 0 + 1 = 345``` 

### Dígitos binarios: el uso de 0 y 1
En el sistema binario, cada **dígito** se denomina **bit** y puede tener solo dos valores: **0** o **1**. Esta simplicidad hace que los dispositivos electrónicos puedan procesar datos mediante señales eléctricas, donde un valor alto (por ejemplo, encendido) puede representar el 1 y un valor bajo (apagado) puede representar el 0. La combinación de múltiples bits permite representar cantidades más grandes y complejas.

Cada bit en una secuencia binaria representa una potencia de 2, de derecha a izquierda:

- El primer bit representa 2⁰ (1),
- El segundo bit representa 2¹ (2),
- El tercero representa 2² (4), y así sucesivamente.

Esto permite que una combinación de bits pueda representar cualquier número decimal.

### Bits y bytes: unidad de medida en binario
Un **bit** es la unidad más pequeña de información en el sistema binario. Sin embargo, trabajar con bits individuales sería poco práctico en la mayoría de las aplicaciones. Por esta razón, los bits se agrupan en conjuntos de 8 llamados **bytes**.

    <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%202.%20Organizaci%C3%B3n%20de%20computadores.png" alt="Conexión del dispositivo E/S" width="550" height="auto"/>
    <p><em>Figura 9: Byte. Fuente: Kostas Dimitriou, Markos Hatzitaskos</em></p>
  </div>

- **Byte:** Un byte contiene 8 bits y puede representar 256 valores distintos (de 00000000 a 11111111 en binario, que es de 0 a 255 en decimal). Los bytes son la unidad de medida estándar en almacenamiento y procesamiento de datos.

- **Kilobyte (KB), Megabyte (MB), Gigabyte (GB), etc.:** A medida que se requiere más espacio para almacenar datos, los bytes se agrupan en unidades mayores. Un kilobyte (KB) equivale a 1,024 bytes, un megabyte (MB) es 1,024 kilobytes, y así sucesivamente. Este sistema jerárquico permite medir grandes cantidades de información de manera ordenada y comprensible.

### Conversión de números decimales a binario
La conversión del sistema decimal a binario se realiza mediante el **método de divisiones sucesivas**, que descompone el número decimal en una secuencia de 0s y 1s.

#### Método de divisiones sucesivas

El **método de divisiones sucesivas** es una técnica simple para convertir un número decimal en binario. Consiste en dividir el número decimal sucesivamente entre 2 y anotar el residuo de cada división. Los restos obtenidos representan los dígitos binarios, y el número binario se forma leyendo los restos de abajo hacia arriba (del último al primero).

**Pasos del método:**

1. Divide el número decimal entre 2.
2. Anota el residuo (0 o 1), que se convierte en el dígito binario.
3. Divide el cociente obtenido nuevamente entre 2.
4. Repite los pasos hasta que el cociente sea 0.
5. El número binario se forma con los restos leídos de abajo hacia arriba.

##### Ejemplo paso a paso de conversión de decimal a binario
Convertimos el número decimal **345** a binario siguiendo el método de divisiones sucesivas: 
  
	345 ÷ 2 = 172, residuo 1
	172 ÷ 2 = 86, residuo 0
	86 ÷ 2 = 43, residuo 0
	43 ÷ 2 = 21, residuo 1
	21 ÷ 2 = 10, residuo 1
	10 ÷ 2 = 5, residuo 0
	5 ÷ 2 = 2, residuo 1
	2 ÷ 2 = 1, residuo 0
	1 ÷ 2 = 0, residuo 1

Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```345₁₀ = 101011001₂```
 
Así que el número decimal **345** es **101011001** en binario.

##### Ejercicios prácticos para convertir números decimales a binario
Apliquemos el método de divisiones sucesivas en diferentes números decimales, con tal de obtener el número binario: 

**Convertir el número decimal 27 a binario**
  
  27 ÷ 2 = 13, residuo 1
	13 ÷ 2 = 6, residuo 1
	6 ÷ 2 = 3, residuo 0
	3 ÷ 2 = 1, residuo 1
	1 ÷ 2 = 0, residuo 1

Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```27₁₀ = 11011₂```

Así que el número decimal **27** es **11011** en binario.

**Convertir el número decimal 58 a binario**
  
	58 ÷ 2 = 29, residuo 0
	29 ÷ 2 = 14, residuo 1
	14 ÷ 2 = 7, residuo 0
	7 ÷ 2 = 3, residuo 1
	3 ÷ 2 = 1, residuo 1
	1 ÷ 2 = 0, residuo 1

Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```58₁₀ = 111010₂```

Así que el número decimal **58** es **111010** en binario.

**Convertir el número decimal 100 a binario**
  
	100 ÷ 2 = 50, residuo 0
	50 ÷ 2 = 25, residuo 0
	25 ÷ 2 = 12, residuo 1
	12 ÷ 2 = 6, residuo 0
	6 ÷ 2 = 3, residuo 0
	3 ÷ 2 = 1, residuo 1
	1 ÷ 2 = 0, residuo 1

Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```100₁₀ = 1100100₂```

Así que el número decimal **100** es **1100100** en binario.

### Conversión de binario a decimal
La conversión del sistema binario a decimal se realiza mediante el **método de multiplicación y suma de potencias de 2**.

#### Método de multiplicación y suma de potencias de 2
El **método de multiplicación y suma de potencias de 2** permite convertir un número binario en su equivalente decimal. Consiste en descomponer el número binario, multiplicando cada dígito (0 o 1) por una potencia de 2 basada en su posición de derecha a izquierda, empezando desde el exponente 0.

  **Pasos del método:**

1. Escribe el número binario y anota la potencia de 2 correspondiente a cada posición de derecha a izquierda.
2. Multiplica cada dígito binario (0 o 1) por su potencia de 2 correspondiente.
3. Suma los resultados de cada multiplicación para obtener el valor decimal.

##### Ejemplo paso a paso de conversión de binario a decimal
Convertimos el número binario **1011** a decimal siguiendo el método de multiplicación y suma de potencias de 2:
  
1. Escribimos el número binario y asignamos una potencia de 2 a cada posición:
  
  ```1 × 2³ + 0 × 2² + 1 × 2¹ + 1 × 2⁰```
 
2. Multiplicamos cada dígito binario por su correspondiente potencia de 2:
  
  ```1 × 8 + 0 × 4 + 1 × 2 + 1 × 1 = 8 + 0 + 2 + 1```

3. Sumamos los resultados para obtener el valor decimal:
  
  ```8 + 0 + 2 + 1 = 11```

  Por lo tanto, el número binario **1011** es igual a **11** en decimal.

##### Ejercicios prácticos para convertir números binarios a decimal
Apliquemos el método de multiplicación y suma de potencias de 2 en diferentes números binarios, con tal de obtener el número decimal: 

**Convertir el número binario 1101 a decimal**

	1 × 2³ + 1 × 2² + 0 × 2¹ + 1 × 2⁰
	1 × 8 + 1 × 4 + 0 × 2 + 1 × 1 = 8 + 4 + 0 + 1
	8 + 4 + 0 + 1 = 13

Así que el número binario **11011** es **13** en decimal.

**Convertir el número binario 10010 a decimal**

	1 × 2⁴ + 0 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰
	1 × 16 + 0 × 8 + 0 × 4 + 1 × 2 + 0 × 1 = 16 + 0 + 0 + 2 + 0
	16 + 0 + 0 + 2 + 0 = 18

Así que el número binario **10010** es **18** en decimal.

**Convertir el número binario 111001 a decimal**

	1 × 2⁵ + 1 × 2⁴ + 1 × 2³ + 0 × 2² + 0 × 2¹ + 1 × 2⁰
	1 × 32 + 1 × 16 + 1 × 8 + 0 × 4 + 0 × 2 + 1 × 1 = 32 + 16 + 8 + 0 + 0 + 1
	32 + 16 + 8 + 0 + 0 + 1 = 57

Así que el número binario **111001** es **57** en decimal.

### Representación binaria de caracteres: Código ASCII
El sistema binario no solo se utiliza para representar números, sino también para codificar caracteres y símbolos a través de códigos estándar como el **Código ASCII**. Este sistema permite que las computadoras representen letras, números y otros caracteres mediante secuencias de 0s y 1s.

#### Introducción al código ASCII

El **Código ASCII (American Standard Code for Information Interchange)** es un estándar de codificación de caracteres desarrollado en los años 60 para representar letras, números y símbolos comunes. Cada carácter en ASCII se representa mediante un número decimal que va de 0 a 127, y estos números se convierten en una secuencia de 7 bits en binario. Con ASCII extendido, se llega a representar hasta 256 caracteres, utilizando 8 bits (1 byte) por carácter.

ASCII facilita la interoperabilidad entre diferentes sistemas y dispositivos, ya que se ha convertido en un estándar universal para representar texto en binario. Cada letra, número o símbolo tiene un código único; por ejemplo:

  - La letra "A" tiene el valor decimal 65, que en binario es **01000001**.
  - La letra "a" tiene el valor decimal 97, que en binario es **01100001**.

  <div style="text-align: center;">
  <img src="https://elcodigoascii.com.ar/codigo-americano-estandar-intercambio-informacion/codigo-ascii.png" alt="XT color" width="1199" height="669"/>
  <p><em>Figura 1: El código ASCII. Fuente: <a href="https://elcodigoascii.com.ar/">El codigo ASCII</a></em></p>
  </div>

#### Conversión de letras y caracteres a código binario
Para convertir letras y caracteres al sistema binario usando el código ASCII, basta con seguir estos pasos:

1. Identificar el valor decimal de la letra o símbolo según la tabla ASCII.
2. Convertir ese valor decimal en binario.

##### 5.3. Ejemplos de codificación binaria de palabras
Veamos algunos ejemplos de cómo se puede codificar una palabra en binario utilizando el código ASCII. Tomemos la palabra **"Hi"** como ejemplo:

1. **H**:
  - Valor decimal: 72
- Binario: 01001000
  
2. **i**:
  - Valor decimal: 105
  - Binario: 01101001
    
Así, la palabra "Hi" en binario sería:
**"Hi"** = 01001000 01101001

Otro ejemplo con la palabra "Cat":

1. **C**:
  - Valor decimal: 67
  - Binario: 01000011
    
2. **a**:
  - Valor decimal: 97
  - Binario: 01100001

3. **t**:
  - Valor decimal: 116
  - Binario: 01110100

Entonces, **"Cat"** en binario sería:
**"Cat"** = 01000011 01100001 01110100

### Operaciones básicas en binario
Las operaciones en binario son fundamentales en el procesamiento de datos y en los cálculos realizados por las computadoras. Estas operaciones incluyen la suma, resta, multiplicación y división, que se llevan a cabo utilizando las reglas propias del sistema binario, donde solo intervienen los dígitos 0 y 1.

#### Suma binaria
La **suma binaria** sigue reglas similares a la suma en el sistema decimal, pero debido a que solo tiene dos dígitos (0 y 1), las combinaciones de suma son más simples:

  - 0 + 0 = 0
  - 0 + 1 = 1
  - 1 + 0 = 1
  - 1 + 1 = 10 (equivale a 0 y lleva 1 al siguiente dígito, similar a cómo llevamos 1 en el sistema decimal)

**Ejemplo**: Sumar **1011** y **1101**

	  1011
  	+ 1101
	--------
 	 11000

Pasos: 
1. Sumamos de derecha a izquierda: 1 + 1 = 10 (escribimos 0 y nos llevamos 1).
2. Sumamos el siguiente dígito con el acarreo: 1 + 0 + 1 = 10 (escribimos 0 y nos llevamos 1).
3. Continuamos hasta obtener el resultado final: **11000**.

#### Resta binaria
La **resta binaria** también sigue reglas similares a la resta decimal, pero con solo dos dígitos posibles. En este caso, se necesita hacer un préstamo si se resta un 1 de un 0, tal como en el sistema decimal:

  - 0 - 0 = 0
  - 1 - 0 = 1
  - 1 - 1 = 0
  - 0 - 1 = 1 (con préstamo, que equivale a restar 1 de la columna siguiente)

**Ejemplo**: Restar **1101** y **10101**

  	  10101
  	- 01101
	--------
 	  01000

Pasos: 
1. De derecha a izquierda: 1 - 1 = 0.
2. En la siguiente columna: 0 - 0 = 0.
3. Continuamos restando, pidiendo préstamos donde sea necesario, hasta obtener **01000**.

#### Multiplicación y división en binario
La **multiplicación binaria** es similar a la multiplicación en el sistema decimal y sigue reglas sencillas:

  - 0 x 0 = 0
  - 1 x 0 = 0
  - 0 x 1 = 0
  - 1 x 1 = 1

**Ejemplo**: Multiplicar **101** y **11**

            101
        x    11
        --------
            101 (101 x 1)
        +  1010 (101 x 10, desplazado una posición a la izquierda)
        --------
           1111
  
La **división binaria** también sigue el mismo principio que la división en decimal, pero utilizando las reglas binarias. Es un poco más compleja y se basa en la resta sucesiva de valores, similar al método de la división larga en decimal.

**Ejemplo**: Dividir **1101** y **10**

  	1101 ÷ 10
  	      110
	--------
 	10 | 1101
	     - 10
	--------
 	      100
 	     - 10
	--------
 	       01
         
  Pasos: 
  1. Tomamos los primeros dos dígitos del dividendo (1101), que son **11**. Como **11** es mayour que **10**, podemos dividir:
     **11 ÷ 10** da un cociente de **1** y un residuo de **1**.
     Colocamos **1** en el cociente y bajamos el siguiente dígito para tener **100**.
  2. Ahora, dividimos 100 entre 10:
     **100 ÷ 10** da un cociente de **1** y un residuo de **0**.
     Colocamos **1** en el cociente y bajamos el siguiente dígito para tener **01**.
  3. Finalmente, **01*** es menor que **10**, por lo que es nuestro residuo final.
  4. Resultado: un cociente de **110** con un residuo de **1** en binario.

### Aplicaciones del código binario
El código binario es la base de toda la tecnología digital. Su uso permite que las computadoras y otros dispositivos digitales representen, almacenen y procesen distintos tipos de datos. Gracias al sistema binario, es posible manejar la información de manera eficiente, fiable y segura en múltiples áreas de aplicación.

Introducción al Sistema Hexadecimal

El sistema hexadecimal es un sistema de numeración que utiliza 16 símbolos, lo que permite representar grandes cantidades de información en un formato compacto y legible. Este sistema es ampliamente utilizado en informática debido a su relación directa con el sistema binario, que es el lenguaje básico de las computadoras.

### ¿Qué es el sistema hexadecimal?

El sistema hexadecimal es un sistema de base 16, lo que significa que utiliza 16 dígitos distintos para representar valores. Estos dígitos van del `0` al `9` y luego de la `A` a la `F`, donde:

- `0` a `9` representan los valores decimales de 0 a 9.
- `A` a `F` representan los valores decimales de 10 a 15.

Por ejemplo:
- El valor hexadecimal `A` equivale al valor decimal `10`.
- El valor hexadecimal `F` equivale al valor decimal `15`.

Este sistema se utiliza en muchas áreas de la informática para representar datos de una manera más legible, especialmente en casos donde el binario sería demasiado extenso.

#### Comparación con otros sistemas de numeración (decimal y binario)

En informática, es común trabajar con varios sistemas de numeración:

- **Sistema decimal**: Es el sistema numérico que usamos en la vida cotidiana. Es de base 10 y utiliza los dígitos del `0` al `9`.
- **Sistema binario**: Es el sistema numérico utilizado por los computadores. Es de base 2 y utiliza solo los dígitos `0` y `1`.

El sistema hexadecimal se sitúa entre el binario y el decimal en términos de legibilidad y conveniencia:

- **Binario a hexadecimal**: Cada dígito hexadecimal representa 4 bits en binario. Esto permite condensar grandes cantidades de datos binarios en una forma mucho más corta y comprensible.
- **Decimal a hexadecimal**: Aunque el decimal es más fácil de entender para los humanos, el hexadecimal facilita la representación de grandes números en un formato que se relaciona directamente con el hardware de los computadores.

Por ejemplo:
- El número binario `1111` se representa como `F` en hexadecimal.
- El número decimal `255` se representa como `FF` en hexadecimal.

#### Importancia y uso del sistema hexadecimal en informática

El sistema hexadecimal es esencial en informática por varias razones:

1. **Representación compacta**: Dado que cada dígito hexadecimal corresponde a 4 bits, el hexadecimal permite una representación más compacta y legible de datos en comparación con el binario.
   
2. **Direcciones de memoria**: En sistemas informáticos, las direcciones de memoria suelen expresarse en hexadecimal para facilitar su lectura y manejo, ya que las direcciones en binario serían demasiado largas y complejas de interpretar.

3. **Colores en diseño gráfico**: En el desarrollo web y diseño gráfico, los colores se representan comúnmente en formato hexadecimal. Por ejemplo, el color `#FF5733` en HTML representa un color específico en código hexadecimal.

4. **Depuración y programación de bajo nivel**: Los programadores y técnicos a menudo usan el hexadecimal al trabajar directamente con hardware o depurar software a nivel de máquina, ya que facilita la interpretación de instrucciones y datos en registros de memoria.

En resumen, el sistema hexadecimal ofrece una forma intermedia entre la legibilidad humana y la precisión binaria, haciéndolo indispensable en el campo de la informática y la electrónica.

### Estructura del Sistema Hexadecimal

El sistema hexadecimal se organiza de forma que cada posición en un número representa una potencia de 16. Esto permite expresar valores grandes en un formato compacto y eficiente, utilizando solo los dígitos del `0` al `9` y las letras `A` a `F`.

#### Valores y representación de los dígitos hexadecimales (0-9 y A-F)

En hexadecimal, cada dígito puede tomar 16 valores distintos, que van del `0` al `F`. Los valores numéricos de estos dígitos son:

- `0` a `9`: Representan los valores decimales `0` a `9`.
- `A` a `F`: Representan los valores decimales `10` a `15`.

Este esquema de dígitos permite representar cualquier número en base 16. Cada uno de estos dígitos ocupa 4 bits en binario, lo que hace que la conversión entre binario y hexadecimal sea directa y conveniente. Por ejemplo:

- El valor hexadecimal `A` se convierte en `1010` en binario.
- El valor hexadecimal `F` se convierte en `1111` en binario.

Esta correspondencia directa entre hexadecimal y binario es la razón por la que el sistema hexadecimal se usa ampliamente en informática, ya que permite representar datos binarios de manera más legible y compacta.

#### Potencias de 16 y lugar de cada dígito en el sistema hexadecimal

Cada posición en un número hexadecimal representa una potencia de 16, comenzando desde la derecha con \(16^0\), luego \(16^1\), \(16^2\), y así sucesivamente hacia la izquierda. Por ejemplo, en el número hexadecimal `2AF3`, cada dígito tiene el siguiente valor posicional:

- `3` está en la posición de \(16^0\), por lo que su valor es \(3 \times 16^0 = 3\).
- `F` está en la posición de \(16^1\), lo que equivale a \(15 \times 16^1 = 240\) (recordando que `F` representa 15 en decimal).
- `A` está en la posición de \(16^2\), por lo que su valor es \(10 \times 16^2 = 2560\) (dado que `A` representa 10 en decimal).
- `2` está en la posición de \(16^3\), por lo que su valor es \(2 \times 16^3 = 8192\).

La suma de estos valores da el valor decimal del número hexadecimal `2AF3`:

\[
8192 + 2560 + 240 + 3 = 10995
\]

Esta estructura permite que los números hexadecimales representen grandes valores en menos espacio y facilita la conversión entre sistemas numéricos. Los desarrolladores y técnicos informáticos utilizan esta organización para manipular datos de manera eficiente, especialmente en el contexto de direcciones de memoria y valores de colores en gráficos.

### Conversión de Hexadecimal a Binario

La conversión de hexadecimal a binario es un proceso directo que facilita la representación de datos en un formato que los ordenadores pueden procesar fácilmente. Dado que cada dígito hexadecimal corresponde exactamente a 4 bits en binario, esta conversión es simple y eficiente.

#### Tabla de equivalencias de dígitos hexadecimales a binario

Para facilitar la conversión, aquí tienes una tabla de equivalencias entre los dígitos hexadecimales y sus representaciones en binario de 4 bits:

| Hexadecimal | Binario |
|-------------|---------|
| 0           | 0000    |
| 1           | 0001    |
| 2           | 0010    |
| 3           | 0011    |
| 4           | 0100    |
| 5           | 0101    |
| 6           | 0110    |
| 7           | 0111    |
| 8           | 1000    |
| 9           | 1001    |
| A           | 1010    |
| B           | 1011    |
| C           | 1100    |
| D           | 1101    |
| E           | 1110    |
| F           | 1111    |

Esta tabla permite convertir cada dígito hexadecimal individualmente a binario de forma rápida y sencilla.

#### Método de conversión de cada dígito hexadecimal en su equivalente binario de 4 bits

Para convertir un número hexadecimal a binario, simplemente convierte cada dígito hexadecimal a su equivalente binario de 4 bits utilizando la tabla anterior. El resultado es la concatenación de estos grupos de 4 bits.

Por ejemplo, para convertir el número hexadecimal `2F` a binario:

1. Toma el primer dígito, `2`, que en binario es `0010`.
2. Toma el segundo dígito, `F`, que en binario es `1111`.
3. Concatenando ambos resultados, `2F` en hexadecimal se convierte en `00101111` en binario.

Este método permite una conversión rápida sin necesidad de cálculos adicionales, ya que cada dígito hexadecimal se traduce directamente a un bloque de 4 bits.

##### Ejemplos prácticos de conversión de hexadecimal a binario

A continuación, se muestran algunos ejemplos prácticos de conversión para ayudar a comprender el proceso:

1. **Ejemplo 1**: Convertir `1A3` a binario
   - `1` en hexadecimal es `0001` en binario.
   - `A` en hexadecimal es `1010` en binario.
   - `3` en hexadecimal es `0011` en binario.
   - Resultado: `1A3` en hexadecimal es `000110100011` en binario.

2. **Ejemplo 2**: Convertir `4F9` a binario
   - `4` en hexadecimal es `0100` en binario.
   - `F` en hexadecimal es `1111` en binario.
   - `9` en hexadecimal es `1001` en binario.
   - Resultado: `4F9` en hexadecimal es `010011111001` en binario.

3. **Ejemplo 3**: Convertir `B2E` a binario
   - `B` en hexadecimal es `1011` en binario.
   - `2` en hexadecimal es `0010` en binario.
   - `E` en hexadecimal es `1110` en binario.
   - Resultado: `B2E` en hexadecimal es `101100101110` en binario.

Estos ejemplos muestran cómo el proceso de conversión de hexadecimal a binario puede aplicarse a cualquier número hexadecimal, proporcionando una forma rápida de representar valores en un formato adecuado para el procesamiento en sistemas digitales.

### Conversión de Binario a Hexadecimal

La conversión de binario a hexadecimal se basa en la agrupación de bits en bloques de 4, ya que cada bloque de 4 bits corresponde exactamente a un dígito hexadecimal. Este método es eficiente y rápido, dado que evita cálculos complejos y aprovecha la relación directa entre estos dos sistemas numéricos.

#### Agrupación de bits en bloques de 4 para obtener dígitos hexadecimales

Para convertir un número binario a hexadecimal, sigue estos pasos:

1. **Agrupa los bits en bloques de 4**: Comienza desde la derecha del número binario y agrupa los bits en bloques de 4. Si el número total de bits no es múltiplo de 4, agrega ceros a la izquierda para completar el último bloque.
   
2. **Convierte cada bloque de 4 bits a hexadecimal**: Utiliza la tabla de equivalencias para convertir cada bloque de 4 bits en su valor hexadecimal correspondiente.

Por ejemplo:
- Para el número binario `10110111`, agrupamos los bits de derecha a izquierda en bloques de 4: `1011 0111`.
- Luego, cada bloque se convierte a hexadecimal:
  - `1011` se convierte en `B`.
  - `0111` se convierte en `7`.
- Por lo tanto, `10110111` en binario es `B7` en hexadecimal.

Esta técnica hace que la conversión de binario a hexadecimal sea rápida y directa.

##### Ejemplos prácticos de conversión de binario a hexadecimal

A continuación, algunos ejemplos prácticos de conversión para ilustrar el proceso:

1. **Ejemplo 1**: Convertir `11011010` a hexadecimal
   - Agrupamos los bits: `1101 1010`
   - Convertimos cada grupo:
     - `1101` es `D` en hexadecimal.
     - `1010` es `A` en hexadecimal.
   - Resultado: `11011010` en binario es `DA` en hexadecimal.

2. **Ejemplo 2**: Convertir `111100111010` a hexadecimal
   - Agrupamos los bits (añadiendo un `0` a la izquierda para completar el primer bloque): `0001 1110 0111 1010`
   - Convertimos cada grupo:
     - `0001` es `1`.
     - `1110` es `E`.
     - `0111` es `7`.
     - `1010` es `A`.
   - Resultado: `111100111010` en binario es `1E7A` en hexadecimal.

3. **Ejemplo 3**: Convertir `101011` a hexadecimal
   - Agrupamos los bits (añadiendo ceros a la izquierda): `0010 1011`
   - Convertimos cada grupo:
     - `0010` es `2`.
     - `1011` es `B`.
   - Resultado: `101011` en binario es `2B` en hexadecimal.

Estos ejemplos muestran que el método de agrupar en bloques de 4 bits simplifica la conversión y permite que cualquier número binario se traduzca rápidamente a hexadecimal.

### Aplicaciones Prácticas del Sistema Hexadecimal

El sistema hexadecimal tiene numerosas aplicaciones prácticas en informática y electrónica, gracias a su capacidad para representar datos binarios de manera compacta y legible. Desde la representación de direcciones de memoria hasta la codificación de colores en diseño gráfico, el hexadecimal es fundamental para varias áreas de la tecnología.

#### Uso en la representación de direcciones de memoria

En sistemas informáticos, las direcciones de memoria se representan comúnmente en hexadecimal. Esto permite que los valores largos en binario se compriman en una forma más legible y manejable. Por ejemplo, una dirección de memoria como `1010 1101 1110 0010` en binario se convierte en `ADE2` en hexadecimal, facilitando la lectura y la escritura de las direcciones de memoria.

El uso de hexadecimal para las direcciones es particularmente útil en programación de bajo nivel y en la depuración de sistemas, donde los programadores interactúan directamente con la memoria de la máquina. Gracias al hexadecimal, los desarrolladores pueden acceder, manipular y analizar datos en memoria de forma rápida y eficiente.

#### Representación de colores en HTML y gráficos

En el diseño gráfico y desarrollo web, el sistema hexadecimal es la norma para representar colores. Los colores se expresan con códigos hexadecimales de 6 dígitos, donde cada par de dígitos representa la intensidad de los colores rojo, verde y azul (RGB). Por ejemplo:

- `#FF5733` representa un color con `FF` (255 en decimal) de rojo, `57` (87 en decimal) de verde y `33` (51 en decimal) de azul.
- `#000000` representa el color negro, donde todos los canales están en `00`.
- `#FFFFFF` representa el color blanco, donde todos los canales están en `FF`.

Esta representación hexadecimal de colores permite una amplia gama de colores (16,777,216 combinaciones posibles) en un formato compacto y estandarizado que los navegadores y programas gráficos interpretan directamente.

#### Otras aplicaciones en informática y electrónica

Además de las direcciones de memoria y la representación de colores, el sistema hexadecimal se utiliza en varias otras aplicaciones en informática y electrónica, tales como:

- **Códigos de máquina y depuración**: Al trabajar con lenguajes de bajo nivel o ensamblador, los códigos de máquina se representan frecuentemente en hexadecimal, lo que facilita la identificación y manipulación de instrucciones específicas.

- **Representación de datos binarios en depuradores**: En entornos de desarrollo y herramientas de depuración, los datos binarios, como el contenido de registros y variables en la memoria, suelen mostrarse en formato hexadecimal para facilitar la visualización y edición de valores binarios complejos.

- **Direcciones MAC en redes**: Las direcciones MAC (Media Access Control) se expresan en hexadecimal. Una dirección MAC típica tiene el formato `00:1A:2B:3C:4D:5E`, donde cada par de dígitos representa 8 bits.

