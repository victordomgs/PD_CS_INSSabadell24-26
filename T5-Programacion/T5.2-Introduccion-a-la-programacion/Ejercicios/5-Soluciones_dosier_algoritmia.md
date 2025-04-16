### 1. Sobre los siguientes códigos: 

#### a) 

El bucle `for` se ejecuta con `i` desde 1 hasta 5 (incluido), es decir, 5 veces. En cada iteración se suma 2 al contador.

Entonces:
- Iteración 1: contador = 0 + 2 = 2
- Iteración 2: contador = 2 + 2 = 4
- Iteración 3: contador = 4 + 2 = 6
- Iteración 4: contador = 6 + 2 = 8
- Iteración 5: contador = 8 + 2 = 10

**Resultado:** 10

#### b) 

El programa suma solo los números pares entre 1 y 5:

- i = 1 → no entra
- i = 2 → suma = 0 + 2 = 2
- i = 3 → no entra
- i = 4 → suma = 2 + 4 = 6
- i = 5 → no entra

**Resultado:** 6

#### c) 

Multiplica todos los valores de `i` de 1 a 4:

- Iteración 1: producto = 1 × 1 = 1
- Iteración 2: producto = 1 × 2 = 2
- Iteración 3: producto = 2 × 3 = 6
- Iteración 4: producto = 6 × 4 = 24

**Resultado:** 24

#### d) 

Está sumando todos los elementos de la lista:

3 + 7 + 1 + 4 + 2 = 17

**Resultado:** 17

#### e)

Elementos mayores que 5:

Hay 3 elementos que cumplen la condición (6, 9, 8)

**Resultado:** 3

#### f)

Filtra los números pares y los multiplica:

2 × 4 × 6 = 48

**Resultado:** 48

#### g)

El algoritmo recorre la lista buscando el valor mínimo y guarda su posición (índice).

- menor inicial = 9 (índice 0)
- i = 1 → 4 < 9 → menor = 4, índice = 1
- i = 2 → 6 > 4 → nada
- i = 3 → 2 < 4 → menor = 2, índice = 3
- i = 4 → 7 > 2 → nada

**Resultado:** 3

#### h)

El algoritmo compara números consecutivos y cuenta cuántas veces un valor es menor que el siguiente:

- 3 < 5 ✅ → contador = 1
- 5 < 2 ❌
- 2 < 7 ✅ → contador = 2
- 7 < 6 ❌

**Resultado:** 2

#### i)

Se estan sumando todos los elementos de la matriz:

- `matriz[0][0] = 1`
- `matriz[0][1] = 2`
- `matriz[1][0] = 3`
- `matriz[1][1] = 4`

Total: 1 + 2 + 3 + 4 = 10

**Resultado:** 10

#### j)

Cuenta cuántos elementos son mayores que 5:

- Fila 0: 2 ❌, 8 ✅, 1 ❌
- Fila 1: 6 ✅, 5 ❌, 9 ✅

Total: 3 elementos (8, 6, 9)

**Resultado:** 3

#### k)

Está accediendo a los elementos donde el índice de fila y columna es el mismo, es decir, la diagonal principal de la matriz:

- i = 0 → `matriz[0][0] = 7`
- i = 1 → `matriz[1][1] = 5`
- i = 2 → `matriz[2][2] = 3`

**Resultado:** 7, 5 y 3

#### l)

Este código suma los valores de cada fila de la matriz y muestra el resultado por pantalla, fila por fila.

- Fila 0: 4 + 2 + 3 = 9
- Fila 1: 1 + 5 + 6 = 12

**Resultado:** Suma de la fila 0: 9 / Suma de la fila 1: 12

---

### 2. Encuentra los errores en los siguientes códigos: 

#### a)

El bucle está sumando el valor de `i`, no los elementos de la lista `numeros`.

**Corrección:**

```python
 suma += numeros[i]
```

#### b)

Está intentando evaluar si `numeros % 2 == 0`, pero `numeros` es toda la lista, no un número.

**Corrección:**

```python
if numeros[i] % 2 == 0:
```

#### c)

Se usa `matriz[i, j]`, pero una lista bidimensional se accede como `matriz[i][j]`, no con coma.

**Corrección:**

```python
print(matriz[i][j])
```

#### d)

Cuando `i = len(lista) - 1` (es decir, 3), se intenta acceder a `lista[4]`, fuera de rango.

```python
for i in range(len(lista) - 1):
```

#### e)

Si "Luis" no está en la lista, la variable `encontrado` no se define y se intenta imprimir → NameError. Se debe inicializar la variable antes de entrar en el bucle.

#### f)

`input` devuelve un string, no un entero.

```python
cantidad = int(input("¿Cuántos números?: "))
```
