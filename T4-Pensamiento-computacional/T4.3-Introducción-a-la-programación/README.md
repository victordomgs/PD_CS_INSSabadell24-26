<h1 align="center">4.3. Introducción a la programación
<div align="center">

</div>

## Contenido:

- [4.3.1. Operaciones fundamentales de un computador](#431-operaciones-fundamentales-de-un-computador)
- [4.3.2. Distinción entre operaciones fundamentales y operaciones compuestas](#432-distinción-entre-operaciones-fundamentales-y-operaciones-compuestas)
- [4.3.3. Características esenciales del lenguaje informático](#433-característica-esenciales-del-lenguaje-informático)
- [4.3.4. Necesidad de los lenguajes de alto nivel](#434-necesidad-de-los-lenguajes-de-alto-nivel)
- [4.3.5. Lenguaje de alto nivel y código máquina](#435-lenguaje-de-alto-nivel-y-código-máquina)
- [4.3.6. Variable, constante, operador y objeto](#436-variable-constante-operador-y-objeto)
- [4.3.7. Definición de operadores](#437-definición-de-operadores)
- [4.3.8. Análisis del uso de variables, constantes y operadores en algoritmos](#438-análisis-del-uso-de-variables-constantes-y-operadores-en-algoritmos)
- [4.3.9. Elaboración de algoritmos usando bucles y bifurcaciones](#439-elaboración-de-algoritmos-usando-bucles-y-bifurcaciones)
- [4.3.10. Descripción de las características de una colección](#4310-descripción-de-las-características-de-una-colección)
- [4.3.11. Desarrollo de algoritmos con el método de acceso a una colección](#4311-desarrollo-de-algoritmos-con-el-método-de-acceso-a-una-colección)
- [4.3.12. Importancia de los subprogramas en colecciones](#4312-importancia-de-los-subprogramas-en-colecciones)
- [4.3.13. Elaboración de algoritmos usando subprogramas predefinidios, matrices unidimensionales y colecciones](#4313-elaboración-de-algoritmos-usando-subprogramas-predefinidos-matrices-unidimensionales-y-colecciones)

---

## 4.3.1. Operaciones fundamentales de un computador

Un ordenador puede realizar algunas **operaciones fundamentales**. El siguiente ejemplo simplificado se utiliza para ilustrar algunas operaciones básicas. Supongamos que un número está almacenado como una cadena de bits en la ubicación de memoria 20 y otro número está almacenado como una cadena de bits en la ubicación de memoria 30. Una instrucción LOAD 20 se transfiere desde la RAM a la Unidad de Control (CU). El contenido de la ubicación de memoria 20 se carga (recupera de la memoria) en la Unidad Aritmético-Lógica (ALU). Se obtiene una segunda instrucción. La CU toma la instrucción ADD 30, carga el contenido de la ubicación de memoria 30 en la ALU y lo suma al número que ya está allí (el número de la ubicación de memoria 20). Una instrucción final STORE 50 se utiliza para almacenar la salida en la ubicación de memoria 50.

Una variación de este fragmento simple de código de máquina sería usar una instrucción que COMPARE (<, >, =) el contenido de la ubicación de memoria 20 con el contenido de la ubicación de memoria 40 y cambie el curso del programa de acuerdo con el resultado de la comparación. Las instrucciones condicionales y las operaciones básicas del álgebra booleana (AND, OR, XOR, NOT) son fundamentales para el desarrollo de programas útiles.

## 4.3.2. Distinción entre operaciones fundamentales y operaciones compuestas

Al combinar operaciones fundamentales de un ordenador, los ordenadores pueden realizar operaciones compuestas. Por ejemplo, encontrar el valor máximo de cuatro números es una **operación compuesta**.

Objetivo: Encontrar el valor máximo de cuatro números

Nuestro objetivo es escribir un algoritmo en forma de pseudocódigo que encuentre el máximo de cuatro números.
Cuatro números como entrada: a, b, c, d.

Debe dar como salida el valor máximo de esos cuatro (MAX).
Siempre debe dar el máximo (el valor real o el orden de los números no debe influir en nuestro algoritmo).

```pseudocode
Begin by setting MAX = a 
Compare MAX and b. 
If b > MAX, setb=MAx 
Compare MAX and c. 
If e > MAX, set c = MAX 
Compare MAX and d. 
If d > MAX, set d = MAX
Output MAX
```

## 4.3.3. Características esenciales del lenguaje informático

Un lenguaje de programación se describe como la combinación de su **semántica**, que se refiere al significado de cada construcción posible en el lenguaje, y su **sintaxis**, que se relaciona con su estructura.

Una **gramática** es un meta-lenguaje que se utiliza para definir la sintaxis de un lenguaje, mientras que las reglas de construcción de sentencias se llaman sintaxis. Cada lenguaje de alto nivel tiene una sintaxis única y un vocabulario específico y limitado.

Las palabras import, class, int, etc., en Java son **palabras reservadas** (reserved keywords) con significados especiales en el lenguaje Java.

Un comando escrito en un lenguaje de programación siempre significa lo mismo y no existe ambigüedad en su interpretación.

## 4.3.4. Necesidad de los lenguajes de alto nivel

Los ordenadores solo pueden procesar 0s y 1s. Cada ordenador tiene su propio **lenguaje máquina**, que está compuesto únicamente de 0s y 1s. El lenguaje máquina es un lenguaje de bajo nivel y es el único que puede ser entendido directamente por un ordenador.

Los programas en lenguaje máquina son difíciles de escribir, difíciles de depurar y de mantener. Un programador en lenguaje máquina tiene que llevar un registro de las ubicaciones de memoria y escribir desde el principio todas las funciones matemáticas requeridas por un programa. Los programas en lenguaje máquina escritos para un ordenador de un tipo no son adecuados para un ordenador de otro tipo.

El siguiente paso evolutivo en la programación vino con la sustitución del código binario para el desarrollo de instrucciones y referencias a direcciones de memoria por símbolos llamados **mnemónicos**. Estos lenguajes de bajo nivel se denominaron lenguaje **mnemónico** y más tarde **lenguajes ensambladores**. Un **ensamblador** se utilizaba para convertir los mnemónicos del lenguaje ensamblador en código máquina.

El desarrollo de programas informáticos se volvió mucho más sencillo, pero cada lenguaje ensamblador seguía siendo específico para un sistema de computación concreto. La falta de abstracción, la necesidad de centrarse en la resolución de problemas y la mejora de la eficiencia llevaron al desarrollo de los lenguajes de alto nivel.

Un lenguaje de **programación de alto nivel** es un lenguaje de programación que utiliza elementos del lenguaje natural, es fácil de usar, facilita la abstracción al ocultar áreas importantes de los sistemas de computación y hace que el desarrollo de programas sea más simple, rápido y comprensible.

## 4.3.5. Lenguaje de alto nivel y código máquina

La mayoría de aplicaciones actuales están escritas en uno de los **lenguajes de alto nivel**. Para ejecutar (RUN) el programa en un sistema informático y obtener el resultado deseado, es necesario un proceso de traducción. Este **proceso de traducción** convierte el programa al **lenguaje máquina** del ordenador en el que se ejecutará.

El programa original desarrollado en un lenguaje de alto nivel se llama **programa fuente** o source code. El programa traducido a lenguaje máquina se llama **programa objeto** o target program.

Se utilizan dos métodos de traducción: **compilación** e **interpretación**.

- **Un compilador** es un traductor que ejecuta el proceso de traducción solo una vez. Normalmente traduce todo el programa fuente al programa objeto. El programa objeto se guarda y, la siguiente vez que un programador quiera usarlo, no será necesario volver a traducirlo. Los compiladores detectan errores de sintaxis durante la traducción y comunican todos los errores al programador cuando el programa entero ha sido revisado. La compilación solo finaliza cuando se han corregido todos los errores de sintaxis. Los compiladores son mucho más rápidos que los intérpretes.
Ejemplos: C, C++.

- **Un intérprete** es un traductor que pasa por el proceso de traducción cada vez que el programa se ejecuta. La interpretación consiste en leer cada línea (instrucción) del programa fuente, analizarla, traducirla a la instrucción correspondiente del programa objeto y ejecutar la línea. Los errores de sintaxis se comunican al programador en cada instrucción que se interpreta.
Ejemplo: BASIC.

- **Java combina compilación e interpretación**. El código fuente se compila a **bytecode de la Máquina Virtual de Java (Java Virtual Machine bytecode)**. Cuando un programa Java se compila de `.java` a `.class file`, la clase es código bytecode de la JVM. Este bytecode puede ser interpretado por el **intérprete de la Máquina Virtual de Java**. La arquitectura Java permite ejecutar el mismo código en cualquier máquina en la que esté instalada la JVM. En Java, en realidad, todos los detalles de la ejecución del código en una plataforma de hardware específica son manejados por la **Máquina Virtual de Java (JVM)**.

## 4.3.6 Variable, constante, operador, objeto

### Variable:

Una variable se utiliza para almacenar un elemento de datos de un programa. El valor almacenado puede cambiarse durante la ejecución del programa. Una variable tiene un nombre (o identificador) y un tipo. El nombre de la variable no debe coincidir con palabras reservadas ni literales del lenguaje.
Es muy recomendable usar nombres de variables significativos (por ejemplo: `roomSize`). El tipo de la variable puede ser un número entero, un número decimal, una cadena de texto, etc. En la mayoría de lenguajes de programación, una variable solo puede almacenar un elemento de datos del tipo particular definido.

### Constante:

Las constantes representan cosas y cantidades que no cambian. Pueden considerarse como variables no modificables. El elemento de datos almacenado en una constante no puede modificarse durante la ejecución del programa (por ejemplo, en Java: `final double PI = 3.14159`).

### Operador:

Los operadores se utilizan para manipular operandos. La expresión `2 + 3` tiene como operador el “+” (signo de suma) y dos operandos: `2` y `3`. Los operandos pueden ser variables, literales, valores booleanos, valores numéricos, cadenas de texto, etc.
Los operadores pueden ser: aritméticos, relacionales, lógicos, etc.

### Objeto:

Un objeto está compuesto de **datos** y **acciones**.

- Los datos representan el estado del objeto y se almacenan en miembros de datos (data members).
- Las acciones se refieren a las operaciones que pueden realizarse sobre el objeto y también se llaman **métodos**.

Los miembros de datos se usan para almacenar el estado actual de un objeto y los métodos se utilizan para cambiar o acceder a esos datos.

## 4.3.7. Definición de operadores

Los siguientes operadores aparecen en la notación aprobada por el IBO para desarrollar pseudocódigo:

- = Definido como “es igual a”. También se usa para asignar un valor a una variable. Ejemplo: `Min = 6` significa que el valor 6 se asigna a la variable Min.
- ≠ Definido como “no es igual a”. Ejemplo: `Min ≠ Max` significa que Min no es igual a Max.
- > Definido como “es mayor que”.
- ≥ Definido como “es mayor o igual que”.
- < Definido como “es menor que”.
- ≤ Definido como “es menor o igual que”.
- div Definido como “parte entera del cociente”. Ejemplo: `22 div 3 = 7`.

mod Definido como “operación módulo”. Calcula el resto de la división de un número entre otro.

La siguiente tabla ilustra algunos ejemplos de uso de mod y div:

| Operando1 | Operador | Operando2 | Resultado |
|-----------|----------|-----------|-----------|
| 9         | mod      | 3         | 0 |
| 11        | mod      | 3         | 2 |
| 0         | mod      | 3         | 0 |
| 22        | div      | 3         | 7 |
| 2         | mod      | 44        | 2 |

## 4.3.8. Análisis del uso de variables, constantes y operadores en algoritmos

Está claro que una constante es una variable cuyo valor no cambia durante la ejecución del programa.

| Nombre de la constante | Valor de la constante |
|-------------------------|-----------------------|
| π (pi)                  | 3.141592653           |
| e (logaritmo natural)   | 2.718281828           |
| c (velocidad de la luz) | 299,792,458 (m/s)     |

En algunos casos, cuando se desarrolla un programa informático, es más conveniente y seguro usar **constantes** en lugar de variables. Cuando se utiliza la palabra clave final, Java entiende que el valor del elemento de datos no puede modificarse.
Si intentas cambiar una constante, como Pi, aparecerá un mensaje:
“**cannot assign a value to final variable Pi**” (no se puede asignar un valor a la variable final Pi).

### Valores locales y globales

El **ámbito (scope) de una variable** define la visibilidad de esa variable. Es decir, determina qué partes del algoritmo pueden almacenar, acceder y recuperar los datos de la variable.

En algunos casos es muy útil limitar el ámbito de una variable:

- Una **variable global** es visible en todas las partes del programa.
- Una **variable local** tiene un ámbito limitado.

## 4.3.9. Elaboración de algoritmos usando bucles y bifurcaciones

WIP

## 4.3.10. Descripción de las características de una colección

Con frecuencia, en la programación informática existe la necesidad de **agrupar y almacenar datos** que se usarán para la solución de un problema.

Una **colección** o **contenedor** está compuesta por cero o más elementos, como objetos y valores, y cuenta con las operaciones necesarias para gestionar los datos.

Las colecciones permiten elementos duplicados y pueden contener datos ordenados o no ordenados.

Las operaciones más importantes de una colección son **añadir (add), eliminar (remove)**, etc. Cada tipo de colección tiene sus propias operaciones específicas.

Los elementos de una colección concreta suelen ser todos del mismo tipo y representar una entidad.

Un **array de tamaño fijo** generalmente **no se considera una colección**, ya que almacena un número fijo de elementos.

## 4.3.11. Desarrollo de algoritmos con el método de acceso a una colección

WIP

## 4.3.12. Importancia de los subprogramas en colecciones

Un **subprograma** es una unidad que contiene una secuencia de instrucciones que realizan una tarea específica y predefinida. Los subprogramas son muy útiles porque permiten a los programadores aprovechar código y soluciones existentes desarrolladas por otros (o por ellos mismos) para acelerar sus tareas.

La **reutilización de código** ahorra tiempo y recursos, y permite completar proyectos exigentes en el menor tiempo posible. Los autores de nuevos programas pueden aprovechar las **bibliotecas de software**, que contienen subprogramas reutilizables en distintos tipos de programas.

### Ventajas de dividir un programa en subprogramas:

- Descomponer un problema complejo de programación en tareas más simples.
- Distribuir un problema de programación muy grande entre distintos programadores en diferentes lugares.
- Habilitar la reutilización de código en múltiples programas.
- Facilitar la abstracción al ocultar detalles de implementación dentro del subprograma.
- Mejorar el mantenimiento y la trazabilidad.
- Reducir la duplicación de código dentro de un mismo programa.

### Ventajas de usar colecciones:

- Los métodos de las colecciones son algoritmos predefinidos que el programador puede usar inmediatamente.
- El rendimiento aumenta gracias a las capacidades de gestión de datos que proporciona la colección.
- Se facilita la reutilización de software porque el uso de métodos se basa en un lenguaje común y una interfaz estándar.

## 4.3.13. Elaboración de algoritmos usando subprogramas predefinidios, matrices unidimensionales y colecciones

En los distintos lenguajes de programación se utilizan términos como **procedimiento, subprocedimientos, función, rutina, método, subrutinas, módulos**, etc., para referirse a los **subprogramas**.

Un **subprograma** es una unidad que contiene una secuencia de instrucciones de computadora que realizan una tarea específica y predefinida. Esta unidad puede usarse en distintos programas cuando esa tarea debe implementarse.

Los subprogramas pueden definirse dentro de un programa o bien de forma separada en **bibliotecas**, que pueden ser reutilizadas por múltiples programas.

En el lenguaje de programación **C++**, por ejemplo:

- Un **procedimiento** realiza una tarea.
- Una **función** produce información y devuelve un valor.

Es importante señalar que, en la mayoría de los casos, una **función** devuelve un valor mientras que un **procedimiento** simplemente ejecuta comandos.

En **Java** se usan los **métodos** para representar subprogramas. Un método en Java puede devolver un valor, y el programa principal puede pasar una o más variables a un método.

- Un **parámetro** es el nombre de la información que se usa en un método, función o procedimiento.
- Un **argumento** es el valor que se pasa a un método, función o procedimiento.

Normalmente, un **módulo** se refiere a una pequeña sección de un programa que está personalizada para ejecutar una tarea particular. Los módulos pueden adaptarse por un programador para realizar un trabajo concreto.
