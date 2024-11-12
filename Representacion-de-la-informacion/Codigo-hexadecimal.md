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

# 3. Conversión de Hexadecimal a Binario

La conversión de hexadecimal a binario es un proceso directo que facilita la representación de datos en un formato que los ordenadores pueden procesar fácilmente. Dado que cada dígito hexadecimal corresponde exactamente a 4 bits en binario, esta conversión es simple y eficiente.

## 3.1 Tabla de equivalencias de dígitos hexadecimales a binario

Para facilitar la conversión, aquí tienes una tabla de equivalencias entre los dígitos hexadecimales y sus representaciones en binario de 4 bits:

| Hexadecimal | Binario |
|-------------|---------|
| 0           | 0000    |
| 1           | 0001    |
| 2           | 0010    |
| 3           | 0011    |
| 4           | 0100    |
| 5           | 0101    |
| 6           | 0110    |
| 7           | 0111    |
| 8           | 1000    |
| 9           | 1001    |
| A           | 1010    |
| B           | 1011    |
| C           | 1100    |
| D           | 1101    |
| E           | 1110    |
| F           | 1111    |

Esta tabla permite convertir cada dígito hexadecimal individualmente a binario de forma rápida y sencilla.

## 3.2 Método de conversión de cada dígito hexadecimal en su equivalente binario de 4 bits

Para convertir un número hexadecimal a binario, simplemente convierte cada dígito hexadecimal a su equivalente binario de 4 bits utilizando la tabla anterior. El resultado es la concatenación de estos grupos de 4 bits.

Por ejemplo, para convertir el número hexadecimal `2F` a binario:

1. Toma el primer dígito, `2`, que en binario es `0010`.
2. Toma el segundo dígito, `F`, que en binario es `1111`.
3. Concatenando ambos resultados, `2F` en hexadecimal se convierte en `00101111` en binario.

Este método permite una conversión rápida sin necesidad de cálculos adicionales, ya que cada dígito hexadecimal se traduce directamente a un bloque de 4 bits.

## 3.3 Ejemplos prácticos de conversión de hexadecimal a binario

A continuación, se muestran algunos ejemplos prácticos de conversión para ayudar a comprender el proceso:

1. **Ejemplo 1**: Convertir `1A3` a binario
   - `1` en hexadecimal es `0001` en binario.
   - `A` en hexadecimal es `1010` en binario.
   - `3` en hexadecimal es `0011` en binario.
   - Resultado: `1A3` en hexadecimal es `000110100011` en binario.

2. **Ejemplo 2**: Convertir `4F9` a binario
   - `4` en hexadecimal es `0100` en binario.
   - `F` en hexadecimal es `1111` en binario.
   - `9` en hexadecimal es `1001` en binario.
   - Resultado: `4F9` en hexadecimal es `010011111001` en binario.

3. **Ejemplo 3**: Convertir `B2E` a binario
   - `B` en hexadecimal es `1011` en binario.
   - `2` en hexadecimal es `0010` en binario.
   - `E` en hexadecimal es `1110` en binario.
   - Resultado: `B2E` en hexadecimal es `101100101110` en binario.

Estos ejemplos muestran cómo el proceso de conversión de hexadecimal a binario puede aplicarse a cualquier número hexadecimal, proporcionando una forma rápida de representar valores en un formato adecuado para el procesamiento en sistemas digitales.

# 4. Conversión de Binario a Hexadecimal

La conversión de binario a hexadecimal se basa en la agrupación de bits en bloques de 4, ya que cada bloque de 4 bits corresponde exactamente a un dígito hexadecimal. Este método es eficiente y rápido, dado que evita cálculos complejos y aprovecha la relación directa entre estos dos sistemas numéricos.

## 4.1 Agrupación de bits en bloques de 4 para obtener dígitos hexadecimales

Para convertir un número binario a hexadecimal, sigue estos pasos:

1. **Agrupa los bits en bloques de 4**: Comienza desde la derecha del número binario y agrupa los bits en bloques de 4. Si el número total de bits no es múltiplo de 4, agrega ceros a la izquierda para completar el último bloque.
   
2. **Convierte cada bloque de 4 bits a hexadecimal**: Utiliza la tabla de equivalencias para convertir cada bloque de 4 bits en su valor hexadecimal correspondiente.

Por ejemplo:
- Para el número binario `10110111`, agrupamos los bits de derecha a izquierda en bloques de 4: `1011 0111`.
- Luego, cada bloque se convierte a hexadecimal:
  - `1011` se convierte en `B`.
  - `0111` se convierte en `7`.
- Por lo tanto, `10110111` en binario es `B7` en hexadecimal.

Esta técnica hace que la conversión de binario a hexadecimal sea rápida y directa.

