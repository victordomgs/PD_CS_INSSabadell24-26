# Actividad 4: Resta Binaria

En esta actividad, aprenderás a realizar restas en el sistema binario, incluyendo cómo hacer préstamos cuando sea necesario. La resta binaria sigue reglas similares a la resta en el sistema decimal, pero con dos dígitos (0 y 1) y el uso de préstamos entre columnas.

## Objetivo

- Realizar correctamente operaciones de resta en binario, incluyendo el uso de préstamos.

## Reglas de la Resta Binaria

**0 - 0 = 0**
**1 - 0 = 1**
**1 - 1 = 0**
**0 - 1 = 1** (con préstamo de la siguiente posición)

Cuando **0 - 1** necesita un préstamo, la columna de la izquierda debe reducirse en 1 y la columna actual se convierte en 10 (igual que en el sistema decimal).

## Ejemplo

Resta los números binarios **1101** y **101**.

**Pasos**:

1. Comenzamos de derecha a izquierda.
   - En la primera columna, \(1 - 1 = 0\).
   - En la segunda columna, \(0 - 0 = 0\).
   - En la tercera columna, \(1 - 1 = 0\).
   - En la cuarta columna, necesitamos un préstamo para restar \(0 - 1\), lo que resulta en **1000** en binario.

**Resultado**: La resta de **1101** y **101** es **1000** en binario.

## Ejercicios

**Realiza las siguientes restas en binario:**

1. 1101 - 101
2. 10101 - 1001
3. 1110 - 110
4. 10011 - 1010
5. 11100 - 1011
6. 10010 - 111
7. 11011 - 10001
8. 100000 - 1111
9. 111111 - 10101
10. 10010 - 100
