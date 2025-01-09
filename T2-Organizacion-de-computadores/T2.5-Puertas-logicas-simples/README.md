<h1 align="center">Puertas lógicas simples
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:
[1. Introducción a las puertas lógicas](#1-introducción-a-las-puertas-lógicas)  

[2. Representación de funciones lógicas](#2-representación-de-funciones-lógicas)  
  - [2.1. Definición de operadores booleanos](#21-definición-de-operadores-booleanos)  
  - [2.2. Tablas de verdad](#22-tablas-de-verdad)  

## 1. Introducción a las puertas lógicas

Las **puertas lógicas** son los componentes básicos de los circuitos digitales y permiten realizar operaciones fundamentales del álgebra de Boole. Estas operaciones son esenciales para procesar información binaria en dispositivos electrónicos como ordenadores, calculadoras y sistemas automáticos. 

A través del uso de puertas lógicas como AND, OR, NOT, entre otras, es posible diseñar y analizar circuitos que realicen tareas específicas basadas en combinaciones de entradas binarias.

## 2. Representación de funciones lógicas

### 2.1. Definición de operadores booleanos

Los **operadores booleanos** son herramientas fundamentales del álgebra de Boole. A continuación, se presentan los operadores más comunes:

1. **NOT** (Negación): Produce el valor opuesto de una entrada. Si la entrada es `1`, el resultado es `0` y viceversa.

| Entrada A | NOT A |
|-----------|-------|
| 0         | 1     |
| 1         | 0     |

2. **AND** (Conjunción): Devuelve `1` si todas las entradas son `1`. Si alguna es `0`, el resultado es `0`.

| Entrada A | Entrada B | A AND B |
|-----------|-----------|---------|
| 0         | 0         | 0       |
| 0         | 1         | 0       |
| 1         | 0         | 0       |
| 1         | 1         | 1       |

4. **OR** (Disyunción): Devuelve `1` si al menos una de las entradas es `1`. Solo es `0` si todas las entradas son `0`.

| Entrada A | Entrada B | A OR B |
|-----------|-----------|--------|
| 0         | 0         | 0      |
| 0         | 1         | 1      |
| 1         | 0         | 1      |
| 1         | 1         | 1      |

6. **NAND** (Negación de AND): Devuelve el valor opuesto al de la operación AND.

| Entrada A | Entrada B | A NAND B |
|-----------|-----------|----------|
| 0         | 0         | 1        |
| 0         | 1         | 1        |
| 1         | 0         | 1        |
| 1         | 1         | 0        |

8. **NOR** (Negación de OR): Devuelve el valor opuesto al de la operación OR.

| Entrada A | Entrada B | A NOR B |
|-----------|-----------|---------|
| 0         | 0         | 1       |
| 0         | 1         | 0       |
| 1         | 0         | 0       |
| 1         | 1         | 0       |

10. **XOR** (Disyunción exclusiva): Devuelve `1` si exactamente una de las entradas es `1`. Si todas las entradas son iguales, devuelve `0`.

| Entrada A | Entrada B | A XOR B |
|-----------|-----------|---------|
| 0         | 0         | 0       |
| 0         | 1         | 1       |
| 1         | 0         | 1       |
| 1         | 1         | 0       |

### 2.2. Tablas de verdad

Las tablas de verdad permiten visualizar los resultados de los operadores booleanos para todas las combinaciones posibles de entradas. A continuación, se muestra un ejemplo para los operadores definidos:

| Entrada A | Entrada B | NOT A | NOT B | A AND B | A OR B | A NAND B | A NOR B | A XOR B |
|-----------|-----------|--------|--------|---------|---------|----------|---------|---------|
| 0         | 0         | 1      | 1      | 0       | 0       | 1        | 1       | 0       |
| 0         | 1         | 1      | 0      | 0       | 1       | 1        | 0       | 1       |
| 1         | 0         | 0      | 1      | 0       | 1       | 1        | 0       | 1       |
| 1         | 1         | 0      | 0      | 1       | 1       | 0        | 0       | 0       |

#### Ejemplo:
Consideremos el siguiente problema:
- María no irá a la escuela si hace frío **y** llueve **o** no ha hecho sus deberes.
  - Entrada A: Hace frío.
  - Entrada B: Llueve.
  - Entrada C: Ha hecho sus deberes.
 
O, dicho de otra manera: María no irá a la escuela si hace frío (A) y llueve (B) o no ha hecho sus deberes (NOT C). 

Esta lógica la podemos interpretar como una combinación de operaciones booleanas: 

**Salida (No va a la escuela)** = (A AND B) OR (NOT C)

| Frío (A) | Llueve (B) | Deberes (C) | Salida (No va a la escuela)  |
|-----------|------------|-------------|-----------------------------|
| 0         | 0          | 0           | 1                           |
| 0         | 0          | 1           | 1                           |
| 0         | 1          | 0           | 0                           |
| 0         | 1          | 1           | 1                           |
| 1         | 0          | 0           | 0                           |
| 1         | 0          | 1           | 1                           |
| 1         | 1          | 0           | 0                           |
| 1         | 1          | 1           | 1                           |

Si nos fijamos en la primera combiación: 
```
Salida = (A AND B) OR (NOT C)
Salida = (0 AND 0) OR 1
Salida = 0 OR 1
Salida = 1
```

