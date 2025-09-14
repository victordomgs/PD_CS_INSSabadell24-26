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
