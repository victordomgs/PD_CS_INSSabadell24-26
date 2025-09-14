<h1 align="center">4.1. Pensamiento concurrente
<div align="center">

</div>

## Contenido:

- [4.1.14. Partes de una solución que se puede implementar concurrentemente](#4114-partes-de-una-solución-que-se-puede-implementar-concurrentemente)
- [4.1.15. Procesamiento concurrente para resolver problemas](#4115-procesamiento-concurrente-para-resolver-problemas)
- [4.1.16. Decisión de usar el pensamiento concurrente para resolver un problema](#4116-decisión-de-usar-el-pensamiento-concurrente-para-resolver-un-problema)

---

## 4.1.14. Partes de una solución que se puede implementar concurrentemente

**Concurrente** significa algo que ocurre **al mismo tiempo que otra cosa**.

Imagina una situación en la que un usuario responde a sus correos electrónicos **mientras escucha** su canción favorita.
O bien otra situación en la que una persona está buscando información en la **WWW**, **imprimiendo** un ensayo y **descargando** algunos controladores para su PC.

En ambos escenarios, las tareas se realizan de manera **concurrente**.

En informática, el **procesamiento concurrente** significa la ejecución de **instrucciones diferentes simultáneamente por múltiples procesadores** para lograr el mejor rendimiento.

Una explicación simplificada de este proceso es que los **programas se dividen en procedimientos** y los **procedimientos en subprocedimientos**.
Estos son luego asignados a **unidades de procesamiento separadas** para que se ejecuten simultáneamente.

El **procesamiento secuencial**, en cambio, es la ejecución de todos los subprocedimientos **uno tras otro** por un solo procesador.

## 4.1.15. Procesamiento concurrente para resolver problemas

Imagina un mundo donde no exista el **procesamiento concurrente**:

- La construcción de casas tardaría mucho más.
- La gente tendría que terminar su desayuno antes de escuchar las noticias de la mañana.
- Una persona tendría que elegir entre **oír o ver, entender o escribir, y sentir o pensar**.

El famoso ejemplo de la preparación de la “**pasta con salsa**” puede aclarar aún más la situación:
No hay necesidad de cocinar la pasta antes que la salsa, porque la mayoría de la gente puede usar **dos fogones** para preparar **tanto la pasta como la salsa al mismo tiempo**.

De esta manera, la persona promedio ahorra un tiempo valioso y disfruta de **pasta caliente acompañada de salsa caliente**.

## 4.1.16. Decisión de usar el pensamiento concurrente para resolver un problema

El **procesamiento concurrente** requiere una mejor **planificación y coordinación de recursos**.
Sin esto, el procesamiento concurrente puede causar **problemas serios**, y la decisión de usar procesamiento en serie o concurrente para resolver un problema debe ser cuidadosamente examinada.

Por ejemplo:
Un **contador** está realizando cambios en una **base de datos financiera electrónica**.
Mientras lo hace, un **segundo contador** abre la misma base de datos, que incluye todas las modificaciones realizadas hasta ese momento por el primer contador, y la utiliza para recuperar información.

El primer contador luego decide que los cambios realizados hasta ese momento **no son válidos** y devuelve los registros de la base de datos a su condición anterior.
El primer contador guarda la base de datos.

La información que el segundo contador recuperó ya **no existe**, pero él no es consciente de esta información crucial.

Este problema podría haberse evitado si **nadie pudiera leer la base de datos modificada** hasta que el primer contador decidiera que las ediciones y modificaciones eran **definitivas**.
