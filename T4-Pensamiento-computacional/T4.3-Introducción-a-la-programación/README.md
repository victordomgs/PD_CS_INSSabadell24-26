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
- [4.3.13. Elaboración de algoritmos usando subprogramas predefinidios, matrices unidimensionales y colecciones](#4313-elaboración-de-algoritmos-usando-subprogramas predefinidos-matrices-unidimensionales-y-colecciones)

---

## 4.3.1. Operaciones fundamentales de un computador

Un ordenador puede realizar algunas **operaciones fundamentales**. El siguiente ejemplo simplificado se utiliza para ilustrar algunas operaciones básicas. Supongamos que un número está almacenado como una cadena de bits en la ubicación de memoria 20 y otro número está almacenado como una cadena de bits en la ubicación de memoria 30. Una instrucción LOAD 20 se transfiere desde la RAM a la Unidad de Control (CU). El contenido de la ubicación de memoria 20 se carga (recupera de la memoria) en la Unidad Aritmético-Lógica (ALU). Se obtiene una segunda instrucción. La CU toma la instrucción ADD 30, carga el contenido de la ubicación de memoria 30 en la ALU y lo suma al número que ya está allí (el número de la ubicación de memoria 20). Una instrucción final STORE 50 se utiliza para almacenar la salida en la ubicación de memoria 50.

Una variación de este fragmento simple de código de máquina sería usar una instrucción que COMPARE (<, >, =) el contenido de la ubicación de memoria 20 con el contenido de la ubicación de memoria 40 y cambie el curso del programa de acuerdo con el resultado de la comparación. Las instrucciones condicionales y las operaciones básicas del álgebra booleana (AND, OR, XOR, NOT) son fundamentales para el desarrollo de programas útiles.
