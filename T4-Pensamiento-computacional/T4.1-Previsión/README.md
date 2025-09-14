<h1 align="center">4.1. Previsión
<div align="center">

</div>

## Contenido:

- [4.1.9. Entradas y salidas necesarias en una solución](#419-entradas-y-salidas-necesarias-en-una-solución)
- [4.1.10. Planificación previa en un problema y su solución](#4110-planificación-previa-en-un-problema-y-su-solución)
- [4.1.11. Necesidad de precondiciones](#4111-necesidad-de-precondiciones)
- [4.1.12. Precondiciones y postcondiciones](#4112-precondiciones-y-postcondiciones)
- [4.1.13. Excepciones que requieren consideración](#4113-excepciones-que-requieren-consideración)

---

## 4.1.9. Entradas y salidas necesarias en una solución

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

## 4.1.10. Planificación previa en un problema y su solución

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
    <p><em>Figura 5: Gráfico de Gantt en un proyecto en construcción. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

El siguiente **diagrama de Gantt** representa un proyecto general. Este gráfico proporciona los siguientes detalles:

- El proyecto consta de **cuatro actividades**.
- La **Tarea 1** y la **Tarea 2** se realizan de manera **secuencial** (la segunda no puede comenzar antes de que la primera esté completada).
- La **duración total** del proyecto es de **21 días**.
- La **Tarea 2** es la tarea de mayor duración.

    <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%207.%20Pensamiento%20computacional.png" alt="Gráfico de Gantt" width="550" height="auto"/>
    <p><em>Figura 6: Gráfico de Gantt en un proyecto genérico. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

## 4.1.11. Necesidad de precondiciones

En la mayoría de los casos, cuando un equipo de programación se enfrenta a un **problema grande**, este problema se divide en **subproblemas más fáciles de resolver y controlar**.

Cada miembro del equipo resolverá uno o más de estos “subproblemas fáciles”.
Cada solución será un **subprocedimiento**, y se expresará como un **algoritmo**.

Cada subprocedimiento será llamado mediante su **identificador** y tendrá una tarea concreta que cumplir.

- La **precondición** indica lo que debe ser verdadero **antes de que el subprocedimiento sea llamado**.
- La **postcondición** indica lo que será verdadero **cuando el subprocedimiento complete su tarea**.

En resumen:

- La **precondición** describe el **estado inicial** antes de la ejecución de un algoritmo.
- La **postcondición** describe el **estado final** después de la ejecución de un algoritmo.

## 4.1.12. Precondiciones y postcondiciones

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

## 4.1.13. Excepciones que requieren consideración

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
