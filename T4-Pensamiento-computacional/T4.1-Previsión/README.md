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