## 4.2 Ejemplos prácticos de conversión de binario a hexadecimal

A continuación, algunos ejemplos prácticos de conversión para ilustrar el proceso:

1. **Ejemplo 1**: Convertir `11011010` a hexadecimal
   - Agrupamos los bits: `1101 1010`
   - Convertimos cada grupo:
     - `1101` es `D` en hexadecimal.
     - `1010` es `A` en hexadecimal.
   - Resultado: `11011010` en binario es `DA` en hexadecimal.

2. **Ejemplo 2**: Convertir `111100111010` a hexadecimal
   - Agrupamos los bits (añadiendo un `0` a la izquierda para completar el primer bloque): `0001 1110 0111 1010`
   - Convertimos cada grupo:
     - `0001` es `1`.
     - `1110` es `E`.
     - `0111` es `7`.
     - `1010` es `A`.
   - Resultado: `111100111010` en binario es `1E7A` en hexadecimal.

3. **Ejemplo 3**: Convertir `101011` a hexadecimal
   - Agrupamos los bits (añadiendo ceros a la izquierda): `0010 1011`
   - Convertimos cada grupo:
     - `0010` es `2`.
     - `1011` es `B`.
   - Resultado: `101011` en binario es `2B` en hexadecimal.

Estos ejemplos muestran que el método de agrupar en bloques de 4 bits simplifica la conversión y permite que cualquier número binario se traduzca rápidamente a hexadecimal.

# 5. Aplicaciones Prácticas del Sistema Hexadecimal

El sistema hexadecimal tiene numerosas aplicaciones prácticas en informática y electrónica, gracias a su capacidad para representar datos binarios de manera compacta y legible. Desde la representación de direcciones de memoria hasta la codificación de colores en diseño gráfico, el hexadecimal es fundamental para varias áreas de la tecnología.

## 5.1 Uso en la representación de direcciones de memoria

En sistemas informáticos, las direcciones de memoria se representan comúnmente en hexadecimal. Esto permite que los valores largos en binario se compriman en una forma más legible y manejable. Por ejemplo, una dirección de memoria como `1010 1101 1110 0010` en binario se convierte en `ADE2` en hexadecimal, facilitando la lectura y la escritura de las direcciones de memoria.

El uso de hexadecimal para las direcciones es particularmente útil en programación de bajo nivel y en la depuración de sistemas, donde los programadores interactúan directamente con la memoria de la máquina. Gracias al hexadecimal, los desarrolladores pueden acceder, manipular y analizar datos en memoria de forma rápida y eficiente.

## 5.2 Representación de colores en HTML y gráficos

En el diseño gráfico y desarrollo web, el sistema hexadecimal es la norma para representar colores. Los colores se expresan con códigos hexadecimales de 6 dígitos, donde cada par de dígitos representa la intensidad de los colores rojo, verde y azul (RGB). Por ejemplo:

- `#FF5733` representa un color con `FF` (255 en decimal) de rojo, `57` (87 en decimal) de verde y `33` (51 en decimal) de azul.
- `#000000` representa el color negro, donde todos los canales están en `00`.
- `#FFFFFF` representa el color blanco, donde todos los canales están en `FF`.

Esta representación hexadecimal de colores permite una amplia gama de colores (16,777,216 combinaciones posibles) en un formato compacto y estandarizado que los navegadores y programas gráficos interpretan directamente.

## 5.3 Otras aplicaciones en informática y electrónica

Además de las direcciones de memoria y la representación de colores, el sistema hexadecimal se utiliza en varias otras aplicaciones en informática y electrónica, tales como:

- **Códigos de máquina y depuración**: Al trabajar con lenguajes de bajo nivel o ensamblador, los códigos de máquina se representan frecuentemente en hexadecimal, lo que facilita la identificación y manipulación de instrucciones específicas.

- **Representación de datos binarios en depuradores**: En entornos de desarrollo y herramientas de depuración, los datos binarios, como el contenido de registros y variables en la memoria, suelen mostrarse en formato hexadecimal para facilitar la visualización y edición de valores binarios complejos.

- **Direcciones MAC en redes**: Las direcciones MAC (Media Access Control) se expresan en hexadecimal. Una dirección MAC típica tiene el formato `00:1A:2B:3C:4D:5E`, donde cada par de dígitos representa 8 bits.

- **Configuración y programación de hardware**: En dispositivos electrónicos y sistemas embebidos, se utiliza hexadecimal para definir configuraciones específicas y valores de registros de hardware, ya que facilita la entrada y revisión de datos a nivel de bits.

Estas aplicaciones demuestran cómo el sistema hexadecimal proporciona una representación compacta y versátil de la información, permitiendo que los desarrolladores y técnicos interactúen de manera efectiva con datos binarios en múltiples contextos.


