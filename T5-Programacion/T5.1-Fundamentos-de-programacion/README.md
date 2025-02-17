<h1 align="center">Fundamentos de programación
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:
[1. Introducción a la algorítmica](#1-los-sistemas-de-información)  
  - [1.1. Paradigmas de programación](#11-paradigmas-de-programación)
[2. Los lenguajes informáticos](#2-los-lenguajes-de-programación)
  - [2.1. Características esenciales de un lenguaje informático](#21-características-esenciales-de-un-lenguaje-informático)


## 1. Introducción a la algorítmica

La **algoritmia** se ocupa del diseño y análisis de **algoritmos**, que son secuencias finitas y ordenadas de pasos que resuelven un problema o realizan una tarea. Estos algoritmos son **las instrucciones que el computador debe seguir** para realizar sus operaciones fundamentales.

> [!IMPORTANT]  
> La **relación** entre las operaciones fundamentales de un computador y la algoritmia es muy estrecha, ya que ambos conceptos se complementan y dependen entre sí para resolver problemas computacionales.

Las operaciones fundamentales de una computadora son: 

1. **Entrada →** El algoritmo define cómo y qué datos debe recibir el computador.
2. **Almacenamiento →** El algoritmo determina qué datos deben guardarse y cómo deben organizarse.
3. **Procesamiento →** El algoritmo describe los cálculos y operaciones lógicas que deben realizarse sobre esos datos.
4. **Salida →** El algoritmo establece qué resultados se deben mostrar y de qué manera.
5. **Comunicación →** Algunos algoritmos implican intercambiar datos con otros sistemas.

### 1.1. Paradigmas de programación 
- **Paradigma imperativo:** es el más clásico y se basa en **dar órdenes al computador** sobre cómo debe realizar cada paso de una tarea. Se basa en secuencias de instrucciones, alteración de estados y estructuras de control (bucles, condicionales). Describe el **"cómo"** se resuelve el problema.
- **Paradigma declarativo:** en este enfoque, se describe el **"qué"** se quiere obtener, en lugar de indicar paso a paso cómo hacerlo. Los cálculos se basan en relaciones lógicas y expresiones.
- **Paradigma Orientado a Objetos (OOP):** organiza el código en **objetos**, que son entidades que combinan **datos (atributos)** y **comportamientos (métodos)**.
- **Paradigma funcional:** se basa en la idea de que las funciones son entidades de primera clase. Las funciones no modifican estados, sino que devuelven resultados.

## 2. Los lenguajes de programación
Un lenguaje informático es un sistema estructurado de comunicación utilizado para dar instrucciones a un ordenador. A diferencia de los lenguajes naturales que utilizamos los humanos, los lenguajes informáticos deben ser precisos y seguir unas reglas estrictas para que el ordenador pueda interpretar y ejecutar correctamente las instrucciones. Las principales características esenciales de un lenguaje informático son las siguientes:

#### 1. Vocabulario fijo
Un lenguaje de programación dispone de un conjunto limitado y predefinido de palabras reservadas y símbolos que forman el vocabulario del lenguaje. Estas palabras y símbolos tienen funciones específicas y no pueden usarse con otro significado. Por ejemplo, en Python, algunas palabras reservadas son if, else, while, def, import, entre otras.

#### 2. Significado inequívoco
Cada instrucción en un lenguaje informático tiene un único significado, es decir, no admite interpretaciones ambiguas. Un mismo código producirá siempre el mismo resultado si se ejecuta bajo las mismas condiciones. Esta precisión es fundamental para evitar errores e inconsistencias en los programas.

#### 3. Gramática y sintaxis sistemáticas
Un lenguaje informático tiene un conjunto de reglas conocido como sintaxis que determina cómo deben combinarse las palabras y símbolos del vocabulario para formar instrucciones válidas. Si se escribe un código que no respeta estas reglas, el programa no se ejecutará y el compilador o intérprete generará un error de sintaxis. Por ejemplo, en Python:

Correcto:
```python
print("Hola, mundo!")
```

Incorrecto (falta de comillas):
```python
print(Hola, mundo!)
```
#### 4. Precisión y formalidad
Los lenguajes informáticos se caracterizan por su formalidad y exactitud. Cada símbolo, cada espacio y cada signo de puntuación pueden afectar el comportamiento del programa. A diferencia del lenguaje humano, en programación no se pueden interpretar las intenciones; el ordenador ejecuta exactamente lo que se le indica.

#### 5. Evolución y estandarización
Los lenguajes informáticos evolucionan con el tiempo, pero su desarrollo sigue procesos de estandarización para garantizar que los programas escritos en una versión sean compatibles y comprensibles en el futuro. Por ejemplo, Python ha evolucionado desde Python 2 a Python 3, con cambios en la sintaxis y funciones.
