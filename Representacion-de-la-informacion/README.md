<h1 align="center">Representación de la información</h1>
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://frontal.ies-sabadell.cat/eso-moodle/"><img src="https://img.shields.io/badge/Moodle-Cursos-%230081C3" alt="Enllaç a Moodle"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>

</div>

La **representación de la información** es un concepto clave en la informática, que permite transformar datos de cualquier tipo (como texto, imágenes, audio y video) en formatos que puedan ser procesados y almacenados por sistemas digitales. El **código binario** es la base de esta representación en los dispositivos electrónicos y computadoras, ya que utiliza combinaciones de dos valores, 0 y 1, para codificar y manipular cualquier tipo de información. Esta transformación a formato binario es fundamental para que la tecnología digital pueda operar de manera precisa, eficiente y fiable, facilitando la comunicación y el procesamiento de datos en el mundo actual.

### Contenido:

- [1. Introducción al código binario](#1-introducción-al-código-binario)
  - [1.1. ¿Qué es el código binario?](#11-qué-es-el-código-binario)
  - [1.2. Historia y aplicaciones del código binario](#12-historia-y-aplicaciones-del-código-binario)
  - [1.3. Importancia del código binario en la informática y la electrónica](#13-importancia-del-código-binario-en-la-informática-y-la-electrónica)

- [2. Conceptos básicos del sistema binario](#2-conceptos-básicos-del-sistema-binario)
  - [2.1. Sistema de numeración binario vs. sistema decimal](#21-sistema-de-numeración-binario-vs-sistema-decimal)
  - [2.2. Dígitos binarios: el uso de 0 y 1](#22-dígitos-binarios-el-uso-de-0-y-1)
  - [2.3. Bits y bytes: unidad de medida en binario](#23-bits-y-bytes-unidad-de-medida-en-binario)

- [3. Conversión de números decimales a binario](#3-conversión-de-números-decimales-a-binario)
  - [3.1. Método de divisiones sucesivas](#31-método-de-divisiones-sucesivas)
  - [3.2. Ejemplo paso a paso de conversión de decimal a binario](#32-ejemplo-paso-a-paso-de-conversión-de-decimal-a-binario)
  - [3.3. Ejercicios prácticos para convertir números decimales a binario](#33-ejercicios-prácticos-para-convertir-números-decimales-a-binario)

- [4. Conversión de binario a decimal](#4-conversión-de-binario-a-decimal)
  - [4.1. Método de multiplicación y suma de potencias de 2](#41-método-de-multiplicación-y-suma-de-potencias-de-2)
  - [4.2. Ejemplo paso a paso de conversión de binario a decimal](#42-ejemplo-paso-a-paso-de-conversión-de-binario-a-decimal)
  - [4.3. Ejercicios prácticos para convertir números binarios a decimal](#43-ejercicios-prácticos-para-convertir-números-binarios-a-decimal)

- [5. Representación binaria de caracteres: Código ASCII](#5-representación-binaria-de-caracteres-código-ascii)
  - [5.1. Introducción al código ASCII](#51-introducción-al-código-ascii)
  - [5.2. Conversión de letras y caracteres a código binario](#52-conversión-de-letras-y-caracteres-a-código-binario)
  - [5.3. Ejemplos de codificación binaria de palabras](#53-ejemplos-de-codificación-binaria-de-palabras)

- [6. Operaciones básicas en binario](#6-operaciones-básicas-en-binario)
  - [6.1. Suma binaria](#61-suma-binaria)
  - [6.2. Resta binaria](#62-resta-binaria)
  - [6.3. Multiplicación y división en binario (introducción básica)](#63-multiplicación-y-división-en-binario-introducción-básica)

- [7. Aplicaciones del código binario](#7-aplicaciones-del-código-binario)
  - [7.1. Uso en almacenamiento de datos](#71-uso-en-almacenamiento-de-datos)
  - [7.2. Comunicación digital](#72-comunicación-digital)
  - [7.3. Representación de imágenes, sonidos y otros tipos de datos](#73-representación-de-imágenes-sonidos-y-otros-tipos-de-datos)

- [8. Ejercicios y prácticas recomendadas](#8-ejercicios-y-prácticas-recomendadas)
  - [8.1. Convertir números decimales a binario y viceversa](#81-convertir-números-decimales-a-binario-y-viceversa)
  - [8.2. Realizar operaciones básicas en binario](#82-realizar-operaciones-básicas-en-binario)
  - [8.3. Codificación de palabras con código ASCII en binario](#83-codificación-de-palabras-con-código-ascii-en-binario)

<br>

## 1. Introducción al código binario
	
La digitalización, al convertir la información en una secuencia de datos en código binario, permite que una misma herramienta (el ordenador) pueda trabajar con información de muy diversa índole (imagen, sonido, texto, etc.). Para los usuarios, la información de un documento digital puede ser visual o sonora; para el ordenador, todos los archivos son datos codificados de igual forma. Nos encontramos ante la paradoja de que, para poder tratar información multimedia de diferente naturaleza y con lenguajes comunicativos diferentes, previamente debemos codificar la información con un lenguaje común a todos los medias: el lenguaje binario.

```📖 El bit es la mínima expresión de la información```

  ## 1.1. ¿Qué es el código binario?
  El **código binario** es un sistema numérico en el que solo se emplean dos dígitos: **0** y **1**. Cada posición en un número binario representa una potencia de 2, de forma similar a cómo el sistema decimal utiliza potencias de 10. Por ejemplo, el número binario **101** en el sistema decimal se lee como:

  ```🔢1 × 2² + 0 × 2¹ + 1 × 2⁰ = 4 + 0 + 1 = 5```

  ## 1.2. Historia y aplicaciones del código binario
  La historia del código binario y su aplicación se remonta varios siglos atrás:

  - **Siglo XVII:** El matemático y filósofo alemán **Gottfried Wilhelm Leibniz** desarrolló una teoría sobre el sistema binario, observando una relación entre los valores de "0" y "1" y la filosofía del Yin y Yang en la cultura china. Su trabajo fue uno de los primeros en documentar el uso de un sistema binario para representar información.

  - **Siglo XIX:** El matemático británico **George Boole** creó la álgebra **booleana**, un sistema de lógica que permite realizar operaciones con valores binarios. Su álgebra constituye la base de la lógica de los circuitos digitales, que sigue siendo utilizada en los procesadores y dispositivos electrónicos actuales.

  - **Siglo XX:** Durante el desarrollo de los primeros computadores en los años 30 y 40, el código binario se consolidó como el lenguaje fundamental de la computación. Ordenadores tempranos como el **ENIAC** y el **UNIVAC** utilizaban interruptores que representaban los valores binarios 1 y 0 para realizar cálculos.

  ## 1.3. Importancia del código binario en la informática y la electrónica

  El código binario es fundamental en el funcionamiento de la informática y la electrónica moderna por varias razones:

  - **Simplicidad en el diseño de circuitos:** Debido a que el código binario solo utiliza dos estados (0 y 1), los circuitos electrónicos pueden construirse de manera simple y eficiente, con conmutadores que representan estos valores. Esto permite que los dispositivos realicen operaciones lógicas y aritméticas con una estructura de hardware relativamente sencilla.

  - **Fiabilidad en la transmisión y almacenamiento de datos:** La información en binario es menos susceptible a errores durante la transmisión, ya que la detección de estados (0 o 1) es más clara que en sistemas de varios niveles. Esto también facilita el almacenamiento de datos en formatos binarios duraderos y seguros.

  - **Base para todas las operaciones de procesamiento:** Los procesadores de las computadoras y otros dispositivos digitales realizan cálculos y operaciones lógicas en formato binario. Todo el software, desde sistemas operativos hasta aplicaciones, funciona gracias a que los datos y las instrucciones pueden representarse y manipularse en código binario.

## 2. Conceptos básicos del sistema binario
El sistema binario es la base de la informática y los sistemas digitales, ya que permite representar y procesar información de manera eficiente. Al comprender cómo funciona el sistema binario y su relación con el sistema decimal, podemos entender cómo se almacenan y transmiten datos en los dispositivos electrónicos.

  ## 2.1. Sistema de numeración binario vs. sistema decimal
  El **sistema binario** y el **sistema decimal** son dos sistemas de numeración que utilizan diferentes bases:

  - **Sistema decimal (base 10):** Es el sistema que usamos habitualmente y se compone de diez dígitos (0, 1, 2, 3, 4, 5, 6, 7, 8 y 9). Cada posición en un número decimal representa una potencia de 10, lo que significa que el valor total se calcula multiplicando cada dígito por una potencia de 10 en función de su posición.

  ```🔢3 × 10² + 4 × 10¹ + 5 × 10⁰ = 300 + 40 + 5 = 345```

  - **Sistema binario (base 2):** Este sistema utiliza solo dos dígitos, 0 y 1. Cada posición en un número binario representa una potencia de 2. Este sistema es ideal para la computación porque los circuitos electrónicos solo necesitan dos estados (por ejemplo, encendido y apagado) para procesar los datos.

  ```🔢1 × 2⁸ + 0 × 2⁷ + 1 × 2⁶ + 0 × 2⁵ + 1 × 2⁴ + 1 × 2³ + 0 × 2² + 0 × 2¹ + 1 × 2⁰ = 256 + 0 + 64 + 0 + 16 + 8 + 0 + 0 + 1 = 345``` 

  ## 2.2. Dígitos binarios: el uso de 0 y 1
  En el sistema binario, cada **dígito** se denomina **bit** y puede tener solo dos valores: **0** o **1**. Esta simplicidad hace que los dispositivos electrónicos puedan procesar datos mediante señales eléctricas, donde un valor alto (por ejemplo, encendido) puede representar el 1 y un valor bajo (apagado) puede representar el 0. La combinación de múltiples bits permite representar cantidades más grandes y complejas.

  Cada bit en una secuencia binaria representa una potencia de 2, de derecha a izquierda:

  - El primer bit representa 2⁰ (1),
  - El segundo bit representa 2¹ (2),
  - El tercero representa 2² (4), y así sucesivamente.

  Esto permite que una combinación de bits pueda representar cualquier número decimal.

  ## 2.3. Bits y bytes: unidad de medida en binario
  Un **bit** es la unidad más pequeña de información en el sistema binario. Sin embargo, trabajar con bits individuales sería poco práctico en la mayoría de las aplicaciones. Por esta razón, los bits se agrupan en conjuntos de 8 llamados **bytes**.

  - **Byte:** Un byte contiene 8 bits y puede representar 256 valores distintos (de 00000000 a 11111111 en binario, que es de 0 a 255 en decimal). Los bytes son la unidad de medida estándar en almacenamiento y procesamiento de datos.

  - **Kilobyte (KB), Megabyte (MB), Gigabyte (GB), etc.:** A medida que se requiere más espacio para almacenar datos, los bytes se agrupan en unidades mayores. Un kilobyte (KB) equivale a 1,024 bytes, un megabyte (MB) es 1,024 kilobytes, y así sucesivamente. Este sistema jerárquico permite medir grandes cantidades de información de manera ordenada y comprensible.

## 3. Conversión de números decimales a binario
La conversión del sistema decimal a binario se realiza mediante el **método de divisiones sucesivas**, que descompone el número decimal en una secuencia de 0s y 1s.

  ## 3.1. Método de divisiones sucesivas
  El **método de divisiones sucesivas** es una técnica simple para convertir un número decimal en binario. Consiste en dividir el número decimal sucesivamente entre 2 y anotar el residuo de cada división. Los restos obtenidos representan los dígitos binarios, y el número binario se forma leyendo los restos de abajo hacia arriba (del último al primero).

  **Pasos del método:**

  1. Divide el número decimal entre 2.
  2. Anota el residuo (0 o 1), que se convierte en el dígito binario.
  3. Divide el cociente obtenido nuevamente entre 2.
  4. Repite los pasos hasta que el cociente sea 0.
  5. El número binario se forma con los restos leídos de abajo hacia arriba.

  ## 3.2. Ejemplo paso a paso de conversión de decimal a binario
  Convertimos el número decimal **345** a binario siguiendo el método de divisiones sucesivas: 
  
  1. 345 ÷ 2 = 172, residuo 1
  2. 172 ÷ 2 = 86, residuo 0
  3. 86 ÷ 2 = 43, residuo 0
  4. 43 ÷ 2 = 21, residuo 1
  5. 21 ÷ 2 = 10, residuo 1
  6. 10 ÷ 2 = 5, residuo 0
  7. 5 ÷ 2 = 2, residuo 1
  8. 2 ÷ 2 = 1, residuo 0
  9. 1 ÷ 2 = 0, residuo 1

  Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```🔢345₁₀ = 101011001₂```
 
  Así que el número decimal **345** es **101011001** en binario.

  ## 3.3. Ejercicios prácticos para convertir números decimales a binario
  Apliquemos el método de divisiones sucesivas en diferentes números decimales, con tal de obtener el número binario: 

  **Convertir el número decimal 27 a binario**
  
  1. 27 ÷ 2 = 13, residuo 1
  2. 13 ÷ 2 = 6, residuo 1
  3. 6 ÷ 2 = 3, residuo 0
  4. 3 ÷ 2 = 1, residuo 1
  5. 1 ÷ 2 = 0, residuo 1

  Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```🔢27₁₀ = 11011₂```

  Así que el número decimal **27** es **11011** en binario.

  **Convertir el número decimal 58 a binario**
  
  1. 58 ÷ 2 = 29, residuo 0
  2. 29 ÷ 2 = 14, residuo 1
  3. 14 ÷ 2 = 7, residuo 0
  4. 7 ÷ 2 = 3, residuo 1
  5. 3 ÷ 2 = 1, residuo 1
  6. 1 ÷ 2 = 0, residuo 1

  Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```🔢58₁₀ = 111010₂```

  Así que el número decimal **58** es **111010** en binario.

  **Convertir el número decimal 100 a binario**
  
  1. 100 ÷ 2 = 50, residuo 0
  2. 50 ÷ 2 = 25, residuo 0
  3. 25 ÷ 2 = 12, residuo 1
  4. 12 ÷ 2 = 6, residuo 0
  5. 6 ÷ 2 = 3, residuo 0
  6. 3 ÷ 2 = 1, residuo 1
  7. 1 ÷ 2 = 0, residuo 1

  Luego, leemos los residuos de abajo hacia arriba, obteniendo:

  ```🔢100₁₀ = 1100100₂```

  Así que el número decimal **100** es **1100100** en binario.

# 4. Conversión de binario a decimal
La conversión del sistema binario a decimal se realiza mediante el **método de multiplicación y suma de potencias de 2**.

  ## 4.1. Método de multiplicación y suma de potencias de 2
  El **método de multiplicación y suma de potencias de 2** permite convertir un número binario en su equivalente decimal. Consiste en descomponer el número binario, multiplicando cada dígito (0 o 1) por una potencia de 2 basada en su posición de derecha a izquierda, empezando desde el exponente 0.

  **Pasos del método:**

  1. Escribe el número binario y anota la potencia de 2 correspondiente a cada posición de derecha a izquierda.
  2. Multiplica cada dígito binario (0 o 1) por su potencia de 2 correspondiente.
  3. Suma los resultados de cada multiplicación para obtener el valor decimal.

  ## 4.2. Ejemplo paso a paso de conversión de binario a decimal
  Convertimos el número binario **1011** a decimal siguiendo el método de multiplicación y suma de potencias de 2:
  
  1. Escribimos el número binario y asignamos una potencia de 2 a cada posición:
  
  ```🔢1 × 2³ + 0 × 2² + 1 × 2¹ + 1 × 2⁰``
 
  2. Multiplicamos cada dígito binario por su correspondiente potencia de 2:
  
  ```🔢1 × 8 + 0 × 4 + 1 × 2 + 1 × 1 = 8 + 0 + 2 + 1``

  3. Sumamos los resultados para obtener el valor decimal:
  
  ```🔢8 + 0 + 2 + 1 = 11``

  Por lo tanto, el número binario **1011** es igual a **11** en decimal.

  ## 4.3. Ejercicios prácticos para convertir números binarios a decimal
  Apliquemos el método de multiplicación y suma de potencias de 2 en diferentes números binarios, con tal de obtener el número decimal: 

  **Convertir el número binario 11011 a decimal**

  1. 1 × 2³ + 1 × 2² + 0 × 2¹ + 1 × 2⁰
  2. 1 × 8 + 1 × 4 + 0 × 2 + 1 × 1 = 8 + 4 + 0 + 1
  3. 8 + 4 + 0 + 1 = 13

  Así que el número binario **11011** es **13** en decimal.

  **Convertir el número binario 10010 a decimal**

  1. 1 × 2⁴ + 0 × 2³ + 0 × 2² + 1 × 2¹ + 0 × 2⁰
  2. 1 × 16 + 0 × 8 + 0 × 4 + 1 × 2 + 0 × 1 = 16 + 0 + 0 + 2 + 0
  3. 16 + 0 + 0 + 2 + 0 = 18

  Así que el número binario **10010** es **18** en decimal.

  **Convertir el número binario 111001 a decimal**

  1. 1 × 2⁵ + 1 × 2⁴ + 1 × 2³ + 0 × 2² + 0 × 2¹ + 1 × 2⁰
  2. 1 × 32 + 1 × 16 + 1 × 8 + 0 × 4 + 0 × 2 + 1 × 1 = 32 + 16 + 8 + 0 + 0 + 1
  3. 32 + 16 + 8 + 0 + 0 + 1 = 57

  Así que el número binario **111001** es **57** en decimal.

# 5. Representación binaria de caracteres: Código ASCII
El sistema binario no solo se utiliza para representar números, sino también para codificar caracteres y símbolos a través de códigos estándar como el **Código ASCII**. Este sistema permite que las computadoras representen letras, números y otros caracteres mediante secuencias de 0s y 1s.

  ## 5.1. Introducción al código ASCII
  El **Código ASCII (American Standard Code for Information Interchange)** es un estándar de codificación de caracteres desarrollado en los años 60 para representar letras, números y símbolos comunes. Cada carácter en ASCII se representa mediante un número decimal que va de 0 a 127, y estos números se convierten en una secuencia de 7 bits en binario. Con ASCII extendido, se llega a representar hasta 256 caracteres, utilizando 8 bits (1 byte) por carácter.

  ASCII facilita la interoperabilidad entre diferentes sistemas y dispositivos, ya que se ha convertido en un estándar universal para representar texto en binario. Cada letra, número o símbolo tiene un código único; por ejemplo:

  - La letra "A" tiene el valor decimal 65, que en binario es **01000001**.
  - La letra "a" tiene el valor decimal 97, que en binario es **01100001**.

  <div style="text-align: center;">
  <img src="https://elcodigoascii.com.ar/codigo-americano-estandar-intercambio-informacion/codigo-ascii.png" alt="XT color" width="1199" height="669"/>
  <p><em>Figura 1: El código ASCII. Fuente: <a href="https://elcodigoascii.com.ar/">El codigo ASCII</a></em></p>
  </div>

  ## 5.2. Conversión de letras y caracteres a código binario
  Para convertir letras y caracteres al sistema binario usando el código ASCII, basta con seguir estos pasos:

  1. Identificar el valor decimal de la letra o símbolo según la tabla ASCII.
  2. Convertir ese valor decimal en binario.

  ## 5.3. Ejemplos de codificación binaria de palabras
  Veamos algunos ejemplos de cómo se puede codificar una palabra en binario utilizando el código ASCII. Tomemos la palabra **"Hi"** como ejemplo:
  1. **H**:
    - Valor decimal: 72
    - Binario: **01001000**
  
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

# 6. Operaciones básicas en binario
Las operaciones en binario son fundamentales en el procesamiento de datos y en los cálculos realizados por las computadoras. Estas operaciones incluyen la suma, resta, multiplicación y división, que se llevan a cabo utilizando las reglas propias del sistema binario, donde solo intervienen los dígitos 0 y 1.

  ## 6.1. Suma binaria
  La **suma binaria^** sigue reglas similares a la suma en el sistema decimal, pero debido a que solo tiene dos dígitos (0 y 1), las combinaciones de suma son más simples:

  - 0 + 0 = 0
  - 0 + 1 = 1
  - 1 + 0 = 1
  - 1 + 1 = 10 (equivale a 0 y lleva 1 al siguiente dígito, similar a cómo llevamos 1 en el sistema decimal)

  **Ejemplo**: Sumar **1011** y **1101**

  | Acarreo |   1   | 1 | 1 |   |
  |---------|-------|---|---|---|
  | Número 1|   1   | 0 | 1 | 1 |
  | Número 2|   1   | 1 | 0 | 1 |
  | Resultado | 1 | 1 | 0 | 0 | 0 |
