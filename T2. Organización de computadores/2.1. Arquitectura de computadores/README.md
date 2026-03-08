<h1 align="center">2.1. Arquitectura de computadores
<div align="center">

</div>

## Contenido:

- [2.1.1. Resuma la arquitectura de la unidad central de procesamiento (CPU) y las funciones de la unidad aritmético-lógica (ALU) y de la unidad de control (CU), así como los registros de la CPU](#211-resuma-la-arquitectura-de-la-unidad-central-de-procesamiento-cpu-y-las-funciones-de-la-unidad-aritmético-lógica-alu-y-de-la-unidad-de-control-cu-así-como-los-registros-de-la-cpu)
- [2.1.2. Describa la memoria principal](#212-describa-la-memoria-principal)
- [2.1.3. Explique el uso de la memoria caché](#213-explique-el-uso-de-la-memoria-caché)
- [2.1.4. Explique el ciclo de instrucción de la máquina](#214-explique-el-ciclo-de-instrucción-de-la-máquina)

---

<br>

## 2.1.1. Resuma la arquitectura de la unidad central de procesamiento (CPU) y las funciones de la unidad aritmético-lógica (ALU) y de la unidad de control (CU), así como los registros de la CPU

### ¿Qué es la unidad central de procesamiento?
La **unidad central de procesamiento (CPU)** a menudo se refiere como el “cerebro” del ordenador. Es un componente crítico que lleva a cabo la mayor parte del procesamiento dentro de un dispositivo.

La CPU está compuesta por dos unidades principales: la **unidad de control (CU)** y **la unidad aritmético-lógica (ALU)**.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%201.%20Modelo%20de%20CPU.png" alt="CPU Model" width="450" height="auto"/>
    <p><em>Figura 1: Modelo de CPU. Fuente: Computer Science IB. (Paul Baumgarten, Ioana Ganea, Carl Turland)</em></p>
  </div>

#### Unidad de control (CU)
La unidad de control **dirige las operaciones del procesador**. Es responsable del ciclo de **búsqueda–decodificación–ejecución**, gestionando las tres operaciones y dirigiendo la memoria del ordenador, la ALU y los dispositivos de entrada/salida para que respondan de manera adecuada.

#### Unidad aritmético-lógica (ALU)
Esta unidad es responsable de **realizar operaciones aritméticas y lógicas**. Estas incluyen operaciones aritméticas básicas como la suma, resta, multiplicación y división, así como **operaciones lógicas** incluyendo AND, OR, XOR y NOT.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%202.%20Central%20processing%20unit%20(CPU).jpg" alt="CPU" width="350" height="auto"/>
    <p><em>Figura 2: Central Processing Unit. Fuente: PcCompomentes</em></p>
  </div>

###  ¿Qué son los registros?
Los registros son cantidades muy pequeñas de almacenamiento que están disponibles directamente en la CPU para **mantener datos temporales** con los que la CPU puede estar trabajando. Los registros son el **registro de instrucciones** (IR), el **contador de programa** (PC), el **registro de direcciones de memoria** (MAR), el **registro de datos de memoria** (MDR) y el **acumulador** (AC).

#### Registro de instrucciones
Cuando una instrucción es captada desde la memoria, se mantiene en el IR dentro de la CPU. Este registro contiene la instrucción que está siendo ejecutada actualmente por la CPU.

#### Contador de programa
El PC contiene **la dirección de la siguiente instrucción** que debe ser captada desde la memoria. Una vez que la instrucción ha sido captada, el PC se actualiza para apuntar a la siguiente instrucción que será necesaria.

#### Registro de direcciones de memoria
El MAR contiene **la dirección de memoria que está siendo captada actualmente**. El contenido del PC se copia en el MAR, y el MAR proporciona esta dirección a la unidad de memoria, de modo que los datos e instrucciones puedan ser leídos desde o copiados a esa ubicación.

#### Registro de datos de memoria
Este contiene los datos que han sido captados o que están a punto de ser escritos en la dirección de memoria que está actualmente en el MAR.

#### Acumulador (AC)
Este almacena los resultados aritméticos o lógicos intermedios producidos por la ALU.

## ¿Qué son los buses?
Los buses son un **componente crítico** del sistema informático, ya que transfieren datos entre varios dispositivos, incluyendo la CPU, la memoria, el almacenamiento y los periféricos. Los buses tienen anchos que se miden en bits. Cuanto mayor es el ancho del bus, más datos puede transmitir a la vez.
Existen tres tipos principales de buses: bus de control, bus de datos y bus de direcciones.

### Bus de control
El bus de control se utiliza para transmitir señales de comando y de control desde la CPU a otros componentes del sistema, y viceversa. Debido a la necesidad de que las señales sean enviadas y recibidas, este bus es bidireccional. Algunas de las señales que se transmitirían a través del bus de control son operaciones de lectura/escritura, peticiones de interrupción, señales de reloj para sincronización y señales de estado de los componentes de hardware.

### Bus de datos
El bus de datos **transporta los datos que están siendo procesados entre la CPU, la memoria y otros periféricos**. El ancho del bus de datos es importante para determinar la cantidad de datos que puede transferir a la vez. Los anchos comunes de los buses de datos son 8, 16, 32 y 64 bits. Como los datos necesitan ser leídos y escritos en la memoria, los buses de datos suelen ser bidireccionales.

### Bus de direcciones
El bus de direcciones se utiliza para transmitir la dirección que debe ser leída o escrita en la memoria. El ancho de este bus determina la capacidad de memoria del sistema. Por ejemplo, un bus de direcciones de **32 bits** puede direccionar $2^{32}$ ubicaciones de memoria.

### ¿Qué son los núcleos?
Las CPU vienen en varias configuraciones diferentes. Estas incluyen procesadores de un solo **núcleo**, **procesadores multinúcleo** y **coprocesadores**.

#### Procesadores de un solo núcleo
Esta CPU tiene una **única unidad de procesamiento**, lo que significa que solo puede manejar una tarea a la vez. Se encuentran con mayor frecuencia en ordenadores de **gama baja** o en **máquinas más antiguas**. Son adecuados para tareas simples que no requieren un alto nivel de multitarea. Los procesadores de un solo núcleo pueden ejecutar más de una aplicación a la vez, pero la CPU tiene que ser compartida entre estas aplicaciones, lo cual puede afectar al rendimiento.

#### Procesadores multinúcleo
Una **CPU con procesadores multinúcleo** tiene dos o más núcleos que pueden ejecutar múltiples instrucciones simultáneamente. A menudo se les denomina como de doble núcleo (dos procesadores), de cuatro núcleos (cuatro procesadores), de seis núcleos (hexa-core) o de ocho núcleos (octa-core). Su rendimiento es **significativamente más rápido que el de los procesadores de un solo núcleo** y son ideales para la multitarea, los videojuegos y los servidores. Sin embargo, el software debe estar escrito para aprovechar estos núcleos adicionales. El software más antiguo que no hace esto probablemente se ejecute a una velocidad similar a la de un procesador de un solo núcleo.

#### Coprocesadores
Un **coprocesador es un tipo especial de procesador que tiene una tarea específica para apoyar a la CPU principal**. Están construidos con un propósito concreto para lograr un rendimiento óptimo en comparación con una CPU de propósito general. Las tareas se descargan de la CPU al coprocesador para que puedan ejecutarse en paralelo, mejorando el rendimiento del sistema. Ejemplos de coprocesadores son las unidades de procesamiento gráfico (cubiertas en la Sección A1.1.2), los procesadores de audio y **los procesadores de señal digital (DSP)**, que se utilizan en telecomunicaciones y compresión de imágenes.

<br>

## 2.1.2. Describa la memoria principal

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

## 2.1.3. Explique el uso de la memoria caché

La **memoria caché** es pequeña, pero ofrece acceso de alta velocidad a la CPU en comparación con la RAM. Actúa como un búfer entre la CPU y la RAM más lenta, almacenando datos e instrucciones de uso frecuente.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%208.%20Jerarqu%C3%ADa%20de%20memoria.png" alt="ROM" width="450" height="auto"/>
    <p><em>Figura 8: Memoria Caché. Fuente: Computer Science IB. (Paul Baumgarten, Ioana Ganea, Carl Turland)</em></p>
  </div>

Existen tres tipos de caché: **L1, L2 y L3**, cada una con diferentes tamaños y velocidades. Cuanto más cerca de la CPU se encuentre, más rápida es.

- **Caché L1**: se encuentra directamente en la CPU, lo que la convierte en la más rápida. Puede accederse a ella casi al instante debido a su ubicación. Sin embargo, también es la más pequeña, normalmente de solo unos pocos kilobytes (32KB a 128KB por núcleo). Cada núcleo de CPU suele tener su propia caché L1, que normalmente se divide en dos secciones: **L1i** para almacenar instrucciones y **L1d** para almacenar datos.
- **Caché L2**: puede estar en la CPU, como la L1, o situada muy cerca de ella. La caché L2 es más grande que la L1 y puede tener hasta varios megabytes de tamaño (256KB a 2MB por núcleo), proporcionando más espacio para almacenar instrucciones de uso frecuente. Es más rápida que la L3, pero un poco más lenta que la L1, aunque sigue acelerando significativamente el procesamiento al reducir la necesidad de acceder a la RAM más lenta.
- **Caché L3**: suele encontrarse más alejada del chip de la CPU. La caché L3 puede ser compartida entre varios núcleos en las CPU multinúcleo, mientras que L1 y L2 suelen ser exclusivas de un solo núcleo. Es la más grande de las tres y puede alcanzar decenas de megabytes (2MB a 64MB compartidos entre todos los núcleos). Es la más lenta de los tres tipos de caché, pero aún así es mucho más rápida que la RAM.

Los términos **acierto de caché (cache hit) y fallo de caché (cache miss)** se utilizan para describir la eficiencia de la memoria caché de la CPU al recuperar datos.

- Un **acierto de caché** es el escenario ideal: la CPU solicita datos y estos se encuentran en la memoria caché.
- Un **fallo de caché** significa que no se encontraron, lo que obliga a recuperarlos desde la memoria principal (RAM) más lenta o incluso desde un almacenamiento todavía más lento (SSD / HDD).

> [!TIP]
> Imagina una cebolla, con sus capas representando los niveles de caché:
>
> La **caché L1** es la más pequeña y rápida, como el centro mismo de la cebolla, donde todo está muy compacto y más cerca del núcleo de la CPU.
>
> La **caché L2** es un poco más grande y más lenta, como la siguiente capa hacia afuera: todavía cerca del centro, pero no tan rápida de acceder como el núcleo.
> 
> La **caché L3** es la más grande y lenta, como las capas exteriores de la cebolla. Sigue siendo importante, pero se tarda un poco más en llegar a ella, de la misma forma que la CPU necesita más tiempo para acceder a los datos en la caché L3 en comparación con L1 y L2.

#### Optimización del rendimiento de la CPU con caché

La caché desempeña un papel fundamental para garantizar que la CPU pueda acceder a los datos lo más rápido posible. Cuando la CPU encuentra los datos buscados en la caché (**acierto de caché**), estos pueden procesarse muy rápidamente. Sin embargo, cuando ocurre un **fallo de caché**, la CPU debe buscar los datos en la memoria más lenta, lo que provoca un retraso.

Imagina que estás jugando a un videojuego en un ordenador. La CPU revisa con frecuencia las cachés L1, L2 y L3 para encontrar los datos que necesita para que el juego funcione sin problemas. Las funciones principales del juego, como los controles del jugador y la lógica del juego, podrían almacenarse en la caché L1, mientras que los datos a los que se accede con menos frecuencia, como las texturas de fondo, pueden estar en la caché L3.

Este sistema por capas ayuda a garantizar que el juego se ejecute de forma fluida, sin interrupciones. Una CPU con una caché más grande o con técnicas de **prefetching** más avanzadas (una técnica mediante la cual la CPU predice qué datos necesitará y los carga en la caché por adelantado) tendrá menos fallos de caché y un mejor rendimiento general.

<br>

## 2.1.4. Explique el ciclo de instrucción de la máquina

El ciclo de búsqueda–decodificación–ejecución, también conocido como “ciclo de instrucción”, es el proceso fundamental que utiliza una CPU para ejecutar instrucciones. El ciclo consta de tres etapas principales:

- **Búsqueda (Fetch):** la CPU obtiene una instrucción de la memoria.
- **Decodificación (Decode):** la CPU interpreta la instrucción y prepara las operaciones necesarias para ejecutarla.
- **Ejecución (Execute):** la CPU realiza las acciones requeridas por la instrucción.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%209.%20The%20fetch-decode-execute%20cycle.png" alt="ROM" width="250" height="auto"/>
    <p><em>Figura 10: The fetch-decode-execute cycle. Fuente: Computer Science IB. (Paul Baumgarten, Ioana Ganea, Carl Turland)</em></p>
  </div>

### Little Man Computer (LMC)

Una forma más sencilla de ver estas etapas con más detalle es utilizar un modelo educativo de CPU conocido como **Little Man Computer**, que puedes buscar en línea o usar en este enlace: [https://peterhigginson.co.uk/lmc](https://peterhigginson.co.uk/lmc).  

Este modelo utiliza **lenguaje ensamblador**, un conjunto simple de instrucciones, cada una representada por tres letras, que se almacena como un código de tres dígitos en la memoria.  

#### Conjunto de instrucciones

| Instrucción | Código | Descripción |
|-------------|--------|-------------|
| **INP** | 901 | Introduce un valor y lo almacena en el acumulador. |
| **OUT** | 902 | Muestra el valor del acumulador. |
| **DAT** | N/A | Define valores de datos directamente en memoria en el punto de declaración, a menudo usados para constantes o variables. |
| **LDA** | 5XX | Carga en el acumulador el valor de la dirección de memoria especificada. |
| **STA** | 3XX | Almacena el valor del acumulador en la dirección de memoria especificada. |
| **ADD** | 1XX | Suma al acumulador el valor de la dirección de memoria especificada. |
| **SUB** | 2XX | Resta al acumulador el valor de la dirección de memoria especificada. |
| **HLT** | 000 | Detiene el programa. |
| **BRA** | 6XX | Salta a la dirección de memoria especificada. |
| **BRZ** | 7XX | Salta a la dirección de memoria especificada si el acumulador es cero. |
| **BRP** | 8XX | Salta a la dirección de memoria especificada si el acumulador es positivo. |

---

#### Ejemplo
Introduce el siguiente programa en la columna de la izquierda y ensámblalo en la RAM.  
Verás la representación de **tres dígitos** para cada instrucción almacenada en una dirección de memoria en la columna de la derecha.  

Por ejemplo:  
`LDA 4` se almacena como **504** en la dirección de memoria **0**.

```
LDA 4
ADD 5
STA 5
HLT
DAT 23
DAT 12
```

LMC se debe ver tal que así:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2010.%20LMC%20Model.png" alt="LMC" width="750" height="auto"/>
    <p><em>Figura 11: LMC Model. Fuente: Peter Higginson</em></p>
  </div>

#### Primer ciclo (Click step)

1. **Búsqueda (Fetch):** El PC (contador de programa) está actualmente en 0, así que se recupera la instrucción en la dirección de memoria 0 (504) abriendo la dirección 0 en la RAM mediante el bus de direcciones y obteniendo la instrucción a través del bus de datos. El bus de control envía una señal de lectura para iniciar este proceso. El valor 5 se almacena en el registro de instrucciones y 04 en el registro de direcciones. Mientras esto sucede, el PC se incrementa a 1 mediante la ALU, preparándose para la siguiente instrucción.

2. **Decodificación (Decode):** Una vez recuperada la instrucción, la CPU la decodifica. La unidad de control utiliza el bus de control para coordinar este proceso. La instrucción almacenada en el registro de instrucciones es 5, que se decodifica como “cargar en el acumulador”. El registro de direcciones 04 indica la dirección de los datos que deben cargarse.

3. **Ejecución (Execute):** Se lleva a cabo la orden. La dirección 4 se abre en el bus de direcciones y el bus de control envía las señales apropiadas para recuperar los datos (23) de esa ubicación a través del bus de datos y almacenarlos en el acumulador.

#### Segundo ciclo (Click step)

1. **Búsqueda (Fetch):** La CPU usa ahora el PC para saber qué instrucción recuperar a continuación: el valor actual es 1. Se abre la dirección 1 y se obtiene la instrucción 105. El bus de control envía una señal de lectura para iniciar este proceso. El valor 1 se almacena en el registro de instrucciones y 05 en el registro de direcciones. El PC se incrementa a 2 mediante la ALU.

2. **Decodificación (Decode):** La instrucción 1 se decodifica como “sumar al acumulador”; el registro de direcciones indica la dirección de los datos que deben sumarse (5). La unidad de control utiliza el bus de control para coordinar este proceso.

3. **Ejecución (Execute):** Se abre la dirección 5, se recuperan los datos (12) y tanto el acumulador (que contiene 23) como los datos recuperados (12) se envían a la ALU. El resultado de 23 + 12 se almacena en el acumulador (35).

#### Tercer ciclo (Click step)

1. **Búsqueda (Fetch):** El PC está actualmente en 2, así que se recupera la instrucción en la dirección de memoria 2 (305). El bus de control envía una señal de lectura para iniciar este proceso. El valor 3 se almacena en el registro de instrucciones y 05 en el registro de direcciones. El PC se incrementa a 3 mediante la ALU.

2. **Decodificación (Decode):** La instrucción 3 se decodifica como “almacenar acumulador en dirección” y el registro de direcciones indica la ubicación donde guardar los datos (05). La unidad de control usa el bus de control para coordinar esto.

3. **Ejecución (Execute):** Se abre la dirección 5 mediante el bus de direcciones, y el bus de control envía las señales adecuadas para enviar el contenido del acumulador por el bus de datos y almacenarlo en la dirección 5 (sobrescribiendo los datos actuales).

#### Cuarto ciclo (Click step)

1. **Búsqueda (Fetch):** El PC está actualmente en 3, por lo que se recupera la instrucción en la dirección de memoria 3 (000). El bus de control envía una señal de lectura para iniciar este proceso. El valor 0 se almacena en el registro de instrucciones y 00 en el registro de direcciones. El PC se incrementa a 4 mediante la ALU.

2. **Decodificación (Decode):** La instrucción 0 se decodifica como “detener”. La unidad de control utiliza el bus de control para señalar esta operación.

3. **Ejecución (Execute):** El ordenador detiene todas las operaciones y finaliza el programa.
