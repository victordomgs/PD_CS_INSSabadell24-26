<h1 align="center">Fundamentos de sistemas 
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
<a href="https://www.linkedin.com/in/v%C3%ADctor-garc%C3%ADa-saiz-/"><img src="https://img.shields.io/badge/LinkedIn-Perfil-%230077B5" alt="Perfil de LinkedIn"/></a>
</a>



</div>

### Contenido:

- [1. Estructura y esquema funcional de un ordenador](#1-estructura-y-esquema-funcional-de-un-ordenador)
  - [1.1. Datos, información y conocimiento](#11-datos-información-y-conocimiento)
    - [1.1.1. Tipología de datos](#111-tipología-de-datos)
    - [1.1.2. Tratamiento de la información](#112-tratamiento-de-la-información)
  - [1.2. Los ordenadores](#12-los-ordenadores)
    - [1.2.1. Hardware](#121-hardware)
      - [1.2.1.1. La CPU (Unidad central de procesamiento)](#1211-la-cpu-unidad-central-de-procesamiento)
      - [1.2.1.2. Memoria](#1212-memoria)
      - [1.2.1.3. Dispositivos de entrada y salida (I/O)](#1213-dispositivos-de-entrada-y-salida-io)
    - [1.2.2. Software](#122-software)
      - [1.2.2.1. Tipos de software](#1221-tipos-de-software)
        - [1.2.2.1.1. Software de sistema](#12211-software-de-sistema)
        - [1.2.2.1.2. Software de aplicación](#12212-software-de-aplicación)
        - [1.2.2.1.3. Software de desarrollo](#12213-software-de-desarrollo)
      - [1.2.2.2. Funciones principales del software de sistema](#1222-funciones-principales-del-software-de-sistema)
        - [1.2.2.2.1. Gestión de hardware](#12221-gestión-de-hardware)
        - [1.2.2.2.2. Gestión de archivos y procesos](#12222-gestión-de-archivos-y-procesos)
      - [1.2.2.3. Licencias de software y tipos de distribución](#1223-licencias-de-software-y-tipos-de-distribución)
        - [1.2.2.3.1. Software propietario vs. software libre](#12231-software-propietario-vs-software-libre)
        - [1.2.2.3.2. Código abierto (open-source) y sus implicaciones](#12232-código-abierto-open-source-y-sus-implicaciones)
        - [1.2.2.3.3. Licencias comunes: GPL, MIT, Creative Commons](#12233-licencias-comunes-gpl-mit-creative-commons)

<br>

## 1. Estructura i esquema funcional de un ordenador

Los sistemas informáticos nos permiten procesar **datos** automáticamente, cosa que no podríamos hacer sin ellos. Las personas aprendemos de lo que nos rodea y, mediante la **información**, podemos mejorar o cambiar nuestros **conocimientos**.

Los ordenadores están formados por diferentes partes que ayudan a procesar la información y también permiten que las personas interactúen con estos.  

En resumen, la informática es una herramienta para trabajar la información, y el ordenador es el medio mediante el cual se hace posible esta interacción entre las personas y la información. 

  ## 1.1. Datos, información y conocimiento
  Los **datos** son hechos o cifras que no tienen significado por ellos mismos hasta que no se procesan y organizan. 

  💡Ej: ```"23", "50", "29", "8"```

  Son solo números sin contexto. Podrían representar muchas cosas diferentes (edades, temperaturas, horas del día, etc.), pero por sí solas no nos dan ningún tipo de información útil.

  La **información** se genera cuando los datos son organizados o procesados para darles significado. Cuando los datos se relacionan entre si o se presentan en su contexto, comienzan a tener un significado y una utilidad. 
  
  💡Ej: ```"Las temperaturas durante la semana pasada fueron de 23°C el lunes, 50°C el martes, 29°C el miércoles i 8°C el jueves."```

  Ahora los datos tienen un contexto y pueden entenderse mejor: son temperaturas que han estado registradas durante la semana. 

  El **conocimiento** es la comprensión profunda y la aplicación de la información. Se produce cuando una persona interpreta la información, la compara con otros hechos o experiencias, y la aplica para entender el mundo o tomar decisiones.

  💡Ej: ```"Si las temperaturas son tan extremas como se registraron (50 °C martes y 8 °C jueves), probablemente se trata de un cambio climático extremo en la zona, el cual puede afectar las cosechas y la salud pública. Es importante tomar medidas para proteger las personas y las infraestructuras ante estos cambios de temperatura."```

  Aquí, el conocimiento no solo es la comprensión de los datos (temperaturas extremas), sino también la capacidad de hacer conexiones entre estos datos, entender sus implicaciones y aplicar este conocimiento a un contexto práctico.


  ## 1.1.1. Tipología de datos
  Siguiendo con los **datos**, no todos los datos son del mismo tipo. Dependiendo del tipo de dato, podremos hacer diferentes cosas con ellos, como calcular, analizar u organizar.

  **Datos numéricos**
  
  Son aquellos datos que contienen **números** y con las cuales se pueden realizar operaciones matemáticas (sumar, restar, multiplicar, etc.).

  💡Ej:
    
  | **Tipos de datos**    | **Ejemplo**                   |
  |----------------------|-------------------------------|
  | **Cantidades**       | 25, 100, 3.14                 |
  | **Medidas**          | 1,75 metres, 20°C             |
  | **Fechas y horas**    | 2023, 15:30                   |

  **Datos alfabéticos**
  
  Son datos que solo contienen **letras**. Estos datos no se pueden utilizar para hacer operaciones matemáticas, pero son útiles para identificar o describir cosas.

  💡Ej:
  
  | **Tipos de datos**       | **Ejemplo**                     |
  |-------------------------|---------------------------------|
  | **Nombre**                 | "Maria", "Joan"                 |
  | **Ciudad**              | "Barcelona", "Madrid"           |
  | **Cuentas de usuarios**    | "usuari", "admin"            |

  **Datos alfanuméricos**
  
  Son una combinación de **números** y **letras**. Este tipo de datos se usa mucho en direcciones, códigos o contraseñas. A pesar de que incluyen números, no se pueden hacer operaciones matemáticas con ellos, puesto que su finalidad es identificar o codificar información, no realizar cálculos.

💡Ej:

  | **Tipos de datos**       | **Ejemplo**                     |
  |-------------------------|---------------------------------|
  | **Direcciones postales**     | "c/ Muntaner, 100, 3r"          |
  | **Codigos de producto**  | "A12B34"                        |
  | **Contraseñas**        | "Passw0rd123"                   |


  **Datos temporales**
  
  Este tipo de datos se relacionan con el **tiempo** y se utilizan para representar fechas, horas o duraciones. Pueden ser tanto numéricos como alfanuméricos (si incluyen letras, por ejemplo, nombres de meses).

  💡Ej:

  | **Tipos de datos** | **Ejemplo**                     |
  |-------------------|---------------------------------|
  | **Fecha**          | "12/04/2023", "2024-03-15"      |
  | **Hora**          | "14:30", "23:59"                |
  | **Duración**        | "3 hores", "2 dies"             |

  **Datos booleanos**
  
  Los datos booleanos representan solo dos opciones posibles: **cierto** o **falso**. Son muy útiles en informática para hacer preguntas de verdad o falsedad, como en los tests y condiciones.

  💡Ej:

  | **Tipos de datos** | **Ejemplo**                     |
  |-------------------|---------------------------------|
  | **Cierto/Falso**     | "True" (cierto), "False" (falso)   |
  | **Si/No**         | "Si", "No"                      |

  **Datos categóricos**
  
  Estos datos pertenecen a categorías o grupos. No tienen un orden numérico, pero nos permiten agrupar los elementos en diferentes clases. Son útiles para clasificar la información.

  💡Ej:

  | **Tipos de datos**         | **Ejemplo**                     |
  |---------------------------|---------------------------------|
  | **Colores**                | "Rojo", "Azul", "Verde"       |
  | **Tipo de vehículos**     | "Coche", "Moto", "Bicicleta"    |
  | **Estados de un producto**  | "Nuevo", "Usado", "Reparado"        |

  
  **Resumen de la clasificación**

  | **Tipos de datos**  | **Ejemplo**                           | **Características**                            |
  |--------------------|---------------------------------------|-------------------------------------------------|
  | **Numéricos**     | 25, 100, 3.14                         | Permite hacer operaciones matemáticas              |
  | **Alfabéticos**   | "Maria", "Joan"                       | Son letras, no se pueden hacer cálculos            |
  | **Alfanuméricos** | "A12B34", "c/ Muntaner, 100, 3r"      | Combinan letras y números, no operan         |
  | **Temporales**      | "2023-03-12", "14:30"                 | Relacionados con fechas y horas                 |
  | **Booleanos**      | True, False, Sí, No                   | Solo dos opciones: cierto o falso                 |
  | **Categóricos**   | "Rojo", "Coche", "Nuevo"             | Agrupaciones o categorías sin orden          |


  ## 1.1.2. Tratamiento de la información

  La manera en que se trata la información ha evolucionado significativamente a lo largo del tiempo, adaptándose a los avances tecnológicos y a las necesidades de cada momento histórico.

  El **tratamiento de la información** se puede definir como el conjunto de operaciones aplicadas sobre los datos para transformarlos en información útil. Este proceso siempre requiere tres elementos esenciales para funcionar de manera eficiente:

  - **Emisor:** El elemento que genera la información, como una persona hablando o un texto escrito.
  - **Canal:** El medio a través del cual se transmite la información, como el aire para la voz o una red de telecomunicaciones para datos.
  - **Receptor:** El elemento que recibe la información, como un lector o un dispositivo.

  ### Fases del tratamiento de la información

  El proceso de tratamiento de la información se divide en tres operaciones principales, como se muestra a continuación:

  | **Operaciones** | **Funciones**                                                  |
  |-----------------|-----------------------------------------------------------------|
  | **Entrada**     | Recogida y almacenamiento de datos                              |
  | **Proceso**     | Manipulación de datos mediante cálculos aritméticos o operaciones lógicas |
  | **Salida**      | Recogida y distribución de los resultados                       |

  Cada fase tiene características importantes:

  - **Entrada:** Recogida de información para ser tratada, como leer libros o obtener datos digitales. Este proceso incluye la selección, verificación y almacenamiento de la información en un soporte adecuado.
  - **Proceso:** Manipulación de la información, ya sea mediante cálculos matemáticos o operaciones lógicas.
  - **Salida:** Comunicación de los resultados, que pueden ser presentados externamente o utilizados en otros procesos.

  ### Evolución histórica del tratamiento de la información

  El tratamiento de la información ha ido evolucionando a lo largo de la historia, desde procesos manuales hasta los actuales procesos automáticos.

  <div style="text-align: center;">
  <img src="https://parceladigital.com/subidos/1611221350x_xt_color.jpg" alt="XT color" width="320" height="180"/>
  <p><em>Figura 1: Imagen de un IBM PC XT. Fuente: <a href="https://parceladigital.com/articulo/el-ordenador-personal-y-su-historia">Parceladigital</a></em></p>
  </div>

  - **Manual:** El tratamiento se realiza completamente a mano, como rellenar documentos.
  - **Mecánico:** Utiliza máquinas con asistencia humana, como las máquinas de escribir o calculadoras.
  - **Automático:** Desde los años 40, con la aparición de los ordenadores y otros dispositivos automáticos, las máquinas pueden procesar información de manera independiente.

  Estas etapas han culminado en la aparición de la **informática**, que se refiere específicamente al tratamiento automático de la información, impulsando el uso de **ordenadores** y otras tecnologías modernas.

  ## 1.2. Los ordenadores

  La física, la química, la meteorología y otras ciencias explican y justifican hechos de nuestro entorno. De manera similar, la **informática** es una ciencia que estudia el tratamiento de la información, lo cual es posible gracias al uso de diversas herramientas, entre ellas, el ordenador.

  ### La informática

  La informática surgió con el objetivo de ayudar a las personas a realizar tareas repetitivas y rutinarias, especialmente en cálculos y gestiones, donde la repetición es común. La idea central es que una máquina puede hacer estas tareas con mayor rapidez y precisión, aunque siempre bajo control humano.

  > 📖 El término informática apareció en Francia en el año 1962 con la denominación "informatique", resultado de la contracción de las palabras: INFORmation autoMATIQUE.

  ### Tareas principales de la informática

  Las tareas que engloba la informática incluyen:

  - **Desarrollo y mejora de nuevas máquinas**, como los ordenadores y otros elementos relacionados.
  - **Desarrollo y mejora de métodos de trabajo automáticos**, basados en el sistema operativo.
  - **Creación de aplicaciones informáticas**, conocidas como programas o paquetes informáticos.

  El término sistema informático se refiere al conjunto de elementos necesarios para llevar a cabo y utilizar aplicaciones informáticas. Esto incluye el hardware, el software y los elementos humanos.

  ### Componentes de un sistema informático

  Un sistema informático se compone de tres elementos interrelacionados:

  - **Parte física (hardware):** Todos los componentes que se pueden ver y tocar, como los monitores, impresoras, ratones, etc.
  - **Parte lógica (software):** Todos los elementos intangibles, como los programas, sistemas operativos y aplicaciones.
  - **Parte humana:** Las personas son el elemento más importante en un sistema informático, ya que sin ellas no existirían ni el hardware ni el software.

  ### Programas y aplicaciones informáticas

  El conjunto de acciones que se ordenan y ejecutan en un ordenador se conoce como programa. En general, un programa es un conjunto de instrucciones que se siguen en un orden determinado para resolver un problema específico.

  Una **aplicación informática** es un conjunto de uno o más programas diseñados para realizar una tarea específica en un sistema informático.

  ### Componentes fundamentales de un ordenador

  El ordenador está formado por dos elementos principales:

  - **Hardware:** Incluye todos los componentes físicos que se pueden ver y tocar, como el monitor, el teclado, la CPU, etc.
  - **Software:** Se refiere a los componentes no físicos, como los programas, las aplicaciones y los sistemas operativos.

  También destacan otros elementos como:

  - **Usuario y programador:** El usuario es la persona que utiliza el ordenador, mientras que el programador es quien escribe los programas en lenguajes de programación para que el ordenador pueda ejecutarlos.
  - **Datos e información:** Los datos son los hechos o materiales originales no procesados, mientras que la información es el resultado de los datos ya procesados.
  - **Documentación:** Conjunto de instrucciones o manuales que explican al usuario cómo utilizar el ordenador y los programas informáticos.

  <div style="text-align: center;">
    <img src="https://ioc.xtec.cat/materials/FP/Recursos/fp_asx_m05_/web/fp_asx_m05_htmlindex/WebContent/u1/media/ic10m5u1_02.png" alt="Estructura de un ordenador" width="640" height="auto"/>
    <p><em>Figura 2: Estructura funcional de un ordenador. Fuente: IOC XTEC</em></p>
  </div>

  ## 1.2.1. Hardware

  ## 1.2.1.1. La CPU (Unidad Central de Procesamiento)

  La **CPU (Unidad Central de Procesamiento)** es el componente fundamental de un ordenador encargado de procesar los datos y ejecutar las instrucciones de un programa. También se conoce como el **procesador** o "cerebro" del ordenador, ya que controla todas las operaciones que se realizan dentro del sistema.

  **Partes de la CPU**

  La CPU está formada por varias partes que trabajan conjuntamente para ejecutar las instrucciones que recibe. Las partes principales de la CPU son:

  - La **Unidad de Control (CU)** es responsable de dirigir y coordinar todas las operaciones del ordenador.
  - La **Unidad Aritmética y Lógica (ALU)** realiza operaciones matemáticas y lógicas. La ALU trabaja con los datos que le suministra la Unidad de Control y devuelve los resultados a otros componentes de la CPU, como los registros o la memoria.
  - Los **registros** son pequeñas áreas de memoria de alta velocidad dentro de la CPU que se utilizan para almacenar datos temporales durante la ejecución de instrucciones. Son mucho más rápidos que la memoria RAM y proporcionan acceso inmediato a los datos que se procesan.

  **Funcionamiento básico de la CPU**

  | **Fase**             | **Descripción**                                                                                                                                                     |
  |----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | **Fetch (Búsqueda)**       | - La CPU localiza la siguiente instrucción en la memoria (RAM).<br>- Usa el contador de programa (PC), que contiene la dirección de la próxima instrucción.<br>- La instrucción se transfiere desde la memoria a un registro en la CPU, como el registro de instrucciones. |
  | **Decode (Decodificación)** | - Una vez la instrucción está en el registro de instrucciones, la Unidad de Control la decodifica.<br>- La Unidad de Control determina las acciones necesarias, incluidos operadores y datos a manipular. |
  | **Execute (Ejecución)**    | - La instrucción se procesa. Si requiere operaciones aritméticas o lógicas, la Unidad de Control envía la orden a la ALU.<br>- Los resultados se almacenan en un registro o se devuelven a la memoria.<br>- El contador de programa se incrementa para pasar a la siguiente   instrucción, repitiendo el ciclo. |

  <div style="text-align: center;">
  <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%203.%20Fundamentos%20de%20sistemas.png" alt="Descripción de la imagen" width="337" height="295"/>
  <p><em>Figura 3: Ciclo de instrucciones de la máquina. Fuente: <a>Creación propia</a></em></p>
  </div>
  
  ## 1.2.1.2. Memoria

  La memoria es un componente fundamental de un ordenador, responsable de almacenar datos e instrucciones que la CPU necesita para ejecutar operaciones. Permite que el procesador tenga acceso rápido a la información requerida.

  > 📖 **Un byte** es una unidad básica de almacenamiento de datos en informática, compuesta por 8 bits, donde cada bit puede tener un valor de 0 o 1. Los bytes son fundamentales en la memoria, ya que permiten almacenar y representar una amplia variedad de datos, desde caracteres individuales (como letras y números) hasta instrucciones de programas y valores numéricos. La memoria de un sistema se organiza en bytes, lo que facilita el acceso y manipulación de datos de manera estructurada y eficiente. La capacidad de un dispositivo para almacenar información se mide en bytes y sus múltiplos (como kilobytes, megabytes y gigabytes), lo cual es crucial para determinar el rendimiento y la capacidad de almacenamiento de computadoras y otros dispositivos electrónicos.

  | Unidad         | Equivalencia en Bytes                     |
  |----------------|------------------------------------------|
  | 1 Kilobyte (KB)| 1,024 Bytes                              |
  | 1 Megabyte (MB)| 1,024 Kilobytes = 1,048,576 Bytes        |
  | 1 Gigabyte (GB)| 1,024 Megabytes = 1,073,741,824 Bytes    |
  | 1 Terabyte (TB)| 1,024 Gigabytes = 1,099,511,627,776 Bytes|
  | 1 Petabyte (PB)| 1,024 Terabytes = 1,125,899,906,842,624 Bytes |
  | 1 Exabyte (EB) | 1,024 Petabytes = 1,152,921,504,606,846,976 Bytes |



  **Memoria principal (RAM)**

  La **RAM (Random Access Memory)** es la memoria principal del ordenador, donde se cargan los datos e instrucciones que la CPU necesita mientras ejecuta un programa. La RAM es volátil, es decir, la información almacenada se pierde cuando el ordenador se apaga.

  - **Función:** Almacena temporalmente datos y programas en uso por la CPU.
  - **Velocidad:** Es rápida, permite acceder a cualquier parte de la memoria de inmediato.
  - **Capacidad:** Normalmente tiene capacidad limitada en comparación con el almacenamiento secundario.

  En un sistema computacional, la Unidad de Control (CU, por sus siglas en inglés) y la Unidad Aritmético-Lógica (ALU) colaboran en el procesamiento de datos, y el flujo de información entre la memoria y estas unidades se gestiona de la siguiente manera:

  <div style="text-align: center;">
  <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%204.%20Fundamentos%20de%20sistemas.png" alt="Descripción de la imagen" width="787" height="267"/>
  <p><em>Figura 4: Estructura de la memoria de acceso aleatoria. Fuente: <a>Creación propia</a></em></p>
  </div>

  1. La CU envía la dirección de memoria al Registro de Direcciones de Memoria. El registro de direcciones de memoria es un componente que almacena la dirección específica en la memoria donde se desea leer o escribir datos.
  3. El contenido de esa dirección se transfiere al Registro de Datos de Memoria. El registro de datos de memoria contiene los datos que se transfieren entre la CPU y la memoria.
  4. Si se requiere procesamiento, el dato en el Registro de Datos de Memoria se envía a la ALU.
  5. La ALU realiza la operación y el resultado puede ser devuelto a la memoria o a un registro.

  **Memoria ROM**

  La **ROM (Read-Only Memory)** es un tipo de memoria no volátil que conserva los datos incluso cuando el ordenador se apaga. La información almacenada en la ROM generalmente es escrita por el fabricante y no se puede modificar fácilmente.

  - **Función:** Contiene instrucciones permanentes necesarias para arrancar el sistema, como la BIOS (Basic Input/Output System).
  - **Característica:** Solo permite la lectura de datos; no se puede escribir en la ROM durante el funcionamiento normal del ordenador.
  - **Ejemplos de uso:** BIOS, firmware de dispositivos.

  **Memoria caché**

  La **memoria caché** es una memoria de pequeña capacidad pero muy rápida que se encuentra entre la CPU y la RAM. Su función principal es acelerar el acceso de la CPU a los datos que se usan con más frecuencia.

  - **Función:** Almacena copias de datos de la memoria principal que se utilizan frecuentemente para reducir el tiempo de acceso.
  - **Tipos:** Existen diferentes niveles de memoria caché (L1, L2, L3), siendo L1 la más rápida pero de menor capacidad, y L3 la más lenta pero de mayor capacidad.
  - **Impacto en el rendimiento:** Reduce los cuellos de botella entre la velocidad de la CPU y la memoria principal.

  **Almacenamiento secundario**

  El **almacenamiento secundario** es el espacio donde se guardan datos de manera permanente. A diferencia de la RAM, no es volátil, por lo que la información se mantiene almacenada aunque el ordenador se apague.

  - **Ejemplos:** Discos duros (HDD), unidades de estado sólido (SSD), discos ópticos (CD/DVD) y unidades USB.
  - **Función:** Almacena de manera permanente datos, programas, archivos y el sistema operativo.
  - **Característica:** Tiene mucha más capacidad que la memoria RAM, pero es más lenta.

  ## 1.2.1.3. Dispositivos de entrada y salida (I/O)

  Los dispositivos de entrada y salida, también conocidos como **periféricos**, son elementos externos que permiten la interacción entre el ordenador y el usuario o con otros sistemas. Estos dispositivos sirven para introducir datos al ordenador, mostrar resultados o permitir la comunicación entre sistemas.

  **Dispositivos de entrada**

  Los **dispositivos de entrada** permiten al usuario o a otros sistemas introducir datos o instrucciones en el ordenador, transformando datos físicos en señales digitales que el ordenador puede procesar.

  - **Teclado:** Dispositivo de entrada más común. Permite introducir caracteres, números y símbolos.
  - **Ratón:** Dispositivo apuntador que permite controlar el cursor en la pantalla.
  - **Escáner:** Convierte documentos físicos, como imágenes o texto, en formato digital.
  - **Micrófono:** Permite la entrada de audio, convirtiendo las ondas sonoras en señales digitales.
  - **Cámara web:** Captura imágenes y vídeo en tiempo real para aplicaciones como videoconferencias.

  **Dispositivos de salida**

  Los **dispositivos de salida** permiten al ordenador enviar información al usuario o a otros sistemas, mostrando o transmitiendo el resultado de las operaciones procesadas.

  - **Monitor:** Muestra visualmente la información generada por el ordenador, como resultados, imágenes y vídeos.
  - **Impresora:** Convierte la información digital en una copia física, como documentos o imágenes impresas.
  - **Altavoces:** Convierten las señales digitales en sonido.
  - **Proyector:** Dispositivo de salida que proyecta imágenes o vídeos en una pantalla grande, usado en presentaciones.

  **Dispositivos de entrada y salida**

  Los **dispositivos de entrada y salida** pueden realizar tanto la función de entrada como de salida de datos, permitiendo la comunicación bidireccional.

  - **Unidades de disco:** Permiten la lectura y escritura de datos en soportes de memoria como discos duros, discos ópticos o SSD.
  - **Pantallas táctiles:** Combinan la función de monitor (salida) con la de entrada, permitiendo interactuar mediante toques o gestos.
  - **Memorias USB:** Dispositivos de almacenamiento externos que permiten leer y escribir datos.
  - **Módems:** Dispositivos de comunicación que permiten enviar y recibir datos a través de una red, generalmente conectada a internet.

  <div style="text-align: center;">
    <img src="https://ioc.xtec.cat/materials/FP/Recursos/fp_asx_m05_/web/fp_asx_m05_htmlindex/WebContent/u1/media/ic10m5u1_04.png" alt="Esquema de los elementos de las unidades funcionales de un ordenador" width="640" height="auto"/>
    <p><em>Figura 5: Esquema de los elementos de las unidades funcionales de un ordenador. Fuente: IOC XTEC</em></p>
  </div>

  <div style="text-align: center;">
    <img src="https://ioc.xtec.cat/materials/FP/Recursos/fp_asx_m05_/web/fp_asx_m05_htmlindex/WebContent/u1/media/ic10m5u1_05.png" alt="Interconexión de las unidades funcionales de un ordenador mediante buses" width="640" height="auto"/>
    <p><em>Figura 6: Interconexión de las unidades funcionales de un ordenador mediante buses. Font: IOC XTEC</em></p>
  </div>

  <div style="text-align: center;">
    <img src="https://ioc.xtec.cat/materials/FP/Recursos/fp_asx_m05_/web/fp_asx_m05_htmlindex/WebContent/u1/media/ic10m5u1_06.png" alt="Estructura funcional de los ordenadores" width="640" height="auto"/>
    <p><em>Figura 7: Estructura funcional de los ordenadores. Fuente: IOC XTEC</em></p>
  </div>

  ## 1.2.2. Software
  El software es el conjunto de programas e instrucciones que permiten a los ordenadores y dispositivos electrónicos realizar tareas específicas. A diferencia del hardware (componentes físicos de un ordenador), el software es intangible y se compone de código creado mediante lenguajes de programación. Hay diferentes tipos de software que cumplen funciones específicas dentro de un sistema informático.

  ## 1.2.2.1. Tipos de software
  ## 1.2.2.1.1. Software de sistema
  El **software de sistema** es el conjunto de programas que gestiona y controla los recursos del hardware y proporciona una base para que otros programas funcionen. Es esencial para el funcionamiento del ordenador y ayuda a gestionar los recursos internos.

  💡Ej: Sistemas operativos: como Windows, macOS o Linux. Son algunos de los software de sistemas más importante. También se incluyen los controladores de dispositivos, que permiten que el sistema operativo se comunique con componentes específicos del hardware, como impresoras, tarjetas gráficas y otros periféricos.

  <div style="text-align: center;">
  <img src="https://www.adslzone.net/app/uploads-adslzone.net/2017/06/windows-linux-1200x675.jpg" alt="Windows y Linux" width="320" height="180"/>
  <p><em>Figura 8: Software de sistema. Fuente: <a href="https://www.adslzone.net/2017/06/01/es-realmente-mas-seguro-linux-que-windows/">ADSLZone</a></em></p>
  </div>

  ## 1.2.2.1.2. Software de aplicación
  El **software de aplicación** está diseñado para realizar tareas específicas que faciliten las actividades de los usuarios. Este tipo de software permite a los usuarios interactuar con el ordenador y realizar tareas cotidianas.

  💡Ej: Procesadores de texto (Microsoft Word), navegadores web (Google Chrome, Firefox), aplicaciones multimedia (Spotify, VLC) y software de edición gráfica (Photoshop, GIMP).

  <div style="text-align: center;">
  <img src="https://image.jimcdn.com/app/cms/image/transf/dimension=533x1024:format=jpg/path/s63841b80d293924d/image/i023016192ee81785/version/1539160109/image.jpg" alt="Software de aplicaciones" width="420" height="180"/>
  <p><em>Figura 9: Software de aplicaciones. Fuente: <a href="https://informatica4esog2.jimdofree.com/software/software-de-aplicaci%C3%B3n/">Jimdo</a></em></p>
  </div>
  
  ## 1.2.2.1.3. Software de desarrollo
  El **software de desarrollo** incluye herramientas utilizadas por los programadores para crear otros programas. Este tipo de software ayuda a los desarrolladores a escribir, probar y mantener el código de las aplicaciones.

  💡Ej: Entornos de desarrollo integrado (IDE) como Visual Studio, Eclipse y herramientas de gestión de bases de datos como MySQL y PostgreSQL.

  <div style="text-align: center;">
  <img src="https://acpdelsureste.com/wp-content/uploads/Tecno.png" alt="Componentes de la tecnología" width="420" height="180"/>
  <p><em>Figura 10: Software de desarrollo. Fuente: <a href="https://acpdelsureste.com/desarrollo-de-software-2/">ACP del Sureste</a></em></p>
  </div>

  ## 1.2.2.2. Funciones principales del software de sistema
  El software de sistema desempeña varias funciones esenciales para el correcto funcionamiento del ordenador, asegurando que el hardware y el software de aplicación trabajen en armonía.

  ## 1.2.2.2.1. Gestión de hardware
  La **gestión de hardware** permite que el software controle los recursos físicos del ordenador, como la CPU, la memoria y los dispositivos de entrada/salida. El software de sistema administra la distribución de estos recursos entre las aplicaciones que se están ejecutando para evitar conflictos y optimizar el rendimiento.

  💡Ej: Cuando abres varias aplicaciones a la vez, el sistema operativo gestiona cómo se utiliza la memoria para que cada programa funcione sin problemas.
  
  ## 1.2.2.2.2. Gestión de archivos y procesos
  La **gestión de archivos y procesos** es otra función del software de sistema. El sistema operativo organiza los archivos almacenados en el ordenador y permite que el usuario cree, modifique y elimine documentos. Además, gestiona los procesos, que son las tareas en ejecución en el ordenador.

  💡Ej: Al guardar un archivo en una carpeta específica, el sistema operativo organiza el archivo en el disco duro. También controla cuántos procesos (programas) están abiertos y se asegura de que cada uno tenga los recursos que necesita.
  
  ## 1.2.2.3. Licencias de software y tipos de distribución
  El software puede distribuirse bajo diferentes tipos de licencias, que definen cómo se puede utilizar, modificar y compartir.

  ## 1.2.2.3.1. Software propietario vs. software libre
  - **Software propietario:** Es un software cuyos derechos están controlados por una empresa o desarrollador. Solo puede utilizarse bajo ciertas condiciones, que suelen incluir la prohibición de modificar el código o distribuirlo libremente.

  💡Ej: Microsoft Office y Adobe Photoshop son software propietario; necesitan licencias para ser utilizados.
  
  - **Software libre:** Es un software que puede ser utilizado, modificado y distribuido libremente. El software libre se basa en la colaboración y permite a los usuarios adaptarlo a sus necesidades.

  💡Ej: LibreOffice y GIMP son software libre, accesible y modificable para todos los usuarios.

  ## 1.2.2.3.2. Código abierto (open-source) y sus implicaciones
  El **software de código abierto** permite que el código fuente esté disponible para cualquier persona que quiera verlo, modificarlo y distribuirlo. Este tipo de software fomenta la innovación, ya que otros programadores pueden mejorar el código.

  💡Ej: Linux es un sistema operativo de código abierto que cuenta con una gran comunidad que contribuye a su desarrollo. Esto lo convierte en un sistema flexible y adaptable.
  
  ## 1.2.2.3.3. Licencias comunes: GPL, MIT, Creative Commons
  Existen diferentes tipos de licencias que definen los términos bajo los cuales se puede utilizar y modificar el software.

  - **GPL (General Public License):** Esta licencia permite que el software sea libremente distribuido y modificado, siempre y cuando el nuevo software mantenga la misma licencia GPL.

  - **MIT License:** Es una licencia más permisiva que permite usar, modificar y distribuir el software, incluso en proyectos comerciales, con pocas restricciones.

  - **Creative Commons:** Aunque es más común en contenidos multimedia, también se usa en software. Ofrece diferentes niveles de permisos, desde uso libre hasta restricciones específicas.

  <div style="text-align: center;">
  <img src="https://s3.amazonaws.com/libapps/accounts/42282/images/licencias_cc.PNG" alt="Licencias Creative Commons" width="637" height="452"/>
  <p><em>Figura 11: Licencias Creative Commons. Fuente: <a href="https://biblioguias.uam.es/citar/creative_commons">S3 Universidad Autónoma de Madrid</a></em></p>
  </div>

  <br>
