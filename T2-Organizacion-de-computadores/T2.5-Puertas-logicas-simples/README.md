<h1 align="center">Puertas lógicas simples
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:
[1. Introducción a las puertas lógicas](#1-introducción-a-las-puertas-lógicas)  
  - [1.1. ¿Qué son las puertas lógicas?](#11-que-son-las-puertas-lógicas)
  - [1.2. Álgebra de Boole](#12-álgebra-de-boole)
  - [1.3. Teorema del álgebra de Boole](#13-teorema-del-álgebra-de-Boole)

[2. Representación de funciones lógicas](#2-representación-de-funciones-lógicas)  
  - [2.1. Definición de operadores booleanos](#21-definición-de-operadores-booleanos)  
  - [2.2. Tablas de verdad](#22-tablas-de-verdad)  

## 1. Introducción a las puertas lógicas

### 1.1. ¿Qué son las puertas lógicas?

Un **circuito lógico** es un sistema compuesto por señales de entrada, dispositivos electrónicos que procesan esas señales, y señales de salida que son el resultado de dichas operaciones. Estas señales son binarias, lo que significa que solo pueden tomar dos valores: $0$ (tensión baja) y $1$ (tensión alta). Una señal está activa cuando su valor es $1$.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%201.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="465" height="auto"/>
    <p><em>Figura 1: Circuito lógico. Fuente: UOC</em></p>
  </div>

Las señales de entrada y salida de un circuito lógico son funciones lógicas que representan operaciones realizadas por los dispositivos electrónicos del circuito. Estas operaciones se fundamentan en principios del **Álgebra de Boole**, y las señales binarias son manipuladas electrónicamente para producir un resultado lógico.

En este contexto, las **puertas lógicas** son los elementos básicos que realizan estas operaciones. Son dispositivos electrónicos que computan funciones lógicas específicas a partir de las señales de entrada.

> [!IMPORTANT]  
> Puesto que las señales sólo pueden tomar dos valores, diremos que uno es el contrario del otro. Así pues, podemos afirmar que cuando una señal no vale $1$, entonces seguro que vale $0$, y viceversa.

Tomamos un circuito que tenga sólo una señal de entrada (que llamamos $x$), un dispositivo electrónico y una señal de salida (que llamamos $z$).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%202.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="361" height="auto"/>
    <p><em>Figura 2: Circuito lógico con una entrada. Fuente: UOC</em></p>
  </div>

Dado que tanto $x$ como $z$ sólo pueden valer $0$ ó $1$, sólo existen cuatro dispositivos electrónicos diferentes que pueden interconectar $x$ y $z$:
- Un dispositivo que haga que la salida $z$ valga siempre $0$ (este dispositivo consistiría en conectar la salida con una fuente de tensión de $0$ voltios).
- Un dispositivo que haga que la salida valga siempre lo mismo que la entrada $x$ (este dispositivo consistiría en conectar directamente la salida con la entrada).
- Un dispositivo que haga que la salida valga siempre lo contrario de lo que vale la entrada (este dispositivo consistiría en un inversor del nivel de tensión).
- Un dispositivo que haga que la salida valga siempre $1$ (este dispositivo consistiría en conectar la salida directamente con la tensión de alimentación).

En otras palabras, podemos decir que sólo hay cuatro funciones lógicas que tengan una sola variable de entrada, tal como se muestra en la figura 3:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%203.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="476" height="auto"/>
    <p><em>Figura 3: Funciones lógicas sobre el circuito lógico de la Figura 2. Fuente: UOC</em></p>
  </div>

Tomamos ahora un circuito que tenga dos señales de entrada (que llamamos $x$ e $y$), un dispositivo electrónico y una señal de salida (que llamamos $z$).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%204.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="297" height="auto"/>
    <p><em>Figura 4: Circuito lógico con dos entradas. Fuente: UOC</em></p>
  </div>

En este caso, existen dieciséis dispositivos electrónicos diferentes que puedan interconectar las entradas con la salida, que corresponden a las funciones lógicas que se muestran en la figura 5.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%205.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="473" height="auto"/>
    <p><em>Figura 5: Funciones lógicas sobre el circuito lógico de la Figura 4. Fuente: UOC</em></p>
  </div>

Así pues, si tenemos en cuenta los circuitos con una o dos entradas, podemos llegar a diseñar hasta $4 + 16 = 20$ dispositivos electrónicos diferentes. Ahora bien, en la práctica sólo se construye un subconjunto de éstos como veremos más adelante.

### 1.2. Álgebra de Boole

Un **álgebra de Boole** es una entidad matemática formada por un conjunto que contiene dos elementos, unas operaciones básicas sobre estos elementos y una lista de axiomas que definen las propiedades que cumplen las operaciones.

Los dos **elementos** de un álgebra de Boole se pueden llamar falso y cierto o, más usualmente, $0$ y $1$. De este modo, una variable booleana o **variable lógica** puede tomar los valores $0$ y $1$. 

Las **operaciones booleanas** básicas son las siguientes:

> [!IMPORTANT]  
> La **negación** o complementación o **NOT**, que corresponde a la partícula no y se representa con una comilla simple (’). Así, la expresión $x’$ denota la negación de la variable $x$, y se lee $no x$.
> 
> El **producto lógico** o **AND**, que corresponde a la conjunción $y$ de la lógica y se representa con el símbolo (·). Así, si $x$ e $y$ son variables lógicas, la expresión $x \cdot y$ denota su producto lógico y se lee $x e y$.
> 
> La **suma lógica** u **OR**, que corresponde a la conjunción $o$ y se representa con el símbolo $+$. Así, la expresión $x + y$ denota la suma lógica de las variables $x$ e $y$, y se lee $x o y$.

Estas operaciones booleanas básicas se pueden definir escribiendo el resultado que dan para cada posible combinación de valores de las variables de entrada, tal como se muestra en la figura 6.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%206.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="555" height="auto"/>
    <p><em>Figura 6: Operaciones booleanas básicas. Fuente: UOC</em></p>
  </div>

## 2. Representación de funciones lógicas

### 2.1. Definición de operadores booleanos

Los **operadores booleanos** son herramientas fundamentales del álgebra de Boole. A continuación, se presentan los operadores más comunes:

1. **NOT** (Negación): Produce el valor opuesto de una entrada. Si la entrada es `1`, el resultado es `0` y viceversa.
2. **AND** (Conjunción): Devuelve `1` si todas las entradas son `1`. Si alguna es `0`, el resultado es `0`.
3. **OR** (Disyunción): Devuelve `1` si al menos una de las entradas es `1`. Solo es `0` si todas las entradas son `0`.
4. **NAND** (Negación de AND): Devuelve el valor opuesto al de la operación AND.
5. **NOR** (Negación de OR): Devuelve el valor opuesto al de la operación OR.
6. **XOR** (Disyunción exclusiva): Devuelve `1` si exactamente una de las entradas es `1`. Si todas las entradas son iguales, devuelve `0`.

### 2.2. Tablas de verdad

Las tablas de verdad permiten visualizar los resultados de los operadores booleanos para todas las combinaciones posibles de entradas. A continuación, se muestra un ejemplo para los operadores definidos:

| Entrada A | Entrada B | NOT A | A AND B | A OR B | A NAND B | A NOR B | A XOR B |
|-----------|-----------|--------|---------|--------|----------|---------|---------|
| 0         | 0         | 1      | 0       | 0      | 1        | 1       | 0       |
| 0         | 1         | 1      | 0       | 1      | 1        | 0       | 1       |
| 1         | 0         | 0      | 0       | 1      | 1        | 0       | 1       |
| 1         | 1         | 0      | 1       | 1      | 0        | 0       | 0       |

#### Ejemplo:
Consideremos el siguiente problema:
- María no irá a la escuela si hace frío **y** llueve **o** no ha hecho sus deberes.
  - Entrada A: Hace frío.
  - Entrada B: Llueve.
  - Entrada C: Ha hecho sus deberes.

| Frío (A) | Llueve (B) | Deberes (C) | Salida (No va a la escuela) |
|-----------|------------|-------------|-----------------------------|
| 0         | 0          | 0           | 0                           |
| 0         | 1          | 0           | 1                           |
| 1         | 0          | 1           | 0                           |
| 1         | 1          | 0           | 1                           |

### 2.3. Diagramas lógicos

Los diagramas lógicos representan de manera gráfica las operaciones booleanas mediante puertas lógicas. Cada operador booleano tiene una representación específica:

1. **NOT**: Triángulo con un círculo en la salida.
2. **AND**: Rectángulo con forma curva en los extremos.
3. **OR**: Forma curva con dos entradas y una salida.
4. **NAND**: Igual que AND, pero con un círculo en la salida.
5. **NOR**: Igual que OR, pero con un círculo en la salida.
6. **XOR**: Igual que OR, pero con una línea adicional en la entrada.
