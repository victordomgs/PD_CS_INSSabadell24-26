<h1 align="center">4.2. Relación entre pensamiento computacional y diseño de programas
<div align="center">

</div>

## Contenido:

- [4.2.1 Describa las características de los algoritmos estándares de matrices lineales](#421-describa-las-características-de-los-algoritmos-estándares-de-matrices-lineales)
- [4.2.2 Resuma las operaciones estándares de las colecciones](#422-resuma-las-operaciones-estándares-de-las-colecciones)
- [4.2.3 Discuta un algoritmo que resuelva un problema específico](#423-discuta-un-algoritmo-que-resuelva-un-problema-específico)
- [4.2.4 Analice un algoritmo que se presente en forma de diagrama de flujo](#424-analice-un-algoritmo-que-se-presente-en-forma-de-diagrama-de-flujo)
- [4.2.5 Analice un algoritmo que se presente como pseudocódigo](#425-analice-un-algoritmo-que-se-presente-como-pseudocódigo)
- [4.2.6 Elabore pseudocódigo para representar un algoritmo](#426-elabore-pseudocódigo-para-representar-un-algoritmo)
- [4.2.7 Sugiera algoritmos adecuados para resolver un problema específico](#427-sugiera-algoritmos-adecuados-para-resolver-un-problema-específico)
- [4.2.8 Deduzca la eficacia de un algoritmo en el contexto de su uso](#428-deduzca-la-eficacia-of-un-algoritmo-en-el-contexto-de-su-uso)
- [4.2.9 Determine el número de veces que se ejecutará una instrucción en un algoritmo para unos datos de entrada concretos](#429-determine-el-número-de-veces-que-se-ejecutará-una-instrucción-en-un-algoritmo-para-unos-datos-de-entrada-concretos)

---

## 4.2.1 Describa las características de los algoritmos estándares de matrices lineales

### Variables

En informática, una variable actúa como una ubicación de almacenamiento que puede usarse para guardar un valor.
Cada variable tiene un nombre (también se usa el término identificador) que se utiliza para referirse al valor almacenado.
El valor de la variable puede cambiar durante la ejecución del programa. Cada variable puede almacenar un tipo particular de dato como **cadenas (strings)**, **reales**, **booleanos** y **enteros**.

### Arreglos unidimensionales o arreglos lineales

Una variable solo puede almacenar un elemento de datos de un programa.
Si se necesita un segundo elemento, entonces debe crearse otra variable. Cuantos más elementos se necesiten, más variables distintas debe crear el programador.

Un **arreglo (array)** puede contener múltiples elementos del mismo tipo de dato (enteros, cadenas, booleanos, etc.).
Un arreglo tiene:

- un **nombre**,
- un **tamaño** (no puede cambiarse durante la ejecución en la mayoría de los casos),
- y un **tipo de dato** que describe lo que puede almacenar.

Un **arreglo unidimensional** es un tipo de arreglo lineal. Muchos lenguajes de programación, incluido Java, definen siempre el límite inferior del arreglo empezando en el número **0**.

#### 📌Ejemplo de programación 1: Uso de un arreglo (arreglo de números)

El siguiente programa llenará el arreglo **A** con valores del **1 al 10** y luego imprimirá sus valores.

```pseudocode
// ==== Arrays ====
A = new Array()
N = 0

loop N from 0 to 9
    A[N] = N + 1
end loop

loop N from 0 to 9
    output "Array position ", N, " contains the value ", A[N]
end loop
```

Salida esperada: 

```sql
Array position 0 contains the value 1
Array position 1 contains the value 2
Array position 2 contains the value 3
Array position 3 contains the value 4
Array position 4 contains the value 5
Array position 5 contains the value 6
Array position 6 contains the value 7
Array position 7 contains the value 8
Array position 8 contains the value 9
Array position 9 contains the value 10
```
### Arreglos bidimensionales

Un **array unidimensional** se considera como una sola línea de elementos.  
Sin embargo, en muchos casos, los datos vienen en forma de tabla.  
Un ejemplo típico es una tabla que muestra la **temperatura media mensual** de 10 ciudades.

|                 | City 1 (Index 0) | City 2 (Index 1) | City 3 (Index 2) | ... | City 10 (Index 9) |
|-----------------|------------------|------------------|------------------|-----|-------------------|
| January (Index 0)   | 15               | 28               | 20               | ... | 20                |
| February (Index 1)  | 14               | 27               | 20               | ... | 19                |
| ...             | ...              | ...              | ...              | ... | ...               |
| December (Index 11) | 15               | 26               | 21               | ... | 20                |


> [!NOTE]
> 1. Los arrays 2D se indexan con dos subíndices.  
>    - El primero se refiere a la **fila**.  
>    - El segundo se refiere a la **columna**.  
>    - Ejemplo: `TEMP[1][1]` → temperatura de febrero en la ciudad 2.
> 2. En este caso, el valor `27` corresponde a `TEMP[1][1]`.  
> 3. Todos los elementos de un array bidimensional deben ser del **mismo tipo de dato**.  

#### 📌Ejemplo de programación 2: Arreglo bidimensional (temperaturas)

```pseudocode
// This program will use the array TEMP which is a 2D ARRAY
// It will print the contents of the array
// 12 months 5 cities

TEMP = [
    [10,11,12,13,10],
    [10,13,14,12,12],
    [13,13,14,15,12],
    [16,17,17,17,16],
    [22,23,24,24,24],
    [26,25,24,25,26],
    [29,28,26,27,26],
    [29,28,27,28,28],
    [24,23,24,25,25],
    [20,21,22,23,24],
    [15,16,17,18,18],
    [12,11,13,11,11]
]

MONTH = 0
CITY = 0

loop MONTH from 0 to 11
    output MONTH+1, "Month"

    loop CITY from 0 to 4
        output "City", CITY+1, TEMP[MONTH][CITY]
    end loop
end loop
```

### Algoritmos de búsqueda en arreglos

#### Sequential Search (búsqueda secuencial o lineal)

Se recorre la lista **uno por uno** hasta encontrar el elemento buscado o hasta llegar al final. Funciona tanto en **listas ordenadas com no ordenadas**.

**Complejidad:** Mejor caso: 𝑂(1) (si el elemento está al principio).Peor caso: 𝑂(𝑛).

#### 📌Ejemplo de programación 3: Búsqueda secuencial

```pseudocode
array = [8, 3, 5, 2, 9]
target = 5
found = False

for i from 0 to length(array)-1
    if array[i] = target then
        output "Element found in position ", i
        found = True
        break
    end if
end for

if found = False then
    output "Element not found"
end if
```

#### Binary Search (búsqueda binaria)

Solo funciona en **listas ordenadas**. Divide el arreglo a la mitad en cada paso: 

- Si el valor está en el medio → encontrado.
- Si el valor buscado es menor → buscar en la mitad izquierda.
- Si el valor buscado es mayor → buscar en la mitad derecha.

**Complejidad:** 𝑂(log 𝑛)

```pseudocode
array = [2, 3, 5, 8, 9, 12, 15]  // ordenado
target = 9
low = 0
high = length(array) - 1
found = False

while low <= high AND found = False
    mid = (low + high) DIV 2
    if array[mid] = target then
        output "Element found in position ", mid
        found = True
    else if array[mid] < target then
        low = mid + 1
    else
        high = mid - 1
    end if
end while

if found = False then
    output "Element not found"
end if
```

### Algoritmos de ordenación en arreglos

#### Bubble Sort (Ordenamiento Burbuja)

Compara **pares de elementos adyacentes** y los intercambia si están en el orden incorrecto. Repite el proceso hasta que no haya más cambios. Es sencillo pero **ineficiente en listas grandes**.

**Complejidad:** 𝑂(𝑛²).

```pseudocode
array = [5, 1, 4, 2, 8]
n = length(array)

for i from 0 to n-1
    for j from 0 to n-2
        if array[j] > array[j+1] then
            swap array[j], array[j+1]
        end if
    end for
end for

output array
```

#### Selection Sort (Ordenamiento por Selección)

Encuentra el **menor elemento** y lo coloca en la primera posición. Luego encuentra el segundo menor y lo coloca en la segunda posición, y así sucesivamente.

**Complejidad:** 𝑂(𝑛²).

```pseudocode
array = [64, 25, 12, 22, 11]
n = length(array)

for i from 0 to n-1
    min_index = i
    for j from i+1 to n-1
        if array[j] < array[min_index] then
            min_index = j
        end if
    end for
    swap array[i], array[min_index]
end for

output array
```

<br>

## 4.2.2 Resuma las operaciones estándares de las colecciones

Un **array** es una elección perfecta cuando un programador desea almacenar información del mismo tipo (por ejemplo, un grupo de strings) y sabe de antemano cuántos elementos desea guardar.

**Problema:** ¿qué ocurre si el programador quiere almacenar enteros, arrays, objetos, booleanos y strings en una misma estructura de datos?

La respuesta es usar **colecciones**, porque algunas permiten especificar los tipos de elementos que contendrán.

- En **C#** y **Visual Basic**, las **colecciones genéricas** solo pueden contener datos de un mismo tipo.
- Las **colecciones no genéricas**, en cambio, pueden almacenar elementos de diferentes tipos de datos.

**Ventaja principal de las colecciones**: actúan como un array redimensionable.
El programador **no necesita saber de antemano** cuántos elementos se colocarán en la estructura de datos.

### Operaciones estándar en colecciones

- `addItem()`: Se usa para añadir un elemento a la colección (adición).

```pseudocode
TEMPERATURES.addItem(32)
```
➝ Agrega `32` a la colección `TEMPERATURES`.

- `getNext()`: Devuelve el primer elemento de la colección la primera vez que es llamado (lectura).

```pseudocode
A = TEMPERATURES.getNext()
```
➝ Asigna a la variable `A` el valor del primer elemento de la colección.

### Operaciones adicionales

- `resetNext()`: Reinicia la iteración de la colección.

```pseudocode
TEMPERATURES.resetNext()
```

- `hasNext()`: Indica si quedan elementos por recorrer en la colección.

```pseudocode
if TEMPERATURES.hasNext() then ...
```
➝ Devuelve `TRUE` si aún existen elementos sin acceder.

- `isEmpty()`: Comprueba si la colección está vacía.

```pseudocode
if TEMPERATURES.isEmpty() then ...
```
➝ Devuelve TRUE si la colección no tiene elementos.

<br>

## 4.2.3 Discuta un algoritmo que resuelva un problema específico

#### 📌Ejemplo de programación 4: Temperaturas mínimas y máximas

Este programa que muestras es un **ejemplo clásico de uso de arrays y condicionales** para analizar temperaturas de varias ciudades.

Objetivo del programa: 

- Guardar **nombres de ciudades**, sus **temperaturas máximas** y **mínimas**.
- Calcular el **promedio de temperaturas máximas** y el **promedio de temperaturas mínimas**.
- Mostrar: Ciudades con máximas por encima del promedio. Ciudades con mínimas por debajo del promedio.

##### Declaración de variables y arreglos

```pseudocode
TOTALH = 0    // suma de las temperaturas máximas
TOTALL = 0    // suma de las temperaturas mínimas
AVGH = 0      // promedio de máximas
AVGL = 0      // promedio de mínimas

CITYNAMES = new Array()   // nombres de las ciudades
HIGHTEMP = new Array()    // temperaturas máximas
LOWTEMP = new Array()     // temperaturas mínimas
```

##### Entrada de datos

```pseudocode
loop I from 0 to 3
    CITYNAMES[I] = input("Type the name of the city")
    HIGHTEMP[I] = input("Type the Maximum temperature of the city")
    LOWTEMP[I] = input("Type the Minimum temperature of the city")

    TOTALH = TOTALH + HIGHTEMP[I]
    TOTALL = TOTALL + LOWTEMP[I]
end loop
```
➝ Aquí el usuario introduce **4 ciudades** (porque `0 to 3` son 4 iteraciones). Además, se van acumulando las máximas y mínimas para luego calcular promedios.

##### Cálculo de promedios

```pseudocode
AVGH = TOTALH / 4
AVGL = TOTALL / 4
```

##### Mostrar resultados

- Ciudades con máxima > promedio máximo:

```pseudocode
output "Cities Above Avg. High:"
loop I from 0 to 3
    if HIGHTEMP[I] > AVGH then
        output CITYNAMES[I], "+"
    end if
end loop
```

- Ciudades con mínima > promedio mínimo:

```pseudocode
output "Cities Below Avg. Low:"
loop I from 0 to 3
    if LOWTEMP[I] < AVGL then
        output CITYNAMES[I], "+"
    end if
end loop
```

<br>

## 4.2.4 Analice un algoritmo que se presente en forma de diagrama de flujo

#### 📌Ejemplo de programación 5: Verificación de contraseñas

**1. Declaración de variables:**

- `A` contendrá la contraseña correcta (`"MORGAN"`).
- `PASSWORD` contendrá la contraseña que introduce el usuario.

**2. Entrada:**

- Se le pide al usuario que introduzca una contraseña (`PASSWORD`).

**3. Condición:**

- Se compara `PASSWORD` con `A`.
- Si son iguales, se muestra "`CORRECT`".
- Si son diferentes, se muestra "`WRONG`".

```pseudocode
DECLARE A : STRING
DECLARE PASSWORD : STRING

A ← "MORGAN"
INPUT PASSWORD

IF PASSWORD = A THEN
    OUTPUT "CORRECT"
ELSE
    OUTPUT "WRONG"
END IF
```

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%209.%20Pensamiento%20computacional.png" alt="Diagrama de flujos" width="550" height="auto"/>
    <p><em>Figura 9: Diagrama de flujos de verificación de contraseña. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

#### 📌Ejemplo de programación 6: Verificación de contraseñas

```pseudocode
n = 0
loop while n <= 3
    output "OK"
    n = n + 1
end loop
output n
```
➝ El ciclo se repite mientras n <= 3 sea verdadero. Cada vez imprime "OK" y aumenta n en 1. Cuando n = 4, la condición se vuelve falsa y termina el bucle. Finalmente, imprime n = 4.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2010.%20Pensamiento%20computacional.png" alt="Diagrama de flujos" width="350" height="auto"/>
    <p><em>Figura 10: Diagrama de flujos utilizando while loop. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

```pseudocode
n = 0
loop n from 0 to 3
    output "OK"
end loop
output n
```
➝ Aquí el bucle establece que n recorrerá de 0 a 3 automáticamente. Imprime "OK" cuatro veces. Al final, cuando termina, n = 3 (depende de la implementación, algunos lenguajes lo dejan en 4, otros en 3).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2011.%20Pensamiento%20computacional.png" alt="Diagrama de flujos" width="350" height="auto"/>
    <p><em>Figura 11: Diagrama de flujos utilizando from/to loop. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

<br>

## 4.2.5 Analice un algoritmo que se presente como pseudocódigo

#### 📌Ejemplo de programación 7: Trace table

Tenemos el siguiente algoritmo:

```pseudocode
MAX = 10
SUM = 0
COUNT = 0

loop COUNT from 0 to MAX-6
    if COUNT = 0 AND MAX > 0 then
        output "Hello"
    else if COUNT > 2 then
        output "Go for it"
    else
        output "OK"
    end if
end loop

SUM = SUM + COUNT

output "Total = ", SUM
```

La siguiente tabla muestra la traza del algoritmo:

| MAX | SUM | COUNT | OUTPUT    | COMMENTS                             |
|-----|-----|-------|-----------|--------------------------------------|
| 10  | 0   | 0     | Hello     | COUNT = 0 AND MAX > 0 TRUE           |
| 10  | 0   | 1     | OK        | COUNT = 0 FALSE, COUNT > 2 FALSE     |
| 10  | 0   | 2     | OK        | COUNT = 0 FALSE, COUNT > 2 FALSE     |
| 10  | 0   | 3     | Go for it | COUNT > 2 TRUE                       |
| 10  | 0   | 4     | Go for it | COUNT > 2 TRUE                       |
| 10  | 5   | 5     | Total = 5 | Exit from loop, SUM = SUM + COUNT = 5 |

#### 📌Ejemplo de programación 8: Calcular resultado de un algoritmo

¿Cuál será el resultado del siguiente algoritmo?

```pseudocode
// Find the output of the following algorithm

DECLARE INTEGER MAX ← 10
DECLARE INTEGER SUM ← 0
DECLARE INTEGER COUNT ← 0

FOR COUNT ← 0 TO MAX - 4 DO
    SUM ← MAX - 4
    COUNT ← MAX - 3

    FOR SUM ← 3 TO 4 DO
        IF COUNT = 0 AND MAX > 0 THEN
            OUTPUT "Hello"
        ELSE IF COUNT < 4 THEN
            OUTPUT "Go for it"
        ELSE
            OUTPUT "OK"
        END IF
    END FOR
END FOR

SUM ← SUM + COUNT

OUTPUT "Total = ", SUM
OUTPUT "MAX = ", COUNT
```

El resultado sería: 

| Iteración COUNT | SUM (dentro del bucle) | OUTPUT | Comentarios                      |
|-----------------|-------------------------|--------|----------------------------------|
| 0               | 6                       | OK     | COUNT = 0 → no entra en if, else |
| 1               | 6                       | OK     | COUNT < 4 → imprime "Go for it"  |
| 2               | 6                       | OK     | COUNT < 4 → imprime "Go for it"  |
| 3               | 6                       | OK     | COUNT < 4 → imprime "Go for it"  |
| 4               | 6                       | OK     | COUNT >= 4 → imprime "OK"        |

**Resultado final:**  
- OUTPUT → OK, OK  
- Total = 13  
- MAX = 8

#### 📌Ejemplo de programación 9: Identifica el error

Encuentra el error en el siguiente algoritmo:

```pseudocode
// This program is supposed
// to print the common factors of two numbers
// Find the error!!

DECLARE INTEGER FIRST ← 14
DECLARE INTEGER SECOND ← 12

OUTPUT "Common factors of numbers ", FIRST, " and ", SECOND

FOR COUNT ← 1 TO SECOND DO
    IF (FIRST MOD COUNT = 0) OR (SECOND MOD COUNT = 0) THEN
        OUTPUT COUNT
    END IF
END FOR
```

Respuesta incorrecta: 

```pseudocode
Wrong Output: 
Common factors of numbers 14 and 12 
1
2
3
4
6
7
12 
```

Se debe realizar el siguiente cambio:

```pseudocode
IF (FIRST MOD COUNT = 0) OR (SECOND MOD COUNT = 0) THEN
```

por:

```pseudocode
IF (FIRST MOD COUNT = 0) AND (SECOND MOD COUNT = 0) THEN
```

Respuesta correcta:

```pseudocode
Correct Output: 
Common factors of numbers 14 and 12
 1
 2
```

#### 📌Ejemplo de programación 10: Identifica el error

El siguiente programa se supone que debe mostrar los elementos comunes que aparecen en dos arreglos. Contiene un error. Identifica este error.

```pseudocode
// This algorithm is supposed to
// compare two arrays and finds
// duplicates that appear in both arrays

DECLARE ARRAY1 = ["aa", "11", "34", "ff", "mn"]
DECLARE ARRAY2 = ["ff", "hh", "mn", "33", "34"]

OUTPUT "The following items appear in both arrays"

FOR A1 ← 0 TO 4 DO
    FOR A2 ← 0 TO 4 DO
        IF ARRAY1[A1] = ARRAY2[A2] THEN
            OUTPUT ARRAY2[A1]
        END IF
    END FOR
END FOR
```

Respuesta incorrecta: 

```pseudocode
The following appear in both arrays
mn
33
```

Se debe realizar el siguiente cambio:

```pseudocode
output ARRAY2[A1]
```

por:

```pseudocode
output ARRAY2[A2]
```

Respuesta correcta:

```pseudocode
The following appear in both arrays
34
ff
```

<br>

## 4.2.6 Elabore pseudocódigo para representar un algoritmo

#### 📌Ejemplo de programación 11: Ordenación ascendente o descendente

```pseudocode
// Algorithm that identifies if an array is sorted in ascending or descending order

I = 0
SORTEDA = 1      // Flag for ascending order
SORTEDD = 1      // Flag for descending order
SAMPLE = new Array()

// Input values
loop I from 0 to 4
    SAMPLE[I] = input("Enter the measurement")
end loop

// Check ascending order
loop I from 0 to 3
    if SAMPLE[I] > SAMPLE[I+1] then
        SORTEDA = 0
    end if
end loop

// Check descending order
loop I from 0 to 3
    if SAMPLE[I] < SAMPLE[I+1] then
        SORTEDD = 0
    end if
end loop

// Output array values
output "The array is:"
loop I from 0 to 4
    output SAMPLE[I]
end loop

// Results
if SORTEDA = 1 then
    output "The array is sorted in ASCENDING order"
else
    output "The array is not sorted in ASCENDING order"
end if

if SORTEDD = 1 then
    output "The array is sorted in DESCENDING order"
else
    output "The array is not sorted in DESCENDING order"
end if
```

Resultado:

```
User enters: 3, 5, 6, 4, 4. 

Output 1: 

The array is: 
3
5
6
4
4
The array is not sorted in ASCENDING order 
The array is not sorted in DESCENDING order

User enters: 6, 5, 3, 2, 1.

Output 2:

The array is:

6
5
3
2
1
The array is not sorted in ASCENDING order 
The array is sorted in DESCENDING order 

User enters: 2, 4, 78, 89, 99. 

Output 3: 

The array is:
 2
 4 
78 
89 
99 
The array is sorted in ASCENDING order 
The array is not sorted in DESCENDING order
```

#### 📌Ejemplo de programación 12: Creación de arreglo de 10 enteros aleatorio entre 0 y 9

```pseudocode
// Algorithm to build and display an array of ten random integers

Declare Integer n
Declare Integer RandomM[10]

// Fill the array with random numbers between 0 and 9
For n = 0 To 9
    Set RandomM[n] = random(10)      // generates a random integer 0–9
End For

// Print all elements of the array
For n = 0 to 9
    Output RandomM[n]
End For
Declare Integer n
```

<br>

## 4.2.7 Sugiera algoritmos adecuados para resolver un problema específico

La **eficiencia** de un algoritmo se refiere a la cantidad de recursos de la computadora requeridos para realizar sus funciones. Minimizar el uso de varios recursos como la CPU y la memoria de la computadora es muy importante.

La **corrección** de un algoritmo se refiere al grado en que el algoritmo satisface su especificación, está libre de fallas y cumple todos los objetivos establecidos durante la fase de diseño e implementación.

La **confiabilidad** se refiere a la capacidad del algoritmo para mantener un nivel de rendimiento predefinido y realizar todas las funciones requeridas bajo las condiciones establecidas, teniendo un largo tiempo medio entre fallas.

La **flexibilidad** de un algoritmo se refiere al esfuerzo requerido para modificar el algoritmo para otros propósitos distintos de aquellos para los que fue desarrollado inicialmente.

#### 📌Ejemplo de programación 13: Frecuencia de aparición de un número en un arreglo

```pseudocode
// PROGRAM TO CALCULATE THE FREQUENCY OF NUMBERS IN AN ARRAY

ARRAY = [-30, -13, 4, -3, -30, -3, -3, -3, -15]
SIZE = 9
COUNTS = new Array()

// Bubble Sort para ordenar el array
for I from 0 to SIZE-2
    for J from 0 to SIZE-2
        if ARRAY[J] > ARRAY[J+1] then
            TEMP = ARRAY[J]
            ARRAY[J] = ARRAY[J+1]
            ARRAY[J+1] = TEMP
        end if
    end for
end for

// Ahora el array está ordenado
PREVIOUS = ARRAY[0]
X = 1   // para contar frecuencia

for I from 1 to SIZE-1
    if ARRAY[I] = PREVIOUS then
        X = X + 1
        if I == SIZE-1 then
            output "Number:", ARRAY[I], "frequency:", X
        end if
    else
        output "Number:", ARRAY[I-1], "frequency:", X
        PREVIOUS = ARRAY[I]
        X = 1
        if I == SIZE-1 then
            output "Number:", ARRAY[I], "frequency:", X
        end if
    end if
end for
```
Resultado:

```pseudocode
Number: -30 frequency: 2
Number: -15 frequency: 1
Number: -13 frequency: 1
Number: -3 frequency: 4
Number: 4 frequency: 1
```

<br>

## 4.2.8 Deduzca la eficacia de un algoritmo en el contexto de su uso

La notación Big O es extremadamente útil cuando se analizan algoritmos, ya que es una medida de la eficiencia de un algoritmo. Cuando decimos que un algoritmo es O(n) lo que se quiere decir es que la tasa de crecimiento de las instrucciones en este algoritmo en particular se ejecutará **n** veces.

#### Algoritmo A
```pseudocode
// Un algoritmo que calcula la suma 1+2+3+...+n
// Complejidad: O(1)

SUM = 0
n = 5 // n como entrada
SUM = n * (n + 1) / 2
output "The SUM is: " + SUM
```

#### Algoritmo B
```pseudocode
// Un algoritmo que calcula la suma 1+2+3+...+n
// Complejidad: O(n)

I = 0
SUM = 0
n = 5 // n como entrada

loop I from 1 to n
    SUM = SUM + I
end loop

output "The SUM is: " + SUM
```

#### Algoritmo C
```pseudocode
// Un algoritmo que calcula la suma 1+2+3+...+n
// Complejidad: O(n^2)

I = 0
SUM = 0
n = 5 // n como entrada
m = 0

loop I from 1 to n
    loop m from 1 to I
        SUM = SUM + 1
    end loop
end loop

output "The SUM is: " + SUM
```

- **Algoritmo A (O(1)):** Usa una fórmula matemática directa:
  
SUM = 𝑛(𝑛+1)/2​

No requiere bucles, solo una operación, por lo que es muy eficiente.

- **Algoritmo B (O(𝑛)):** Usa un bucle desde 1 hasta 𝑛, sumando cada número. El tiempo de ejecución crece proporcionalmente al tamaño de 𝑛.

- **Algoritmo C (O(𝑛²)):** Usa dos bucles anidados: el primero de 1 a 𝑛 y dentro otro de 1 a i. Esto genera muchas más operaciones, haciendo que el tiempo de ejecución crezca proporcionalmente a 𝑛².

<br>

## 4.2.9 Determine el número de veces que se ejecutará una instrucción en un algoritmo para unos datos de entrada concretos

#### 📌Ejemplo de programación 14: Cálculo del número de iteraciones

```pseudocode
Declare Integer a
Declare Integer b

Input a
Input b
If a > b Then
    Set a = b - 3
    While a < b
        Display "loop 1"
        Set b = a * 2
        While b > 7
            Set b = a - 2
            Display "loop 3"
        End While
        Display "loop 2"
    End While
End If
```

Q1. ¿Qué va a ser la salida cuando a = 10 y b = 4?
A1. El programa nunca terminará. Será un bucle infinito.

Q2. ¿Qué va a ser la salida cuando a = 4 y b = 10?
A2. No hay salida.

Q3. ¿Qué va a ser la salida cuando a = 10 y b = 9?
A3. Salida: loop1 loop2 loop3

Q4. ¿Qué va a ser la salida cuando a = 10 y b = 0?
A4. Salida: loop1 loop2

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2012.%20Pensamiento%20computacional.png" alt="Diagrama de flujos" width="550" height="auto"/>
    <p><em>Figura 12: Diagrama de flujos del ejemplo de programación 14. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

