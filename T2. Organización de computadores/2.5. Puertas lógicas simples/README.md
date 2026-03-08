<h1 align="center">2.5. Puertas lógicas simples

<div align="center">

</div>

## Contenido:

- [2.5.1. Defina los operadores booleanos: AND, OR, NOT, NAND, NOR y XOR](#251-defina-los-operadores-booleanos-and-or-not-nand-nor-y-xor)
- [2.5.2. Elabore tablas de verdad usando los operadores anteriores](#252-elabore-tablas-de-verdad-usando-los-operadores-anteriores)
- [2.5.3. Elabore un diagrama lógico usando puertas AND, OR, NOT, NAND, NOR y XOR](#253-elabore-un-diagrama-lógico-usando-puertas-and-or-not-nand-nor-y-xor)

---

<br>

## 2.5.1. Defina los operadores booleanos: AND, OR, NOT, NAND, NOR y XOR

### La historia de las puertas lógicas
A mediados del siglo XIX, un matemático británico llamado George Boole desarrolló un sistema algebraico conocido como “álgebra booleana”. Este proporcionó un marco matemático para representar enunciados y operaciones lógicas que sentaron las bases de la lógica digital moderna.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2030.%20George%20Boole.jpg" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 30: George Boole. Fuente: Wikipedia</em></p>
  </div>
  
George Boole, el matemático británico que desarrolló el álgebra booleana, sentando las bases de la lógica digital y la informática moderna.

A principios del siglo XX, un matemático e ingeniero eléctrico estadounidense llamado Claude Shannon fue la primera persona en reconocer el potencial del álgebra booleana para el diseño de circuitos eléctricos. Demostró cómo el diseño de circuitos de relés eléctricos podía optimizarse utilizando álgebra booleana, y posteriormente el desarrollo de la tecnología de semiconductores impulsó aún más la evolución de las puertas lógicas.

El transistor fue inventado en 1947 en los Laboratorios Bell, lo que hizo posible construir puertas lógicas compactas y eficientes. Entre las décadas de 1960 y 1970, los circuitos integrados comenzaron a incorporar múltiples transistores en un solo chip, lo que llevó al desarrollo de los microprocesadores. Las puertas lógicas son los bloques fundamentales de los sistemas digitales modernos, desde la calculadora básica hasta los superordenadores avanzados.

### Puertas básicas

Las puertas lógicas son **componentes fundamentales en la electrónica digital**, esenciales para construir diversos tipos de circuitos dentro de los ordenadores y otros dispositivos digitales.
Los tipos básicos de puertas lógicas incluyen las puertas **AND**, **OR** y **NOT**, cada una de las cuales realiza una función lógica específica. Estas puertas reciben una o más entradas binarias y producen una salida binaria según la operación lógica que llevan a cabo.

Para comprender y verificar el comportamiento de estas puertas, utilizamos tablas de verdad, que enumeran de manera sistemática todas las combinaciones posibles de entradas y sus salidas correspondientes, proporcionando una representación clara de la función de la puerta. Además, cada puerta tiene una representación en álgebra booleana que permite simplificar expresiones lógicas complejas.

Las puertas lógicas están formadas por transistores, que actúan como interruptores electrónicos, permitiendo o bloqueando el flujo de corriente eléctrica. En un transistor, el cable de control (o “gate”) regula la corriente entre los dos electrodos, conocidos como “source” (fuente) y “drain” (drenador). Cuando se aplica un voltaje a la puerta, se permite que la corriente fluya desde la fuente hacia el drenador, lo que permite que el transistor cambie de estado y realice operaciones lógicas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2031.%20Circuito%20l%C3%B3gico.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 31: Puerta Buffer apagada. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

  Una puerta Buffer que muestra el funcionamiento interno de la puerta: cuando el cable de control está apagado, no puede fluir electricidad entre los electrodos.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2032.%20Circuito%20l%C3%B3gico.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 32: Puerta Buffer encendida. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cuando la electricidad circula por el cable de control, el transistor permite el flujo de electricidad entre los electrodos.

Arriba se muestra una puerta Buffer simple, donde podemos considerar el cable de control como la entrada y el electrodo drain como la salida. Si la entrada está encendida, la salida está encendida; y si la entrada está apagada, la salida está apagada. Podemos mostrar esto usando una tabla de verdad:

| Input A | Output X |
|---------|----------|
|    1    |     1    |
|    0    |     0    |

#### Puerta AND

El diagrama de debajo muestra una puerta AND implementada con transistores. La puerta tiene dos entradas y una salida. Si solo una de las entradas está encendida, uno de los transistores sin entrada detendría el paso de la corriente. Solo cuando ambas entradas están en alto (1) los transistores permiten que la corriente fluya, lo que da como resultado una salida alta (1).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2033.%20Puerta%20AND.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 33: Puerta AND. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

**Regla de entrada y salida:** La puerta AND produce 1 solo si ambas entradas son 1.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     0     |
|    0    |    1     |     0     |
|    1    |    0     |     0     |
|    1    |    1     |     1     |

```Boolean algebra: X = A · B```

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2034.%20Esquema%20a%20nivel%20de%20transistores%20de%20una%20puerta%20AND.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 34: Esquema a nivel de transistores de una puerta AND. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### Puerta OR

El diagrama de la izquierda muestra una puerta OR implementada con transistores. La puerta tiene dos entradas —A y B— y una salida. Cuando cualquiera de las entradas A o B está en alto (1), el transistor correspondiente se activa, permitiendo que la corriente fluya a través del circuito y dando como resultado una salida alta (1). Cuando ambas entradas están en bajo (0), ninguno de los transistores conduce y la salida permanece en bajo (0).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2035.%20Puerta%20OR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 35: Puerta OR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

```Boolean algebra: X = A + B```

**Regla de entrada y salida:** La puerta OR produce 1 si al menos una de las entradas es 1.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     0     |
|    0    |    1     |     1     |
|    1    |    0     |     1     |
|    1    |    1     |     1     |

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2036.%20Esquema%20a%20nivel%20de%20transistores%20de%20una%20puerta%20OR.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 36: Esquema a nivel de transistores de una puerta OR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### Puerta NOT

El diagrama siguiente ilustra una puerta NOT (inversor) utilizando un transistor. En esta configuración, la línea de entrada está conectada a la puerta (gate) del transistor, la línea de salida está conectada a la fuente (source) y el drenador (drain) está conectado a tierra.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2037.%20Puerta%20NOT.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 37: Puerta NOT. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2038.%20Esquema%20a%20nivel%20de%20transistores%20de%20una%20puerta%20NOT.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 38: Esquema a nivel de transistores de una puerta NOT. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cuando la entrada está en alto (1), el transistor se enciende, permitiendo que la corriente fluya desde la fuente hacia el drenador, conectando efectivamente la salida a tierra y produciendo un voltaje bajo en la salida (0). Cuando la entrada está en bajo (0), el transistor se apaga, impidiendo que la corriente fluya hacia tierra. En este estado, la salida adopta un voltaje alto (1).

**Regla de entrada y salida:** La puerta NOT produce el valor opuesto al de la entrada. 

| Input A | Output X |
|---------|-----------|
|    0    |     1     |
|    1    |     0     |

```Boolean algebra: X = ¬A```

### Puertas derivadas (complejas)

Las siguientes puertas —**NAND**, **NOR**, **XOR** y **XNOR**— son ejemplos de puertas derivadas. Las puertas derivadas son combinaciones de las puertas básicas y proporcionan funciones lógicas más complejas. Para mostrarlas, subiremos un nivel de abstracción y, en lugar de examinar el esquema a nivel de transistores, veremos cómo se combinan las puertas básicas para crearlas.

#### Puerta NAND (NOT AND)

Una puerta NAND se construye con una puerta AND seguida de una puerta NOT. Debido a esto, produce la salida opuesta a una puerta AND. Si ambas entradas están en alto (1), la salida es baja (0). En todos los demás casos, la salida es alta (1).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2039.%20Puerta%20NAND.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 39: Puerta AND y NOT. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cómo se construye una puerta NAND: una puerta AND seguida de una puerta NOT.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2040.%20Puerta%20NAND.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 40: Puerta NAND. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

**Regla de entrada y salida:** La puerta NAND produce 1 a menos que ambas entradas sean 1.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     1     |
|    0    |    1     |     1     |
|    1    |    0     |     1     |
|    1    |    1     |     0     |

```Boolean algebra: X = ¬(A · B)```

#### Puerta NOR (NOT OR)

Una puerta NOR produce la salida opuesta a una puerta OR, ya que está construida utilizando una puerta OR seguida de una puerta NOT. Esto significa que solo cuando ambas entradas están en bajo (0) la salida es alta (1). En todos los demás casos, la salida es baja (0).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2041.%20Puerta%20NOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 41: Puerta OR y NOT. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cómo se construye una puerta NOR: una puerta OR seguida de una puerta NOT.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2042.%20Puerta%20NOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 42: Puerta NOR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

**Regla de entrada y salida:** La puerta NOR produce 1 solo si ambas entradas son 0.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     1     |
|    0    |    1     |     0     |
|    1    |    0     |     0     |
|    1    |    1     |     0     |

```Boolean algebra: X = ¬(A + B)```

#### Puerta XOR (OR exclusivo)

La puerta XOR (OR exclusivo) se diferencia de la puerta OR en un aspecto clave: su salida es verdadera solo cuando las entradas son diferentes. Esto significa que la puerta XOR produce verdadero cuando exactamente una de las entradas es verdadera, pero falso cuando ambas entradas son iguales. Por ejemplo, si ambas entradas están en alto (1), la salida de la puerta XOR es baja (0). Esto es distinto a la puerta OR, que en ese caso produciría una salida alta (1).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2043.%20Puerta%20XOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 43: Puerta exclusive OR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cómo se construye una puerta XOR.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2044.%20Puerta%20XOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 44: Puerta XOR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

**Regla de entrada y salida:** La puerta XOR produce 1 si las entradas son diferentes.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     0     |
|    0    |    1     |     1     |
|    1    |    0     |     1     |
|    1    |    1     |     0     |

```Boolean algebra: X = A ⊕ B```

#### Puerta XNOR (exclusive NOT OR)

La puerta XNOR se construye utilizando una puerta XOR seguida de una puerta NOT. Esto significa que su salida es la opuesta a la de una puerta XOR, produciendo un valor alto (1) únicamente cuando ambas entradas son iguales (ya sea ambas altas o ambas bajas).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2045.%20Puerta%20XNOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 45: Puerta XNOR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Cómo se construye una puerta XNOR: una puerta XOR seguida de una puerta NOT.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2046.%20Puerta%20XNOR.png" alt="Imagen" width="250" height="auto"/>
    <p><em>Figura 46: Puerta XNOR. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

**Regla de entrada y salida:** La puerta XNOR produce 1 si las entradas son iguales.

| Input A | Input B | Output X |
|---------|----------|-----------|
|    0    |    0     |     1     |
|    0    |    1     |     0     |
|    1    |    0     |     0     |
|    1    |    1     |     1     |

```Boolean algebra: X = ¬(A ⊕ B)```

<br>

## 2.5.2. Elabore tablas de verdad usando los operadores anteriores

### Tablas de verdad para predecir la salida de circuitos lógicos simples

El siguiente diagrama muestra un circuito lógico, donde varios compuertas lógicas están conectadas entre sí. En este escenario, debes ser capaz de trabajar con circuitos que tengan hasta tres entradas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2047.%20Diagrama%20de%20circuito%20l%C3%B3gico%201%20.png" alt="Imagen" width="550" height="auto"/>
    <p><em>Figura 47: Diagrama de circuito lógico 1. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Al crear una tabla de verdad, primero introduce las tres entradas y sus posibles estados; en este caso, A, B y C. Como hay tres entradas, puedes calcular el número de filas necesarias usando 2<sup>n</sup>, donde *n* representa el número de entradas.

En este ejemplo:

2<sup>3</sup> = 8

- Rellena la columna de la derecha alternando entre 0 y 1.
- Rellena la columna central alternando, cada dos filas, entre 0 y 1.
- Rellena la columna de la izquierda alternando, cada cuatro filas, entre 0 y 1.

Seguir este patrón te dará todos los posibles estados de entrada.

| A | B | C |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 0 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |
| 1 | 1 | 1 |

Una vez hecho esto, añadimos los valores intermedios para facilitar recordar el estado en cada etapa del circuito. En este ejemplo, tenemos tres valores intermedios: P, Q y R. Finalmente, añadimos la columna de salida, X.

| A | B | C | P | Q | R | X |
|---|---|---|---|---|---|---|
| 0 | 0 | 0 |   |   |   |   |
| 0 | 0 | 1 |   |   |   |   |
| 0 | 1 | 0 |   |   |   |   |
| 0 | 1 | 1 |   |   |   |   |
| 1 | 0 | 0 |   |   |   |   |
| 1 | 0 | 1 |   |   |   |   |
| 1 | 1 | 0 |   |   |   |   |
| 1 | 1 | 1 |   |   |   |   |

Ahora, comenzando por los valores intermedios, recorre el circuito lógico paso a paso.

| A | B | C | P (A AND B) | Q (B NOR C) | R (P OR Q) | X (C XOR R) |
|---|---|---|--------------|-------------|------------|-------------|
| 0 | 0 | 0 |      0       |      1      |     1      |      1      |
| 0 | 0 | 1 |      0       |      0      |     0      |      1      |
| 0 | 1 | 0 |      0       |      0      |     0      |      0      |
| 0 | 1 | 1 |      0       |      0      |     0      |      1      |
| 1 | 0 | 0 |      0       |      1      |     1      |      1      |
| 1 | 0 | 1 |      0       |      0      |     0      |      1      |
| 1 | 1 | 0 |      1       |      0      |     1      |      1      |
| 1 | 1 | 1 |      1       |      0      |     1      |      0      |

### Tablas de verdad para determinar las salidas a partir de las entradas de la descripción de un problema

**Descripción del problema:** *Una alarma para bebés que se activa cuando la alarma está encendida y el bebé está llorando o la habitación está demasiado fría.*

Con una descripción del problema, primero necesitamos identificar las entradas. Aquí tenemos tres: el interruptor de la alarma, el llanto del bebé y la temperatura de la habitación, que podemos representar como A, B y C y configurar nuestra tabla de verdad.

Sabemos que la alarma se activa si el dispositivo está encendido Y el bebé está llorando O la habitación está demasiado fría. A partir de aquí, podemos identificar las puertas lógicas en la descripción. Podemos deducir que el dispositivo debe estar encendido antes de que la alarma pueda activarse, por lo que, si el interruptor está apagado, todas las salidas serían 0. Si el dispositivo está encendido, al menos una de las otras dos entradas debe estar activa para que la alarma se dispare. Tenemos un valor intermedio (el bebé está llorando O la habitación está fría), representado con P.

| A (encendida) | B (llorando) | C (fría) | P (B or C) | X (A and P) |
|------------|------------|----------|------------|-------------|
| 0          | 0          | 0        | 0          | 0           |
| 0          | 0          | 1        | 1          | 0           |
| 0          | 1          | 0        | 1          | 0           |
| 0          | 1          | 1        | 1          | 0           |
| 1          | 0          | 0        | 0          | 0           |
| 1          | 0          | 1        | 1          | 1           |
| 1          | 1          | 0        | 1          | 1           |
| 1          | 1          | 1        | 1          | 1           |

### Expresiones lógicas

Podemos representar circuitos lógicos utilizando álgebra booleana. Si usamos de nuevo el escenario de la alarma para bebés, podemos representarlo así:

```X = A · (B + C)```

En álgebra booleana, los paréntesis se utilizan a menudo para indicar qué operaciones deben realizarse primero. Sin embargo, existe un orden estándar de las operaciones, similar a PEMDAS (o BODMAS) en matemáticas. Si no hay paréntesis presentes, se debe seguir esta secuencia:

- NOT
- AND (incluyendo NAND)
- OR (incluyendo NOR y XOR)

Esto garantiza que las operaciones se ejecuten en el orden correcto para obtener resultados precisos.

### Mapas de Karnaugh y simplificación algebraica

Los mapas de Karnaugh (K-maps) son una herramienta que ayuda a simplificar expresiones booleanas, facilitando la creación de circuitos digitales más simples y eficientes. En lugar de utilizar métodos algebraicos complicados, los mapas de Karnaugh permiten agrupar visualmente términos de una tabla de verdad, lo que hace más rápido encontrar una expresión simplificada.

Este proceso es útil porque reduce el número de puertas lógicas necesarias en un circuito, ahorrando tiempo, espacio, costes y consumo de energía.

#### Dos entradas

Este mapa de Karnaugh de dos entradas se utiliza para expresiones con dos variables. En este mapa, la variable A se coloca en el lateral y la variable B en la parte superior. Sin embargo, el orden de las variables no importa: B podría colocarse en el lateral y A en la parte superior. Ambos estados posibles (0 y 1) para cada variable se muestran en el mapa, representando todas las combinaciones de sus valores.

##### Expresión: A + B

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2048.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

Dividimos la expresión en el operador OR (O) y nos centramos primero en el término que implica a A. Rellenamos el mapa de Karnaugh donde A es 1, lo que, en este caso, corresponde a toda la fila inferior. En esta etapa, ignoramos B y solo completamos las celdas en las que A = 1.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2049.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

Hacemos lo mismo para la segunda parte de la expresión: B. 

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2050.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

Este mapa de Karnaugh completado ahora muestra la expresión A + B.

Este es otro ejemplo de un mapa completado para la expresión ¬A + B:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2051.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

<br>

##### Expresión: A · B + A · ¬B

Esta es una expresión más complicada, pero que aún solo tiene dos entradas. Utilizando esta expresión, el circuito tendría el siguiente aspecto:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2052.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

La estructura del mapa en forma de tabla sigue siendo la misma:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2053.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

Volvemos a dividir la expresión en el símbolo OR (O), centrándonos inicialmente en A · B. En este caso, introducimos un 1 únicamente en una celda, donde tanto A como B son 1.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2054.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

A continuación, nos centramos en la segunda parte de la expresión A · ¬B. En este caso, introducimos un 1 en la celda donde A es 1 y B es 0.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2055.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

El mapa de Karnaugh ya está completo y muestra que el valor de B no tiene ningún impacto en el resultado, lo que nos permite simplificar la expresión a simplemente A. Si creamos el circuito utilizando esta expresión simplificada, podemos ver que el circuito es significativamente más eficiente, mientras que sigue realizando la misma función.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2056.%20K-map.png" alt="Imagen" width="450" height="auto"/>
  </div>

#### Tres entradas

##### Expresión: ¬A · B · C + A · ¬B · C + A · B · C
Con tres entradas, utilizamos un mapa de Karnaugh similar, pero en este caso colocamos dos de las entradas en la parte superior. Los dígitos de la parte superior pueden parecer fuera de orden en comparación con el conteo binario estándar (00, 01, 10, 11). En su lugar, siguen la convención del código Gray (véase la Sección A1.2.2 para más información), en la que solo cambia un dígito cada vez. Es importante configurar el mapa de esta manera para garantizar una agrupación y una simplificación correctas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2057.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

Ahora seguimos pasos similares a los del mapa de Karnaugh de dos entradas. Separamos la expresión por el operador OR (O) y nos centramos en el primer término: ¬A · B · C. En este paso, completamos el mapa de Karnaugh introduciendo un 1 en las celdas donde A es 0, B es 1 y C es 1.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2058.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

Seguido de: A · ¬B · C

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2059.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

Y finalmente: A · B · C

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2060.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

#### Agrupación de los 1 y simplificación de la expresión

Aunque no se indicó explícitamente antes, es posible que hayas observado los recuadros dibujados alrededor de los grupos de 1 en los mapas de Karnaugh. Estos recuadros ayudan a simplificar la expresión booleana, pero hay algunas reglas importantes que deben seguirse al agrupar los 1:

- **Los grupos deben contener potencias de 2:** Se pueden agrupar uno, dos, cuatro, ocho o dieciséis 1.
- **Los grupos deben ser rectangulares o cuadrados:** Cada grupo debe formar un rectángulo o un cuadrado.
- **Los grupos no pueden ser diagonales:** Los 1 adyacentes solo se pueden agrupar horizontal o verticalmente, no en diagonal.
- **Los grupos deben ser lo más grandes posible:** Siempre se debe intentar formar los grupos más grandes para simplificar aún más la expresión.
- **Los grupos pueden solaparse:** Algunos 1 pueden incluirse en más de un grupo si esto ayuda a formar grupos más grandes.
- **Minimizar el número total de grupos:** El objetivo es utilizar el menor número de grupos posible para cubrir todos los 1.

Para determinar la expresión a partir de los grupos, analizamos cada grupo de celdas y nos fijamos en las variables. Si el valor de una variable se mantiene igual en todas las celdas del grupo, esa variable se conserva en la expresión simplificada. Sin embargo, si el valor de la variable cambia dentro del grupo, se elimina de la expresión.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2061.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

El primer grupo está completamente a lo largo de la fila inferior, lo que significa que C se mantiene constante (C = 1), por lo que la conservamos en la expresión. A cambia de 0 a 1 entre las celdas del grupo, así que descartamos A. B permanece en 1 en ambas celdas, por lo que conservamos B.

Por tanto, la primera parte de nuestra expresión final es: B · C

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2062.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

El segundo grupo, al igual que el primero, se encuentra a lo largo de la fila inferior, lo que significa que C se mantiene en 1, ya que no cambia dentro del grupo. En este caso, A permanece en 1 en ambas celdas, mientras que B cambia de 0 a 1. Dado que B cambia, descartamos B de esta parte de la expresión. Como resultado, conservamos A y C, lo que nos da la segunda parte de nuestra expresión: A · C

A continuación, combinamos estas expresiones mediante el operador OR (O), obteniendo la expresión final: B · C + A · C

> [!CAUTION]
> Al configurar tu mapa de Karnaugh para tres entradas, asegúrate de utilizar código Gray en los encabezados y no el binario estándar. El código Gray garantiza que solo cambie un bit entre celdas adyacentes, lo que ayuda a agrupar los 1 y a simplificar la expresión de forma más eficaz.

#### Conexión por los bordes en los mapas de Karnaugh

Aquí se muestra el mapa de Karnaugh para la expresión: ¬B + A · B · C

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2063.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

Para agrupar estos 1, puedes asumir que esta es la respuesta:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2064.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

Sin embargo, los mapas de Karnaugh se consideran tridimensionales, y los grupos pueden formarse de izquierda a derecha y de arriba abajo (aunque con tres entradas solo es posible de izquierda a derecha). En este ejemplo, es posible construir un grupo más grande combinando los dos grupos de los extremos, formando un grupo cuadrado de cuatro 1.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2065.%20K-map.png" alt="Imagen" width="650" height="auto"/>
  </div>

<br>

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2066.%20K-map.png" alt="Imagen" width="550" height="auto"/>
  </div>

Mapa de Karnaugh dibujado sobre un toro y en un plano – las celdas marcadas con puntos son adyacentes.

Utilizando estos grupos, podemos formar la expresión simplificada: A · C + ¬B

<br>

## 2.5.3. Elabore un diagrama lógico usando puertas AND, OR, NOT, NAND, NOR y XOR

### Diseño de circuitos digitales a partir de expresiones de álgebra booleana

Al comprender los principios del álgebra booleana, podemos simplificar expresiones lógicas complejas y traducirlas en diagramas de circuitos. Este proceso, que va desde la notación matemática abstracta hasta el diseño de circuitos, es esencial para crear sistemas digitales eficientes y fiables. Comenzaremos creando el circuito digital a partir de la expresión que se muestra a continuación:

```Y = (A · B) + (¬A · B)```

1. Comienza con dos entradas: A y B.

2. Trabaja sobre el primer paréntesis introduciendo una puerta AND (Y) y conectando tanto A como B a ella.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2067.%20K-map.png" alt="Imagen" width="370" height="auto"/>
  </div>

3. Trabaja sobre el segundo paréntesis, conectando A a una puerta NOT (NO) y B a otra puerta NOT.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2068.%20K-map.png" alt="Imagen" width="370" height="auto"/>
  </div>

4. Conecta ambas salidas a una puerta AND (Y).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2069.%20K-map.png" alt="Imagen" width="550" height="auto"/>
  </div>

5. Ahora trabaja fuera de los paréntesis e introduce una puerta OR (O) para unirlas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2070.%20K-map.png" alt="Imagen" width="550" height="auto"/>
  </div>
