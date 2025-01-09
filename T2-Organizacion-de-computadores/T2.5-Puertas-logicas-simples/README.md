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

#### Ejemplos:

##### Ejemplo 1:

Un sistema de riego automático funciona si está activado manualmente o si el sensor de humedad detecta que el suelo está seco.

Consideramos las siguientes entradas: 
- Entrada A: Se activa manualmente.
- Entrada B: Detecta humedad el sensor.

Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

**Salida (Sistema de riego activado)** = (A OR B)

| A         | B          | Salida      |
|-----------|------------|-------------|
| 0         | 0          | 0           |
| 0         | 1          | 1           |
| 1         | 0          | 1           |
| 1         | 1          | 1           |

##### Ejemplo 2:

Un sistema de seguridad activa la alarma solo si ambas puertas de entrada y ventana están abiertas al mismo tiempo.

Consideramos las siguientes entradas: 
- Entrada A: Puerta de entrada abierta.
- Entrada B: Ventana abierta.

 Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

 **Salida (Sistema de alarmas activado)** = A AND B

| A         | B          | Salida      |
|-----------|------------|-------------|
| 0         | 0          | 0           |
| 0         | 1          | 0           |
| 1         | 0          | 0           |
| 1         | 1          | 1           |

##### Ejemplo 3:

Un sistema de seguridad activa la alarma si no se cumplen ambas condiciones: la puerta está cerrada y la ventana está cerrada.

Consideramos las siguientes entradas: 
- Entrada A: Puerta cerrada.
- Entrada B: Ventana cerrada.

 Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

**Salida (Alarmas activada)** = NOT(A AND B)

| A                   | B                   | A AND B | NAND                    |
|---------------------|---------------------|---------|-------------------------|
| 0                   | 0                   | 0       | 1                       |
| 0                   | 1                   | 0       | 1                       |
| 1                   | 0                   | 0       | 1                       |
| 1                   | 1                   | 1       | 0                       |


##### Ejemplo 4:

Un sistema de ahorro de energía apaga las luces si ningún interruptor está activado.

Consideramos las siguientes entradas: 
- Entrada A: Interruptor 1 activado.
- Entrada B: Interruptor 2 activado.

Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

**Salida (Luces apagadas)** = NOT(A OR B)

| A                   | B                   | A OR B  | NOR                     |
|---------------------|---------------------|---------|-------------------------|
| 0                   | 0                   | 0       | 1                       |
| 0                   | 1                   | 1       | 0                       |
| 1                   | 0                   | 1       | 0                       |
| 1                   | 1                   | 1       | 0                       |
  
##### Ejemplo 5:

Un sistema de encendido alternativo activa un dispositivo si exactamente uno de los botones está presionado.

Consideramos las siguientes entradas: 
- Entrada A: Botón 1 activado.
- Entrada B: Botón 2 activado.

Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

**Salida (Dispositivo activado)** = A XOR B

| A                   | B                   |  XOR                     |
|---------------------|---------------------| -------------------------|
| 0                   | 0                   |  0                       |
| 0                   | 1                   |  1                       |
| 1                   | 0                   |  1                       |
| 1                   | 1                   |  0                       |
  

##### Ejemplo 6:

Una alarma de seguridad suena si la puerta está abierta y no hay luz en la habitación.

Consideramos las siguientes entradas: 
- Entrada A: Puerta abierta.
- Entrada B: Luz encendida.

 Esta lógica la podemos interpretar como una combinación de operaciones booleanas:

  **Salida (Alarma de seguridad suena)** = A AND (NOT B)

| A         | B          | NOT B       | Salida      |
|-----------|------------|-------------|-------------|
| 0         | 0          | 1           | 0           |
| 0         | 1          | 0           | 0           |
| 1         | 0          | 1           | 1           |
| 1         | 1          | 0           | 0           |

##### Ejemplo 3:

Un sistema de calefacción se enciende si hace frío y alguien esta en casa o si se activa manualmente.

O, dicho de otra manera: Un sistema de calefacción se enciende si hace frío (A) y si alguien esta en casa (B) o si se activa manualmente (C).

Consideramos las siguientes entradas: 
- Entrada A: Hace frío.
- Entrada B: Alguien en casa.
- Entrada C: Se activa manualmente.

Esta lógica la podemos interpretar como una combinación de operaciones booleanas: 

**Salida (Sistema de calefacción se enciende)** = (A AND B) OR C

| A         | B          | (A AND B)   | C           | Salida        |
|-----------|------------|-------------|-------------|---------------|
| 0         | 0          | 0           | 0           | 0             |
| 0         | 0          | 0           | 1           | 1             |
| 0         | 1          | 0           | 0           | 0             |
| 0         | 1          | 0           | 1           | 1             |
| 1         | 0          | 0           | 0           | 0             |
| 1         | 0          | 0           | 1           | 1             |
| 1         | 1          | 1           | 0           | 1             |
| 1         | 1          | 1           | 1           | 1             |



