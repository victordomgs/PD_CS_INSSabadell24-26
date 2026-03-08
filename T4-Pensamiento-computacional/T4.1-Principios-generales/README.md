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

## 4.1.9 Identifique las entradas y las salidas necesarias en una solución

La **entrada** (input) es algo que se introduce en un programa, mientras que la salida (output) es algo que se produce después de un proceso.

Se sabe que la **velocidad (V)** se define como la rapidez de un objeto en una dirección determinada.
Usamos la ecuación **V = s / t** para calcular la velocidad media de un objeto V.

- **V** representa la **velocidad** y es la **salida** de nuestra solución.
- s representa el **desplazamiento total** desde la posición inicial del objeto y es una de las **entradas** requeridas en la solución.
- t representa el **tiempo transcurrido** y es otra de las **entradas** requeridas en la solución.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%205.%20Pensamiento%20computacional.png" alt="Calculo de velocidad" width="550" height="auto"/>
    <p><em>Figura 5: Calculo de V. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

<br>

## 4.1.10 Identifique la planificación previa en un problema propuesto y su solución

La **preplanificación** es el proceso de planificar algo con antelación.

Supongamos que un cliente desea desesperadamente comprar un dispositivo en cuanto sea posible. Él/ella puede realizar un **pedido anticipado** de este dispositivo antes de que esté disponible para la compra. Cuando el dispositivo salga al mercado, él/ella será uno de los primeros en obtenerlo. Este es un ejemplo típico de **preorder** (pedido anticipado).

Muchas recetas de cocina nos indican que pongamos la comida en un horno **precalentado**. Eso significa que el cocinero necesita **preplanificar** tal acción.

Supongamos que un estudiante quiere encontrar su libro de texto; él/ella sabe que lo guarda dentro de su taquilla en la escuela. Así que primero debe ir a la escuela y luego abrir su taquilla, donde finalmente encontrará su libro de texto. Este es un ejemplo típico de **pensamiento procedimental y preplanificación**.

El **prefetching**, en términos generales, significa obtener datos o instrucciones de la memoria hacia la caché **antes de que sean realmente necesarios**.
Cuando un programa solicita datos que ya habían sido prefetched, puede usar esos datos directamente y continuar con la ejecución, en lugar de esperar a recuperarlos desde la RAM. Este es un ejemplo típico de **preplanificación de una acción para ahorrar tiempo y mejorar la eficiencia**.

Otro ejemplo de preplanificación eficaz es el uso de **bibliotecas de software**.
Estas consisten en elementos ya preparados para su uso futuro.
Una biblioteca de software contiene **código preescrito, clases, procedimientos, métodos, etc.**, que un programador puede utilizar para añadir más funcionalidades a sus programas, sin tener que reescribir el código equivalente.

Un **diagrama de Gantt** es un tipo de gráfico de barras, llamado así por Henry Gantt.
Se usa ampliamente en la **planificación y gestión de proyectos**, como una forma de mostrar actividades, tareas y eventos en función del tiempo.

- En la parte izquierda del gráfico hay una lista de tareas, actividades y eventos.
- En la parte superior se coloca una escala temporal adecuada.
- Todas las tareas, actividades y eventos están representados por **barras**.
- Cada barra representa la **duración, el día de inicio y el día de finalización** de la tarea, actividad o evento.

Un diagrama de Gantt permite una **inspección sencilla de las actividades del proyecto**, las actividades que se superponen, la duración total del proyecto, etc.

El siguiente diagrama de Gantt representa un proyecto de construcción. Este gráfico muestra detalles como:

- El proyecto incluye **8 actividades**.
- Los **trabajos de obra** deben realizarse antes de las tareas de **fontanería y electricidad**.
- La **fontanería y la electricidad** se realizan de forma **concurrente** (es decir, ambas al mismo tiempo).
- Los trabajos de obra y la fontanería se realizan de forma **secuencial**.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%206.%20Pensamiento%20computacional.png" alt="Gráfico de Gantt" width="550" height="auto"/>
    <p><em>Figura 6: Gráfico de Gantt en un proyecto en construcción. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

El siguiente **diagrama de Gantt** representa un proyecto general. Este gráfico proporciona los siguientes detalles:

- El proyecto consta de **cuatro actividades**.
- La **Tarea 1** y la **Tarea 2** se realizan de manera **secuencial** (la segunda no puede comenzar antes de que la primera esté completada).
- La **duración total** del proyecto es de **21 días**.
- La **Tarea 2** es la tarea de mayor duración.

    <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%207.%20Pensamiento%20computacional.png" alt="Gráfico de Gantt" width="550" height="auto"/>
    <p><em>Figura 7: Gráfico de Gantt en un proyecto genérico. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

<br>

## 4.1.11 Explique la necesidad de las precondiciones durante la ejecución de un algoritmo

