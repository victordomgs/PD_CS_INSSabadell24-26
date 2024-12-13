<h1 align="center">Puertas lógicas simples
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
<a href="https://www.linkedin.com/in/v%C3%ADctor-garc%C3%ADa-saiz-/"><img src="https://img.shields.io/badge/LinkedIn-Perfil-%230077B5" alt="Perfil de LinkedIn"/></a>
</a>



</div>

## Contenido:
[1. Introducción a las puertas lógicas](#1-introducción-a-las-puertas-lógicas)  
  - [1.1. ¿Qué son las puertas lógicas?](#11-que-son-las-puertas-lógicas)
  - [1.2. Álgebra de Boole](#12-álgebra-de-boole)
  - [1.3. Teorema del álgebra de Boole](#13-teorema-del-álgebra-de-Boole)
[2. Representación de funciones lógicas](#1-representación-de-funciones-lógicas)
  - [2.1. Expresiones algebraicas](#11-expresiones-algebraicas)

## 1. Introducción a las puertas lógicas

### 1.1. ¿Qué son las puertas lógicas?

Un **circuito lógico** es un sistema compuesto por señales de entrada, dispositivos electrónicos que procesan esas señales, y señales de salida que son el resultado de dichas operaciones. Estas señales son binarias, lo que significa que solo pueden tomar dos valores: 0 (tensión baja) y 1 (tensión alta). Una señal está activa cuando su valor es 1.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%201.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="465" height="auto"/>
    <p><em>Figura 1: Circuito lógico. Fuente: UOC</em></p>
  </div>

Las señales de entrada y salida de un circuito lógico son funciones lógicas que representan operaciones realizadas por los dispositivos electrónicos del circuito. Estas operaciones se fundamentan en principios del **Álgebra de Boole**, y las señales binarias son manipuladas electrónicamente para producir un resultado lógico.

En este contexto, las **puertas lógicas** son los elementos básicos que realizan estas operaciones. Son dispositivos electrónicos que computan funciones lógicas específicas a partir de las señales de entrada.

> [!IMPORTANT]  
> Puesto que las señales sólo pueden tomar dos valores, diremos que uno es el contrario del otro. Así pues, podemos afirmar que cuando una señal no vale 1, entonces seguro que vale 0, y viceversa.

Tomamos un circuito que tenga sólo una señal de entrada (que llamamos x), un dispositivo electrónico y una señal de salida (que llamamos z).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%202.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="361" height="auto"/>
    <p><em>Figura 2: Circuito lógico con una entrada. Fuente: UOC</em></p>
  </div>

Dado que tanto x como z sólo pueden valer 0 ó 1, sólo existen cuatro dispositivos electrónicos diferentes que pueden interconectar x y z:
- Un dispositivo que haga que la salida z valga siempre 0 (este dispositivo consistiría en conectar la salida con una fuente de tensión de 0 voltios).
- Un dispositivo que haga que la salida valga siempre lo mismo que la entrada x (este dispositivo consistiría en conectar directamente la salida con la entrada).
- Un dispositivo que haga que la salida valga siempre lo contrario de lo que vale la entrada (este dispositivo consistiría en un inversor del nivel de tensión).
- Un dispositivo que haga que la salida valga siempre 1 (este dispositivo consistiría en conectar la salida directamente con la tensión de alimentación).

En otras palabras, podemos decir que sólo hay cuatro funciones lógicas que tengan una sola variable de entrada, tal como se muestra en la figura 3:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%203.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="476" height="auto"/>
    <p><em>Figura 3: Funciones lógicas sobre el circuito lógico de la Figura 2. Fuente: UOC</em></p>
  </div>

Tomamos ahora un circuito que tenga dos señales de entrada (que llamamos x e y), un dispositivo electrónico y una señal de salida (que llamamos z).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%204.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="297" height="auto"/>
    <p><em>Figura 4: Circuito lógico con dos entradas. Fuente: UOC</em></p>
  </div>

En este caso, existen dieciséis dispositivos electrónicos diferentes que puedan interconectar las entradas con la salida, que corresponden a las funciones lógicas que se muestran en la figura 5.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%205.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="473" height="auto"/>
    <p><em>Figura 5: Funciones lógicas sobre el circuito lógico de la Figura 4. Fuente: UOC</em></p>
  </div>

Así pues, si tenemos en cuenta los circuitos con una o dos entradas, podemos llegar a diseñar hasta 4 + 16 = 20 dispositivos electrónicos diferentes. Ahora bien, en la práctica sólo se construye un subconjunto de éstos como veremos más adelante.

### 1.2. Álgebra de Boole

Un **álgebra de Boole** es una entidad matemática formada por un conjunto que contiene dos elementos, unas operaciones básicas sobre estos elementos y una lista de axiomas que definen las propiedades que cumplen las operaciones.

Los dos **elementos** de un álgebra de Boole se pueden llamar falso y cierto o, más usualmente, 0 y 1. De este modo, una variable booleana o **variable lógica** puede tomar los valores 0 y 1. 

Las **operaciones booleanas** básicas son las siguientes:

> [!IMPORTANT]  
> La **negación** o complementación o **NOT**, que corresponde a la partícula no y se representa con una comilla simple (’). Así, la expresión "x’" denota la negación de la variable "x", y se lee “no x”.
> 
> El **producto lógico** o **AND**, que corresponde a la conjunción "y" de la lógica y se representa con el símbolo “·”. Así, si "x" e "y" son variables lógicas, la expresión "x · y" denota su producto lógico y se lee “x e y”.
> 
> La **suma lógica** u **OR**, que corresponde a la conjunción "o" y se representa con el símbolo “+”. Así, la expresión “x + y” denota la suma lógica de las variables "x" e "y", y se lee “x o y”.

Estas operaciones booleanas básicas se pueden definir escribiendo el resultado que dan para cada posible combinación de valores de las variables de entrada, tal como se muestra en la figura 6.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%206.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="555" height="auto"/>
    <p><em>Figura 6: Operaciones booleanas básicas. Fuente: UOC</em></p>
  </div>

Los **axiomas** que describen el comportamiento de las operaciones booleanas son los siguientes:
1. **La propiedad conmutativa:** el orden de las variables no importa.
```
x+y=y+x
x⋅y=y⋅x
```
2. **La propiedad asociativa:** el agrupamiento de las variables no afecta al resultado.
```
x+(y+z)=(x+y)+z
x⋅(y⋅z)=(x⋅y)⋅z
```
3. **La propiedad distributiva:** cómo distribuir una variable entre otras en las operaciones.
```
x⋅(y+z)=(x⋅y)+(x⋅z)
x+(y⋅z)=(x+y)⋅(x+z)
```
4. **Elementos neutros:** 0 es el elemento neutro de OR y 1 es el elemento neutro de AND.
```
x+0=x
x⋅1=x
```
5. **Complementación:** el complemento de una variable (x') es su inverso lógico.
```
x+x'=1
x⋅x'=0
```
A partir de estos axiomas, se puede demostrar una serie de leyes o teoremas muy útiles para trabajar con expresiones algebraicas booleanas.

### 1.3. Teorema del álgebra de Boole

Si "x", "y" y "z" son variables lógicas, se cumplen las siguientes leyes:

1. **Principio de dualidad:** establece que cualquier identidad válida siguie siendo verdadera si:
```
Se intercambian las operaciones + (OR) y · (AND).
Se intercambian los valores constantes 0 y 1.
```
2. **Ley de idempotencia:**
```
x+x=x: Si un valor lógico se OR con sí mismo, el resultado es el mismo valor.
x·x=x: Si un valor lógico se AND con sí mismo, el resultado es el mismo valor.
```
3. **Ley de absorción:** se simplifican expresiones lógicas eliminando redundacias.
```
x+(x⋅y)=x: Si "x" ya está presente, cualquier AND adicional con "y" no cambia el resultado.
x⋅(x+y)=x: Si "x" ya está presente, cualquier OR adicional con "y" no cambia el resultado.
```
4. **Ley de dominancia:** estas leyes reflejan el impacto de los valores extremos 1 y 0 en OR y AND:
```
x+1=1: OR con 1 siempre da 1.
x·0=0: AND con 0 siempre da 0.
```
5. **Ley de involución:** la doble negación de un valor lógico devuelve el valor original.
```
(x')'=x
```
6. **Leyes de Morgan:** estas leyes transforman una expresión con AND en una con OR (y viceversa) cuando se aplica la negación:
```
(x+y)'=x'·y'
(x·y)'=x'+y'
```

> [!WARNING]  
> En las expresiones algebraicas utilizamos los paréntesis de la misma forma que estamos acostumbrados a hacerlo en aritmética tradicional; por ejemplo, la expresión "x+y·z" es lo mismo que la "x+(y·z)" y es diferente que "(x+y)·z".
> 
> Para negar una expresión entera la pondremos entre paréntesis y, por tanto, x+y' es diferente de (x+y)'.

A continuación, veremos que existe una correspondencia entre los elementos de un circuito lógico y la lógica intuitiva (de aquí deriva la denominación de circuitos “lógicos”). La lógica tiene cinco componentes básicos:
– Los valores falso y cierto.
– Las conjunciones y y o.
– La partícula de negación no.

Por ejemplo, sean las dos frases siguientes:
```
frase_A: “Juan estudia química”,
frase_B: “Carmen estudia piano”.
```
Cada una de estas frases puede ser verdadera o falsa. A partir de éstas, de las conjunciones y la negación construimos ahora las tres frases siguientes:
```
frase_Y: “Juan estudia química y Carmen estudia piano”,
frase_O: “Juan estudia química o Carmen estudia piano”,
frase_NO: “Juan no estudia química”.
```

Según la lógica:
- La frase_Y es verdadera sólo si son ciertas la frase_A y la frase_B, simultáneamente.
- La frase_O es verdadera si lo es la frase_A o bien la frase_B, o ambas.
- La frase_NO es verdadera sólo si la frase_A es falsa.

La correspondencia de la lógica con los elementos de un circuito lógico es la siguiente:

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%206.%20Puertas%20l%C3%B3gicas%20simples.png" alt="Puertas lógicas simples" width="398" height="auto"/>
    <p><em>Figura 7: Correspondencia lógica con la Figura 3 y Figura 5. Fuente: UOC</em></p>
  </div>

En efecto, sean dos señales lógicas x e y. Si analizamos las tablas de las figuras 1 y 2, podemos observar lo siguiente:
- g1(x,y) vale 1 si valen 1 las dos variables x e y simultáneamente;
- g7(x,y) vale 1 si x vale 1 o bien y vale 1 o bien las dos valen 1;
- f2(x) vale 1 sólo si x vale 0.

Es decir, se cumple lo mismo que en el ejemplo de las frases. Por eso, la función g1 se llama AND (la conjunción y en inglés), la función g7 se denomina OR (la conjunción o en inglés) y la función f2 se llama NOT (no en inglés).

## 2. Representación de funciones lógicas.

Las funciones lógicas se pueden expresar de varias maneras. Las que usaremos nosotros son las **expresiones algebraicas** y las **tablas de verdad**.

### 2.1. Expresiones algebraicas

Las **expresiones algebraicas** estan formadas por variables lógicas, los elementos 0 y 1, los operadores producto (·), suma (+) y negación (’), y los símbolos (,) e =.

 g_4(x, y)
