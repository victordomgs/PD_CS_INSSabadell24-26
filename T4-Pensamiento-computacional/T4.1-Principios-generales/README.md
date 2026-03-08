<h1 align="center">4.1. Principios generales
<div align="center">

</div>

## Contenido

### Pensamiento procedimental
- [4.1.1 Identifique el procedimiento adecuado para resolver un problema](#411-identifique-el-procedimiento-adecuado-para-resolver-un-problema)
- [4.1.2 Evalúe si el orden de las actividades realizadas influirá en el resultado](#412-evalúe-si-el-orden-de-las-actividades-realizadas-influirá-en-el-resultado)
- [4.1.3 Explique el papel de los subprocesos en la resolución de un problema](#413-explique-el-papel-de-los-subprocesos-en-la-resolución-de-un-problema)

### Pensamiento lógico
- [4.1.4 Identifique cuándo es necesario tomar decisiones en una situación concreta](#414-identifique-cuándo-es-necesario-tomar-decisiones-en-una-situación-concreta)
- [4.1.5 Identifique las decisiones necesarias para resolver un problema concreto](#415-identifique-las-decisiones-necesarias-para-resolver-un-problema-concreto)
- [4.1.6 Identifique la condición asociada a una decisión concreta en un problema específico](#416-identifique-la-condición-asociada-a-una-decisión-concreta-en-un-problema-específico)
- [4.1.7 Explique la relación entre las decisiones y las condiciones de un sistema](#417-explique-la-relación-entre-las-decisiones-y-las-condiciones-de-un-sistema)
- [4.1.8 Deduzca reglas lógicas para situaciones del mundo real](#418-deduzca-reglas-lógicas-para-situaciones-del-mundo-real)

### Previsión
- [4.1.9 Identifique las entradas y las salidas necesarias en una solución](#419-identifique-las-entradas-y-las-salidas-necesarias-en-una-solución)
- [4.1.10 Identifique la planificación previa en un problema propuesto y su solución](#4110-identifique-la-planificación-previa-en-un-problema-propuesto-y-su-solución)
- [4.1.11 Explique la necesidad de las precondiciones durante la ejecución de un algoritmo](#4111-explique-la-necesidad-de-las-precondiciones-durante-la-ejecución-de-un-algoritmo)
- [4.1.12 Resuma las precondiciones y las postcondiciones de un problema especificado](#4112-resuma-las-precondiciones-y-las-postcondiciones-de-un-problema-especificado)
- [4.1.13 Identifique excepciones que se deben tener en cuenta en la solución a un problema concreto](#4113-identifique-excepciones-que-se-deben-tener-en-cuenta-en-la-solución-a-un-problema-concreto)

### Pensamiento concurrente
- [4.1.14 Identifique las partes de una solución que se puedan implementar concurrentemente](#4114-identifique-las-partes-of-una-solución-que-se-puedan-implementar-concurrentemente)
- [4.1.15 Describa cómo se puede usar el procesamiento concurrente para resolver un problema](#4115-describa-cómo-se-puede-usar-el-procesamiento-concurrente-para-resolver-un-problema)
- [4.1.16 Evalúe la decisión de usar el procesamiento concurrente para resolver un problema](#4116-evalúe-la-decisión-de-usar-el-procesamiento-concurrente-para-resolver-un-problema)

### Pensamiento abstracto
- [4.1.17 Identifique ejemplos de abstracción](#4117-identifique-ejemplos-de-abstracción)
- [4.1.18 Explique por qué es necesaria la abstracción en la derivación de las soluciones informáticas para una situación dada](#4118-explique-por-qué-es-necesaria-la-abstracción-en-la-derivación-de-las-soluciones-informáticas-para-una-situación-dada)
- [4.1.19 Elabore una abstracción a partir de una situación concreta](#4119-elabore-una-abstracción-a-partir-de-una-situación-concreta)
- [4.1.20 Distinga entre una entidad del mundo real y su abstracción.](#4120-distinga-entre-una-entidad-del-mundo-real-y-su-abstracción)

---

## 4.1.1 Identifique el procedimiento adecuado para resolver un problema

Cuando se tiene que resolver un problema concreto, se debe identificar un **método o procedimiento eficaz**.
Este procedimiento reduce la solución a una serie de **pasos simples**.

Estos pasos deben seguirse en el orden correcto para obtener el resultado deseado.

Por ejemplo:

- Es imposible conducir una **motocicleta** si no sabes montar en **bicicleta**.
- Primero debes aprender a montar en bicicleta y, después, podrás conducir la motocicleta.

<br>

## 4.1.2. Orden de actividades y resultados

Una empresa desea desarrollar un nuevo **sistema de información**.
La fase de análisis será la que la empresa debe completar antes de pasar a las siguientes etapas del proyecto.

Si la empresa intenta implementar el nuevo sistema sin antes analizar el **dominio del problema**, entonces casi con total seguridad se producirá un **desperdicio total de dinero, esfuerzo y recursos**.

<br>

## 4.1.3. Subprocesos en la resolución de problemas

Un buen enfoque para enfrentar un **problema complejo** es desarrollar un método para **dividirlo en subproblemas más pequeños**.
Este método es muy eficaz y eficiente porque es mucho más sencillo abordar varios subproblemas que un único problema complejo.

Los subproblemas resultantes pueden dividirse aún más en otros más pequeños hasta que finalmente puedan ser tratados de manera **individual**.

Esta estrategia se denomina con frecuencia **diseño descendente (top–down design)** o **refinamiento paso a paso (stepwise refinement)**.

El mismo enfoque puede aplicarse al desarrollo de **programas informáticos complejos**.
Mediante el **diseño descendente de programas**, el problema complejo se descompone y para cada subproblema se desarrolla un **subprocedimiento adecuado**.

Un **subprocedimiento** contiene una serie de instrucciones que realizan una tarea.
Cuando un subprocedimiento es llamado, se ejecutan todas las sentencias incluidas en él.

Todos los subprocedimientos que representan diferentes partes de la solución del problema pueden usarse en el momento adecuado mediante sus **identificadores**.

De este modo, el procedimiento se divide en una serie de subprocedimientos; este proceso se conoce como **programación modular**.

Un **identificador** es el nombre que utiliza el programador para identificar de forma única una variable, un objeto, un subprocedimiento, etc.

**Ejemplo:**

Supongamos un programa que calcula las soluciones de una **ecuación cuadrática**.
Un **subprocedimiento** llamado Discriminante podría usarse para calcular el discriminante **D**.

```
Entrada: a, b, c
Llamar al subprocedimiento Discriminante que devuelve el valor D

Si D > 0 entonces
    Calcular x1 = (-b + √D) / (2a)
    Calcular x2 = (-b - √D) / (2a)
Sino, si D = 0 entonces
    Calcular x1 = -b / (2a)
    Calcular x2 = -b / (2a)
Sino
    Salida: "No hay soluciones reales"
Fin Si

Salida: x1, x2

--------------------------------------
Subprocedimiento Discriminante:
    Calcular D = b² - 4 * a * c
    Retornar D
```

<br>

## 4.1.4 Identifique cuándo es necesario tomar decisiones en una situación concreta

### Suma simple

El proceso de suma no requiere tomar ninguna decisión. El algoritmo es directo:

```
Entrada: A
Entrada: B
C = A + B
Salida: C
```

### Problema decisional

Algunos problemas requieren decisiones.

Imagina un cruce peatonal con semáforo:

- Si la luz está **verde**, entonces **es seguro cruzar** → el peatón **cruza**.
- Si la luz está **roja**, entonces el peatón debe **detenerse y esperar**.

```
If Light is green
Then
Set pedestrian = PASS
Else
Set pedestrian = WAIT
End If
```

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%201.%20Pensamiento%20computacional.png" alt="Conditional operation" width="550" height="auto"/>
    <p><em>Figura 1: Operación condicional. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>
  
<br>

## 4.1.5 Identifique las decisiones necesarias para resolver un problema concreto

En la vida cotidiana, las personas están constantemente **identificando las decisiones necesarias** y las diferentes **acciones relevantes** para un problema o una situación.

Es evidente que **tomamos diferentes acciones según las condiciones que prevalezcan**.

### Ejemplo: Ir a un partido de fútbol

Un estudiante puede ir al partido de fútbol **si se cumplen las dos condiciones**:

- Haber hecho los deberes (**Homework done**)
- Que el clima sea bueno (**Weather is good**)

| Homework done | Weather is good | Allowed |
|---------------|-----------------|---------|
| TRUE          | TRUE            | TRUE    |
| TRUE          | FALSE           | FALSE   |
| FALSE         | TRUE            | FALSE   |
| FALSE         | FALSE           | FALSE   |

```
Boolean Homework_done
Boolean Weather_is_good
Boolean Allowed

Input Homework_done
Input Weather_is_good

If Homework_done AND Weather_is_good Then
    Allowed = True
Else
    Allowed = False
End If
```

<br>

## 4.1.6 Identifique la condición asociada a una decisión concreta en un problema específico

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%202.%20Pensamiento%20computacional.png" alt="The loop while" width="550" height="auto"/>
    <p><em>Figura 2: The loop while. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

> [!TIP]
> **WHILE loop:** Ejecuta las instrucciones mientras la condición sea verdadera. En cuanto la condición se evalúa como falsa, el bucle termina y no se ejecuta el cuerpo.
> **FROM/TO loop (también conocido como FOR loop):** Ejecuta las instrucciones un número determinado de veces, según los valores inicial y final. El bucle termina cuando la condición se evalúa como falsa, es decir, cuando se alcanza o supera el límite indicado.

La **iteración** es el proceso de repetir una serie de instrucciones. Es extremadamente útil en la programación y se utiliza para repetir una sentencia o un bloque de sentencias dentro de un algoritmo.

La iteración se expresa usando las sentencias “**from to loop**” y “**while loop**”.

La notación aprobada por el **IB** para desarrollar pseudocódigo incluye los siguientes diagramas de flujo y pseudocódigo para representar estas sentencias.

La figura en forma de **rombo** realiza una prueba booleana, evalúa una expresión y devuelve un valor booleano (**true o false**).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%203.%20Pensamiento%20computacional.png" alt="The from to loop" width="550" height="auto"/>
    <p><em>Figura 3: The from to loop (IB notation). Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

La notación aprobada por el **IB** para desarrollar pseudocódigo no incluye el siguiente **símbolo de diagrama de flujo**, aunque está ampliamente aceptado.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%204.%20Pensamiento%20computacional.png" alt="The from to loop" width="550" height="auto"/>
    <p><em>Figura 4: The from to loop. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

#### Ejemplo: loop while
```
//use of while loop
//to print a message
//user selects the number of times
I = O
X = input("How many times do you want to see the message")
loop while I < x
  I=I+1
output("it will be printed (number entered) times")
end while
```

#### Ejemplo: loop from to
```
//use of from to loop
//to print a message
//user selects the number of times
I = 0
X = input("How many times do you want to see the message")
loop I from 1 to X
  output("it will be printed (number entered) times")
end loop
```

<br>

## 4.1.7 Explique la relación entre las decisiones y las condiciones de un sistema

Una **sentencia condicional** ejecuta diferentes instrucciones dependiendo de una **prueba booleana**.
La sentencia condicional ```if–then–else``` es común en muchos lenguajes de programación y en la lógica humana.

Aunque existen algunas variaciones, la estructura en forma de pseudocódigo es:

```
IF (Boolean condition) THEN 
(Consequent) 
ELSE (Alternative) 
END I
```

Cuando se utiliza un If en un algoritmo, se evalúa una **condición booleana** (ejemplo: x > 0, x = y, etc.).

- Si la condición es **verdadera**, se ejecutará la instrucción o instrucciones del **(Consecuente)**.
- De lo contrario, la ejecución continuará con la instrucción o instrucciones de la **(Alternativa)**.
- Si no existe una rama **else**, el algoritmo continúa después del ```END IF```.

#### Ejemplo: if then else
```
//A way to use if—end if
//It finds if a numbered entered is positive, negative or 0
X = input ("Please enter a number")
if x > 0 then
  output "Positive" 
end if
if X = 0 then 
  output "0" 
end if
if x < 0 then 
  output "Negative" 
and if 
```

#### Ejemplo: if then else
```
//A way to use if—then—else—end if
//It finds if a numbered entered is positive, negative or 0
x = input ("Please enter a number“)
if X > 0 then
  output "Positive"
else if x = 0 then
  output "0"
else
  output "Negative"
end if
```

<br>

## 4.1.8 Deduzca reglas lógicas para situaciones del mundo real

Las **reglas lógicas** o **reglas de inferencia** son reglas obvias para la mayoría de los seres humanos.
La programación y el pensamiento algorítmico implican la **traducción de estas reglas en algoritmos**.

Los siguientes ejemplos cotidianos implican el uso del sentido común:

- Si llueve, me pondré un impermeable.
- Estudiaré todas mis lecciones.
- Tengo que pagar mis facturas.

A veces, la lógica conduce a descubrimientos brillantes, como la **ecuación de Einstein E = m * c²**, que es una manera matemática de expresar la lógica.

Einstein fue capaz de combinar con éxito su lógica con el conocimiento científico.

<br>