En la mayoría de los casos, cuando un equipo de programación se enfrenta a un **problema grande**, este problema se divide en **subproblemas más fáciles de resolver y controlar**.

Cada miembro del equipo resolverá uno o más de estos “subproblemas fáciles”.
Cada solución será un **subprocedimiento**, y se expresará como un **algoritmo**.

Cada subprocedimiento será llamado mediante su **identificador** y tendrá una tarea concreta que cumplir.

- La **precondición** indica lo que debe ser verdadero **antes de que el subprocedimiento sea llamado**.
- La **postcondición** indica lo que será verdadero **cuando el subprocedimiento complete su tarea**.

En resumen:

- La **precondición** describe el **estado inicial** antes de la ejecución de un algoritmo.
- La **postcondición** describe el **estado final** después de la ejecución de un algoritmo.

<br>

## 4.1.12 Resuma las precondiciones y las postcondiciones de un problema especificado

Al **cocinar una comida para la cena**, todos los ingredientes necesarios deben estar disponibles **antes de cocinar**.
Esto es la **precondición** del algoritmo cocinar.

Después de cocinar, se necesita una mesa para poder comer.
Esto es la **postcondición** para una cena adecuada.

El siguiente fragmento de algoritmo tiene como **precondición** ```A = 2``` y como **postcondición** ```B = 30```:

```
//pre—condition A=2 
X = 3
B = X + A
if A > 0 then
    B = 3 * 6
else
    B = 0
end if
//post-condition B=30
```

El siguiente algoritmo calcula e imprime la **raíz cuadrada** de un número entero ```x```.
Tiene como **precondición** que ```x >= 0``` y como **postcondición** el cálculo de ```√x```.

```
// Pre-condition: x >= 0
// Post-condition: calculates the square root of x
Sub-procedure square_root(x como parámetro)
    x = √x
    output x
End of Sub-procedure
```

Ejemplos de ejecución del subprocedimiento ```square_root```:

- **Entrada: 9** → Salida: 3
- **Entrada: 0** → Salida: 0
- **Entrada: -1** → Viola la precondición, ya que la raíz cuadrada de un número negativo no está definida en los enteros (la raíz de un número siempre es positiva o compleja).

<br>

## 4.1.13 Identifique excepciones que se deben tener en cuenta en la solución a un problema concreto

Una **excepción** es un acto o evento que interrumpe el flujo previsto de la ejecución de un programa.
Las excepciones ocurren durante la ejecución del programa y pueden ser gestionadas eficazmente mediante mecanismos específicos que proporcionan la mayoría de los lenguajes de programación modernos.

El término **excepción**, en este punto del temario, se refiere a una ocasión o caso que **no es compatible con la regla general**.

El siguiente ejemplo aclara la importancia de identificar diversas **excepciones** en la solución de un problema específico.

### Ejemplo de programación: Alternativas y precondiciones

Una empresa tiene la siguiente política para calcular la prima de fin de año de sus empleados:

- Si el empleado ha trabajado en la empresa **9 meses o más**, entonces la prima es igual al **30% de su salario mensual**.
- Si el empleado ha trabajado en la empresa **menos de 9 meses** y su salario es **menor de 2000 €**, entonces la prima es igual al **20% de su salario mensual**.
- Si el empleado ha trabajado en la empresa **menos de 9 meses** y su salario es igual o **superior a 2000 €**, entonces la prima es igual al **10% de su salario mensual**.

Un programador no entendió el problema y escribió el siguiente pseudocódigo, que **viola tanto las precondiciones como las postcondiciones**:

```
// Pre—condition violated: Months = the correct number of months the employee worked for the company
// Post-conditions violated: the program calculates and outputs the correct bonus for each employee according to the company’s policy

// Wrong BONUS PROGRAM
BONUS = 0
TOTAL = 0
SALARY = 1200
BONUS = (30/100) * (SALARY)
TOTAL = BONUS + (SALARY * 12)
output "TOTAL IS:" , TOTAL , "Euros"
output "BONUS IS:" , BONUS , "Euros"
```

El siguiente pseudocódigo **sí satisface las precondiciones y postcondiciones del problema**:

```
// Correct BONUS PROGRAM
MONTHS = 0
SALARY = 0
BONUS
TOTAL

SALARY = input("what is the salary of the employee?")
MONTHS = input("How many months did he/she work?")

if MONTHS >= 9 then
    BONUS = (30/100) * (SALARY)
    TOTAL = BONUS + (SALARY * MONTHS)

else if MONTHS < 9 AND SALARY < 2000 then
    BONUS = (20/100) * (SALARY)
    TOTAL = BONUS + (SALARY * MONTHS)

else if MONTHS < 9 AND SALARY >= 2000 then
    BONUS = (10/100) * (SALARY)
    TOTAL = BONUS + (SALARY * MONTHS)

end if

output "TOTAL IS:" , TOTAL , "Euros"
output "BONUS IS:" , BONUS , "Euros"
```
