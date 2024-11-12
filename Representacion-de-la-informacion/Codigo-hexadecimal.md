<h1 align="center">Código hexadecimal</h1>
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://frontal.ies-sabadell.cat/eso-moodle/"><img src="https://img.shields.io/badge/Moodle-Cursos-%230081C3" alt="Enllaç a Moodle"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>

</div>

El **código hexadecimal** es fundamental en la **representación de la información** debido a su capacidad para condensar y simplificar la lectura de datos binarios complejos. Al agrupar cada cuatro bits en un solo dígito hexadecimal, los programadores y técnicos pueden manejar y visualizar información de manera más eficiente y comprensible, especialmente en contextos como la programación de bajo nivel, la depuración y la gestión de direcciones de memoria. Además, el sistema hexadecimal es ampliamente utilizado en la representación de colores en diseño gráfico, en códigos de caracteres y en muchas otras aplicaciones donde se requiere una manipulación precisa de los datos. En resumen, el hexadecimal actúa como una **"capa intermedia" entre la legibilidad humana y la precisión binaria**, facilitando la interacción con el hardware y el software a un nivel detallado y accesible.

### Contenido:

- [1. Introducción al Sistema Hexadecimal](#1-introducción-al-sistema-hexadecimal)
  - [1.1 ¿Qué es el sistema hexadecimal?](#11-qué-es-el-sistema-hexadecimal)
  - [1.2 Comparación con otros sistemas de numeración](#12-comparación-con-otros-sistemas-de-numeración)
  - [1.3 Importancia y uso del sistema hexadecimal](#13-importancia-y-uso-del-sistema-hexadecimal)

- [2. Estructura del Sistema Hexadecimal](#2-estructura-del-sistema-hexadecimal)
  - [2.1 Valores y representación de los dígitos hexadecimales](#21-valores-y-representación-de-los-dígitos-hexadecimales)
  - [2.2 Potencias de 16 y lugar de cada dígito en el sistema hexadecimal](#22-potencias-de-16-y-lugar-de-cada-dígito-en-el-sistema-hexadecimal)

- [3. Conversión de Hexadecimal a Binario](#3-conversión-de-hexadecimal-a-binario)
  - [3.1 Tabla de equivalencias de dígitos hexadecimales a binario](#31-tabla-de-equivalencias-de-dígitos-hexadecimales-a-binario)
  - [3.2 Método de conversión de cada dígito hexadecimal en su equivalente binario de 4 bits](#32-método-de-conversión-de-cada-dígito-hexadecimal-en-su-equivalente-binario-de-4-bits)
  - [3.3 Ejemplos prácticos de conversión de hexadecimal a binario](#33-ejemplos-prácticos-de-conversión-de-hexadecimal-a-binario)

- [4. Conversión de Binario a Hexadecimal](#4-conversión-de-binario-a-hexadecimal)
  - [4.1 Agrupación de bits en bloques de 4 para obtener dígitos hexadecimales](#41-agrupación-de-bits-en-bloques-de-4-para-obtener-dígitos-hexadecimales)
  - [4.2 Ejemplos prácticos de conversión de binario a hexadecimal](#42-ejemplos-prácticos-de-conversión-de-binario-a-hexadecimal)

- [5. Aplicaciones Prácticas del Sistema Hexadecimal](#5-aplicaciones-prácticas-del-sistema-hexadecimal)
  - [5.1 Uso en la representación de direcciones de memoria](#51-uso-en-la-representación-de-direcciones-de-memoria)
  - [5.2 Representación de colores en HTML y gráficos](#52-representación-de-colores-en-html-y-gráficos)
  - [5.3 Otras aplicaciones en informática y electrónica](#53-otras-aplicaciones-en-informática-y-electrónica)

<br>

# 1. Introducción al Sistema Hexadecimal

El sistema hexadecimal es un sistema de numeración que utiliza 16 símbolos, lo que permite representar grandes cantidades de información en un formato compacto y legible. Este sistema es ampliamente utilizado en informática debido a su relación directa con el sistema binario, que es el lenguaje básico de las computadoras.

## 1.1 ¿Qué es el sistema hexadecimal?

El sistema hexadecimal es un sistema de base 16, lo que significa que utiliza 16 dígitos distintos para representar valores. Estos dígitos van del `0` al `9` y luego de la `A` a la `F`, donde:

- `0` a `9` representan los valores decimales de 0 a 9.
- `A` a `F` representan los valores decimales de 10 a 15.

Por ejemplo:
- El valor hexadecimal `A` equivale al valor decimal `10`.
- El valor hexadecimal `F` equivale al valor decimal `15`.

Este sistema se utiliza en muchas áreas de la informática para representar datos de una manera más legible, especialmente en casos donde el binario sería demasiado extenso.

## 1.2 Comparación con otros sistemas de numeración (decimal y binario)

En informática, es común trabajar con varios sistemas de numeración:

- **Sistema decimal**: Es el sistema numérico que usamos en la vida cotidiana. Es de base 10 y utiliza los dígitos del `0` al `9`.
- **Sistema binario**: Es el sistema numérico utilizado por los computadores. Es de base 2 y utiliza solo los dígitos `0` y `1`.

El sistema hexadecimal se sitúa entre el binario y el decimal en términos de legibilidad y conveniencia:

- **Binario a hexadecimal**: Cada dígito hexadecimal representa 4 bits en binario. Esto permite condensar grandes cantidades de datos binarios en una forma mucho más corta y comprensible.
- **Decimal a hexadecimal**: Aunque el decimal es más fácil de entender para los humanos, el hexadecimal facilita la representación de grandes números en un formato que se relaciona directamente con el hardware de los computadores.

Por ejemplo:
- El número binario `1111` se representa como `F` en hexadecimal.
- El número decimal `255` se representa como `FF` en hexadecimal.

## 1.3 Importancia y uso del sistema hexadecimal en informática

El sistema hexadecimal es esencial en informática por varias razones:

1. **Representación compacta**: Dado que cada dígito hexadecimal corresponde a 4 bits, el hexadecimal permite una representación más compacta y legible de datos en comparación con el binario.
   
2. **Direcciones de memoria**: En sistemas informáticos, las direcciones de memoria suelen expresarse en hexadecimal para facilitar su lectura y manejo, ya que las direcciones en binario serían demasiado largas y complejas de interpretar.

3. **Colores en diseño gráfico**: En el desarrollo web y diseño gráfico, los colores se representan comúnmente en formato hexadecimal. Por ejemplo, el color `#FF5733` en HTML representa un color específico en código hexadecimal.

4. **Depuración y programación de bajo nivel**: Los programadores y técnicos a menudo usan el hexadecimal al trabajar directamente con hardware o depurar software a nivel de máquina, ya que facilita la interpretación de instrucciones y datos en registros de memoria.

En resumen, el sistema hexadecimal ofrece una forma intermedia entre la legibilidad humana y la precisión binaria, haciéndolo indispensable en el campo de la informática y la electrónica.

# 2. Estructura del Sistema Hexadecimal

El sistema hexadecimal se organiza de forma que cada posición en un número representa una potencia de 16. Esto permite expresar valores grandes en un formato compacto y eficiente, utilizando solo los dígitos del `0` al `9` y las letras `A` a `F`.

## 2.1 Valores y representación de los dígitos hexadecimales (0-9 y A-F)

En hexadecimal, cada dígito puede tomar 16 valores distintos, que van del `0` al `F`. Los valores numéricos de estos dígitos son:

- `0` a `9`: Representan los valores decimales `0` a `9`.
- `A` a `F`: Representan los valores decimales `10` a `15`.

Este esquema de dígitos permite representar cualquier número en base 16. Cada uno de estos dígitos ocupa 4 bits en binario, lo que hace que la conversión entre binario y hexadecimal sea directa y conveniente. Por ejemplo:

- El valor hexadecimal `A` se convierte en `1010` en binario.
- El valor hexadecimal `F` se convierte en `1111` en binario.

Esta correspondencia directa entre hexadecimal y binario es la razón por la que el sistema hexadecimal se usa ampliamente en informática, ya que permite representar datos binarios de manera más legible y compacta.

## 2.2 Potencias de 16 y lugar de cada dígito en el sistema hexadecimal

Cada posición en un número hexadecimal representa una potencia de 16, comenzando desde la derecha con \(16^0\), luego \(16^1\), \(16^2\), y así sucesivamente hacia la izquierda. Por ejemplo, en el número hexadecimal `2AF3`, cada dígito tiene el siguiente valor posicional:

- `3` está en la posición de \(16^0\), por lo que su valor es \(3 \times 16^0 = 3\).
- `F` está en la posición de \(16^1\), lo que equivale a \(15 \times 16^1 = 240\) (recordando que `F` representa 15 en decimal).
- `A` está en la posición de \(16^2\), por lo que su valor es \(10 \times 16^2 = 2560\) (dado que `A` representa 10 en decimal).
- `2` está en la posición de \(16^3\), por lo que su valor es \(2 \times 16^3 = 8192\).

La suma de estos valores da el valor decimal del número hexadecimal `2AF3`:

\[
8192 + 2560 + 240 + 3 = 10995
\]

Esta estructura permite que los números hexadecimales representen grandes valores en menos espacio y facilita la conversión entre sistemas numéricos. Los desarrolladores y técnicos informáticos utilizan esta organización para manipular datos de manera eficiente, especialmente en el contexto de direcciones de memoria y valores de colores en gráficos.
