<h1 align="center">4.2. Relación entre pensamiento computacional y diseño de programas
<div align="center">

</div>

## Contenido:

- [4.2.1. Algoritmos en matrices](#421-algoritmos-en-matrices)
- [4.2.2. Operaciones estándares de las colecciones](#422-operaciones-estándares-de-las-colecciones)
- [4.2.3. Algoritmos para problemas concretos](#423-algoritmos-para-problemas-concretos)
- [4.2.4. Algoritmos presentados en diagramas de flujos](#424-algoritmos-presentados-en-diagramas-de-flujos)
- [4.2.5. Algoritmos presentados en pseudocódigo](#425-algoritmos-presentados-en-pseudocódigo)
- [4.2.6. Elaboración de pseudocódigo](#426-elaboración-de-pseudocódigo)
- [4.2.7. Algoritmos adecuados para problemas específicos](#427-algoritmos-presentados-en-diagramas-de-flujos)
- [4.2.8. Eficacia de un algoritmo según el contexto](#428-eficacia-de-un-algoritmo-según-el-contexto)
- [4.2.9. Determinación del número de iteraciones según las entradas](#428-determinación-del-número-de-iteraciones-según-las-entradas)

---

## 4.2.1. Algoritmos en matrices

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

#### Ejemplo de programación 1: Uso de un arreglo (arreglo de números)

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

#### Ejemplo de programación 2: Arreglo bidimensional (temperaturas)

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
