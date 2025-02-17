<h1 align="center">Guía básica de Python
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:

[1. Sintaxis básica y conceptos fundamentales](#1-sintaxis-básica-y-conceptos-fundamentales)  
  - [1.1. Escritura e indentación](#11-escritura-e-indentación)  
  - [1.2. Comentarios](#12-comentarios)  
  - [1.3. Tipos de datos básicos](#13-tipos-de-datos-básicos)  
    - [1.3.1. Enteros (int)](#131-enteros-int)  
    - [1.3.2. Decimales (float)](#132-decimales-float)  
    - [1.3.3. Cadenas de texto (str)](#133-cadenas-de-texto-str)  
    - [1.3.4. Booleanos (bool)](#134-booleanos-bool)  

[2. Variables y constantes](#2-variables-y-constantes)  
  - [2.1. Definición y uso de variables](#21-definición-y-uso-de-variables)  
  - [2.2. Definición y uso de constantes](#22-definición-y-uso-de-constantes)  

[3. Operadores](#3-operadores)  
  - [3.1. Operadores aritméticos](#31-operadores-aritméticos)  
  - [3.2. Operadores de comparación](#32-operadores-de-comparación)  
  - [3.3. Operadores lógicos](#33-operadores-lógicos)  

[4. Entrada y salida de datos](#4-entrada-y-salida-de-datos)  
  - [4.1. Función print()](#41-función-print)  
  - [4.2. Función input()](#42-función-input)  

[5. Estructuras de control](#5-estructuras-de-control)  
  - [5.1. Condicionales](#51-condicionales)  
  - [5.2. Bucles](#52-bucles)  
    - [5.2.1. Bucle while](#521-bucle-while)  
    - [5.2.2. Bucle for](#522-bucle-for)  
  - [5.3. Sentencias break y continue](#53-sentencias-break-y-continue)  

[6. Funciones](#6-funciones)  
  - [6.1. Definición de funciones](#61-definición-de-funciones)  
  - [6.2. Parámetros y argumentos](#62-parámetros-y-argumentos)  
  - [6.3. Retorno de valores](#63-retorno-de-valores)  
  - [6.4. Ventajas del uso de funciones](#64-ventajas-del-uso-de-funciones)  

[7. Colecciones básicas](#7-colecciones-básicas)  
  - [7.1. Listas (list)](#71-listas-list)  
  - [7.2. Tuplas (tuple)](#72-tuplas-tuple)  
  - [7.3. Diccionarios (dict)](#73-diccionarios-dict)  


## 1. Sintaxis básica y conceptos fundamentales

### 1.1. Escritura e indentación

Python es un lenguaje que se caracteriza por su sintaxis clara y legible. Una de sus peculiaridades es que utiliza la **indentación** (espacios en blanco al inicio de la línea) para definir bloques de código, en lugar de llaves `{}` como en otros lenguajes.

Cada vez que se crea una estructura como un condicional, un bucle o una función, el bloque de instrucciones que depende de esa estructura debe estar indentado con la misma cantidad de espacios. Por convención, se utilizan **4 espacios** para cada nivel de indentación.

Ejemplo:
```python
if True:
    print("Este bloque está indentado")
    print("Forma parte del if")
print("Este ya no pertenece al if")
```

Si la indentación no es correcta, se producirá un error de sintaxis.

### 1.2. Comentarios

Los comentarios son líneas de texto que el intérprete de Python ignora. Sirven para explicar el código y mejorar su legibilidad. En Python, los comentarios se escriben con el símbolo `#`.

Ejemplo:
```python
# Este es un comentario
print("Hola, mundo")  # Esto también es un comentario
```

Para comentarios multilínea, se pueden utilizar triples comillas (`"""` o `'''`), aunque se suele usar más para documentación.

Ejemplo:
```python
"""
Esto es un comentario de varias líneas.
Suele emplearse para documentar funciones y módulos.
"""
```

### 1.3. Tipos de datos básicos

Python maneja diferentes tipos de datos. Los más básicos son:

#### 1.3.1. Enteros (int)

Son números enteros, positivos o negativos, sin decimales.

Ejemplo:
```python
edad = 25
puntuacion = -10
```

#### 1.3.2. Decimales (float)

Son números con parte decimal. En Python, los decimales se representan con un punto `.`.

Ejemplo:
```python
altura = 1.75
precio = -99.99
```

#### 1.3.3. Cadenas de texto (str)

Representan secuencias de caracteres. En Python, se definen usando comillas simples `'` o dobles `"`.

Ejemplo:
```python
nombre = 'Juan'
apellido = "Pérez"
```

Operaciones básicas con cadenas:
```python
saludo = "Hola" + " " + nombre
print(saludo)  # Salida: Hola Juan
```

#### 1.3.4. Booleanos (bool)

Son valores lógicos que solo pueden tomar dos valores: `True` (verdadero) y `False` (falso).

Ejemplo:
```python
es_mayor = True
esta_lloviendo = False
```

Los valores booleanos son útiles para tomar decisiones en el código mediante condicionales:
```python
if es_mayor:
    print("Es mayor de edad")
else:
    print("Es menor de edad")
```

## 2. Variables y constantes

### 2.1. Definición y uso de variables

Una **variable** es un espacio en memoria que se utiliza para almacenar un valor que puede cambiar durante la ejecución del programa. En Python, no es necesario especificar el tipo de dato, ya que se determina automáticamente al asignar un valor.

#### Asignación de variables
```python
edad = 25
nombre = "Juan"
precio = 19.99
es_mayor = True
```

#### Reasignación de valores
```python
edad = 30
nombre = "María"
```

#### Buenas prácticas
- Usar nombres descriptivos.
- Seguir la convención de minúsculas y guiones bajos (snake_case): `nombre_usuario`.

### 2.2. Definición y uso de constantes

Una **constante** es un valor que no debe cambiar durante la ejecución del programa. Aunque Python no tiene un tipo específico para constantes, por convención se escriben en mayúsculas.

#### Declaración de constantes
```python
PI = 3.1416
IVA = 0.21
```

Aunque nada impide modificar una constante, por convención no se debe hacer.

```python
PI = 3.15  # Esto es posible, pero no recomendable
```

## 3. Operadores

### 3.1. Operadores aritméticos

Los operadores aritméticos se utilizan para realizar operaciones matemáticas:

| Operador | Descripción | Ejemplo | Resultado |
|----------|--------------|---------|------------|
| `+` | Suma | `3 + 2` | `5` |
| `-` | Resta | `5 - 3` | `2` |
| `*` | Multiplicación | `4 * 2` | `8` |
| `/` | División | `10 / 2` | `5.0` |
| `//` | División entera | `10 // 3` | `3` |
| `%` | Módulo (resto) | `10 % 3` | `1` |
| `**` | Potencia | `2 ** 3` | `8` |

Ejemplo en Python:
```python
suma = 3 + 2
resta = 5 - 3
multiplicacion = 4 * 2
division = 10 / 2
division_entera = 10 // 3
modulo = 10 % 3
potencia = 2 ** 3
```

### 3.2. Operadores de comparación

Los operadores de comparación se utilizan para comparar dos valores y devuelven un valor booleano (`True` o `False`):

| Operador | Descripción | Ejemplo | Resultado |
|----------|--------------|---------|------------|
| `==` | Igual que | `5 == 5` | `True` |
| `!=` | Diferente de | `5 != 3` | `True` |
| `<` | Menor que | `3 < 5` | `True` |
| `>` | Mayor que | `5 > 3` | `True` |
| `<=` | Menor o igual que | `3 <= 3` | `True` |
| `>=` | Mayor o igual que | `5 >= 4` | `True` |

Ejemplo en Python:
```python
es_igual = 5 == 5
es_diferente = 5 != 3
menor_que = 3 < 5
mayor_que = 5 > 3
menor_igual = 3 <= 3
mayor_igual = 5 >= 4
```

### 3.3. Operadores lógicos

Los operadores lógicos se utilizan para combinar expresiones condicionales:

| Operador | Descripción | Ejemplo | Resultado |
|----------|--------------|---------|------------|
| `and` | Y lógico | `True and False` | `False` |
| `or` | O lógico | `True or False` | `True` |
| `not` | Negación lógica | `not True` | `False` |

Ejemplo en Python:
```python
resultado_and = True and False
resultado_or = True or False
resultado_not = not True
```

Estos operadores se utilizan frecuentemente en estructuras condicionales:
```python
edad = 20
es_mayor = edad >= 18
tiene_permiso = True

if es_mayor and tiene_permiso:
    print("Puede entrar")
else:
    print("No puede entrar")
```

## 4. Entrada y salida de datos

### 4.1. Función print()

La función `print()` se utiliza para mostrar información en la pantalla. Es una de las funciones más básicas y esenciales en Python, ya que permite ver el resultado de las operaciones y el estado de las variables durante la ejecución del programa.

#### Sintaxis
```python
print(valor1, valor2, ..., sep=' ', end='\n')
```
- `valor1, valor2, ...`: Son los valores que se quieren mostrar. Pueden ser variables, textos (entre comillas), números, etc.
- `sep=' '` (opcional): Define el separador entre los valores. Por defecto es un espacio.
- `end='\n'` (opcional): Define qué se mostrará al final de la línea. Por defecto es un salto de línea.

#### Ejemplos
```python
print("Hola, mundo")
print("El resultado es", 5 + 3)
print("Python", "es", "fácil", sep='-')
print("Este es el final", end='.')
```

Salida:
```
Hola, mundo
El resultado es 8
Python-es-fácil
Este es el final.
```

### 4.2. Función input()

La función `input()` se utiliza para pedir al usuario que introduzca datos por teclado. Siempre devuelve el valor introducido como una cadena de texto (`str`), por lo que es necesario convertirlo al tipo adecuado si se quiere trabajar con números.

#### Sintaxis
```python
variable = input(mensaje_opcional)
```
- `mensaje_opcional`: Es un texto que se mostrará al usuario como indicación de qué debe introducir.

#### Ejemplos
```python
nombre = input("¿Cómo te llamas? ")
edad = input("¿Cuántos años tienes? ")
print("Hola", nombre, ", tienes", edad, "años")
```

Entrada:
```
¿Cómo te llamas? Juan
¿Cuántos años tienes? 25
```

Salida:
```
Hola Juan, tienes 25 años
```

#### Conversión de tipos
Si se necesita que el valor introducido sea un número entero (`int`) o decimal (`float`), se debe convertir:

```python
edad = int(input("Introduce tu edad: "))
peso = float(input("Introduce tu peso: "))
print("Edad:", edad, "Peso:", peso)
```

Entrada:
```
Introduce tu edad: 30
Introduce tu peso: 70.5
```

Salida:
```
Edad: 30 Peso: 70.5
```

## 5. Estructuras de control

### 5.1. Condicionales

Las condicionales permiten ejecutar diferentes bloques de código dependiendo de si se cumple una condición o no.

#### Sintaxis básica:
```python
if condicion:
    # Bloque de código si se cumple la condición
elif otra_condicion:
    # Bloque de código si se cumple otra_condicion
else:
    # Bloque de código si no se cumple ninguna condición
```

#### Ejemplo:
```python
edad = int(input("Introduce tu edad: "))
if edad >= 18:
    print("Eres mayor de edad")
elif edad >= 16:
    print("Tienes entre 16 y 18 años")
else:
    print("Eres menor de edad")
```

### 5.2. Bucles

#### 5.2.1. Bucle while

El bucle `while` se ejecuta mientras se cumpla una condición.

#### Sintaxis:
```python
while condicion:
    # Bloque de código que se repite mientras la condición sea verdadera
```

#### Ejemplo:
```python
contador = 0
while contador < 5:
    print("Contador:", contador)
    contador += 1
```

#### 5.2.2. Bucle for

El bucle `for` se utiliza para iterar sobre una secuencia (como una lista o un rango de valores).

#### Sintaxis:
```python
for variable in secuencia:
    # Bloque de código que se repite por cada elemento de la secuencia
```

#### Ejemplo con `range()`:
```python
for i in range(5):
    print("Valor de i:", i)
```

#### Ejemplo recorriendo una lista:
```python
frutas = ["manzana", "banana", "naranja"]
for fruta in frutas:
    print("Fruta:", fruta)
```

### 5.3. Sentencias break y continue

- `break`: Interrumpe el bucle y sale de él.
- `continue`: Salta a la siguiente iteración del bucle, omitiendo el código restante.

#### Ejemplo con `break`:
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

Salida:
```
0
1
2
3
4
```

#### Ejemplo con `continue`:
```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

Salida:
```
0
1
3
4
```

## 6. Funciones

### 6.1. Definición de funciones

Una función es un bloque de código que realiza una tarea específica. Permite reutilizar código y dividir el programa en partes más pequeñas y manejables.

#### Sintaxis básica:
```python
def nombre_funcion():
    # Cuerpo de la función
    print("Hola desde la función")
```

#### Llamar a una función:
```python
nombre_funcion()
```

#### Ejemplo:
```python
def saludar():
    print("Hola, bienvenido a Python")

saludar()
```

### 6.2. Parámetros y argumentos

Las funciones pueden recibir valores de entrada llamados parámetros. Estos parámetros permiten personalizar el comportamiento de la función.

#### Sintaxis con parámetros:
```python
def saludar(nombre):
    print("Hola", nombre)
```

#### Llamar a la función con un argumento:
```python
saludar("Ana")
```

#### Parámetros múltiples:
```python
def sumar(a, b):
    print("La suma es:", a + b)

sumar(3, 5)
```

### 6.3. Retorno de valores

Las funciones pueden devolver un valor usando la palabra clave `return`.

#### Ejemplo:
```python
def multiplicar(a, b):
    resultado = a * b
    return resultado

producto = multiplicar(4, 3)
print("El producto es:", producto)
```

### 6.4. Ventajas del uso de funciones

- **Reutilización de código:** Permite definir el código una vez y reutilizarlo múltiples veces.
- **Modularidad:** Divide el programa en partes más pequeñas y fáciles de entender.
- **Legibilidad:** Facilita la lectura y el mantenimiento del código.
- **Evita repeticiones:** Reduce la duplicación de código, lo que minimiza errores.

#### Ejemplo práctico combinando todo:
```python
def calcular_area_rectangulo(base, altura):
    area = base * altura
    return area

resultado = calcular_area_rectangulo(5, 10)
print("El área del rectángulo es:", resultado)
```

## 7. Colecciones básicas

### 7.1. Listas (list)

Una lista es una colección ordenada y mutable que permite almacenar varios elementos. Los elementos pueden ser de diferentes tipos de datos.

#### Sintaxis:
```python
mi_lista = [1, 2, 3, "hola", True]
```

#### Acceso a elementos:
```python
print(mi_lista[0])  # Accede al primer elemento
print(mi_lista[-1])  # Accede al último elemento
```

#### Modificar elementos:
```python
mi_lista[1] = 42
```

#### Métodos comunes:
```python
mi_lista.append(4)  # Añadir elemento al final
mi_lista.remove(3)  # Eliminar elemento por valor
mi_lista.pop()  # Eliminar el último elemento
mi_lista.insert(1, "nuevo")  # Insertar elemento en posición específica
```

#### Recorrer una lista:
```python
for elemento in mi_lista:
    print(elemento)
```

### 7.2. Tuplas (tuple)

Una tupla es una colección ordenada e inmutable. Sus elementos no pueden ser modificados después de su creación.

#### Sintaxis:
```python
mi_tupla = (1, 2, 3, "hola", True)
```

#### Acceso a elementos:
```python
print(mi_tupla[0])
print(mi_tupla[-1])
```

#### Recorrer una tupla:
```python
for elemento in mi_tupla:
    print(elemento)
```

#### Conversión de tupla a lista:
```python
mi_lista = list(mi_tupla)
```

### 7.3. Diccionarios (dict)

Un diccionario es una colección no ordenada que almacena pares clave-valor. Las claves son únicas y permiten acceder rápidamente a los valores asociados.

#### Sintaxis:
```python
mi_diccionario = {"nombre": "Ana", "edad": 25, "ciudad": "Madrid"}
```

#### Acceso a valores:
```python
print(mi_diccionario["nombre"])
```

#### Modificar valores:
```python
mi_diccionario["edad"] = 26
```

#### Añadir nuevas claves:
```python
mi_diccionario["profesion"] = "Ingeniera"
```

#### Métodos comunes:
```python
mi_diccionario.keys()  # Devuelve las claves
mi_diccionario.values()  # Devuelve los valores
mi_diccionario.items()  # Devuelve los pares clave-valor
```

#### Recorrer un diccionario:
```python
for clave, valor in mi_diccionario.items():
    print(clave, ":", valor)
```
