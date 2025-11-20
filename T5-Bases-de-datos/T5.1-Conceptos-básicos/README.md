<h1 align="center">5.1. Conceptos básicos
<div align="center">

</div>

## Contenido:

- [5.1.1. Diferencias entre datos e información](#511-diferencias-entre-datos-e-información)
- [5.1.2. Diferencias entre un sistema de información y una base de datos](#512-diferencias-entre-un-sistema-de-información-y-una-base-de-datos)
- [5.1.3. Necesidad de las bases de datos](#513-necesidad-de-las-bases-de-datos)
- [5.1.4. Coherencia de los datos](#514-coherencia-de-los-datos)
- [5.1.5. Transacción de bases de datos](#515-transacción-de-bases-de-datos)
- [5.1.6. Concepto de concurrencia](#516-concepto-de-concurrencia)
- [5.1.7. Propiedades ACID](#517-propiedades-ACID)
- [5.1.8. Funciones de consulta y actualización](#518-funciones-de-consulta-y-actualización)
- [5.1.9. Validación y verificación de datos](#519-validación-y-verificación-de-datos)

---

## 5.1.1. Diferencias entre datos e información

En el ámbito de las bases de datos, es fundamental distinguir entre **datos e información**, porque todo el trabajo posterior —el diseño de tablas, la consulta, el análisis y la toma de decisiones— parte de comprender qué representa cada uno.

Los **datos** son elementos aislados, brutos, sin procesar. Por sí solos no tienen un significado completo ni permiten extraer conclusiones. Pueden ser números, palabras, símbolos o incluso valores medidos por sensores. Un dato es simplemente un registro de algo que ha sucedido o una característica de un objeto, pero sin contexto. Por ejemplo, el número “23”, el texto “Madrid” o el valor “4.7” son datos: existen, pero no sabemos aún qué representan. ¿Es “23” la edad de una persona? ¿El número de productos vendidos? ¿La temperatura? Mientras no se añada contexto, permanece como un dato suelto.

La **información**, en cambio, surge cuando esos datos se organizan, se interpretan y se conectan con un contexto. La información aporta significado, responde preguntas y permite comprender una situación. Cuando sabemos que “23” se refiere a “23 estudiantes matriculados en un curso”, ese dato ha sido transformado en información útil. La información permite tomar decisiones, identificar patrones y entender fenómenos.

En una base de datos, este proceso de convertir datos en información ocurre constantemente. Las tablas almacenan datos individuales: nombres, fechas, cantidades, identificadores. Pero cuando un sistema de gestión de bases de datos organiza esos datos y ejecutamos consultas para relacionarlos —por ejemplo, “¿cuántos estudiantes se han matriculado este año?” o “¿cuál ha sido la venta total del mes?”— obtenemos información que sí es interpretable y valiosa.

Dicho de otro modo:

- **Los datos son materia prima**, elementos independientes que no cuentan una historia por sí solos.
- **La información es el resultado del procesamiento**, la interpretación y la estructuración de los datos para que tengan sentido en un contexto concreto.

Comprender esta diferencia es esencial para trabajar con bases de datos, porque el objetivo final de cualquier sistema de información no es almacenar datos por almacenarlos, sino transformarlos en información relevante que apoye decisiones, análisis y conocimiento.

<br>

## 5.1.2. Diferencias entre un sistema de información y una base de datos

Aunque a menudo se usan como si fueran lo mismo, un **sistema de información** y una **base de datos** son conceptos distintos y cumplen funciones muy diferentes dentro de una organización. Entender esta diferencia ayuda a los estudiantes a situar las bases de datos dentro del ecosistema más amplio de tecnologías que permiten gestionar, analizar y utilizar la información.

Una **base de datos** es, en esencia, un repositorio donde se almacenan datos de forma organizada. Su función principal es garantizar que esos datos se guardan de manera estructurada, coherente y segura, para que puedan consultarse y modificarse con facilidad. En una base de datos encontramos tablas, registros, claves primarias y relaciones; es un espacio que se centra en cómo se representan y organizan los datos. Por sí sola, una base de datos no toma decisiones, no automatiza procesos ni interactúa con los usuarios más allá de permitirles almacenar y recuperar información.

En cambio, un **Sistema de Información (SI)** es un conjunto mucho más amplio de elementos que trabajan juntos para transformar datos en información útil. Incluye no solo bases de datos, sino también software, hardware, procedimientos, personas y flujos de trabajo. Un sistema de información tiene como objetivo apoyar las actividades de una organización: gestionar pedidos, controlar inventarios, procesar matrículas, generar informes o ayudar a la toma de decisiones. Por ejemplo, un sistema de información escolar incluye la base de datos de alumnos, la aplicación que usan los profesores para introducir notas, los informes automáticos que se generan, y las reglas que determinan cómo se procesan los datos.

Una forma sencilla de visualizar la diferencia es pensar que una base de datos es **el corazón** del sistema —almacena los datos—, pero el sistema de información es **todo el organismo**, con sus procesos, herramientas y usuarios interactuando alrededor de esos datos. Un sistema de información usa la base de datos como fuente, pero la enriquece con procesos de negocio, interfaces y mecanismos que convierten los datos en información útil.

<br>

## 5.1.3. Necesidad de las bases de datos

En prácticamente cualquier organización moderna —desde una pequeña tienda hasta un hospital o una institución educativa— existe una enorme cantidad de datos que deben ser almacenados, organizados y consultados de manera eficiente. La necesidad de las bases de datos surge precisamente de esta realidad: gestionar datos de forma manual o mediante archivos sueltos no solo es ineficiente, sino también arriesgado. Las bases de datos aparecen como una respuesta tecnológica que permite transformar el caos potencial de los datos en una estructura ordenada, accesible y fiable.

Antes de la existencia de los sistemas de bases de datos, era habitual que la información se guardara en documentos en papel, hojas de cálculo o archivos separados. Estos enfoques generaban numerosos problemas: duplicación de datos, inconsistencias, dificultades para encontrar información, errores humanos y falta de control sobre quién tenía acceso a qué. Además, cuando la cantidad de datos empezaba a crecer, estos métodos se volvían prácticamente inmanejables.

Las **bases de datos** se crearon para resolver precisamente estos desafíos. Proporcionan un modelo estructurado donde los datos se pueden guardar de manera coherente, evitando duplicidades y permitiendo mantener la integridad de la información. Esto significa que, si un dato cambia, ese cambio se actualiza en un solo lugar, y cualquier sistema que utilice esa base de datos accederá siempre a la versión correcta y más reciente.

Otra necesidad fundamental que cubren las bases de datos es la **eficiencia**. Gracias a los sistemas de gestión de bases de datos (SGBD), es posible hacer consultas complejas en cuestión de milisegundos: encontrar todos los pedidos de un cliente, calcular ventas por mes o identificar qué estudiantes están matriculados en un curso. Esta capacidad de procesar y relacionar datos rápidamente es crucial en contextos donde la toma de decisiones depende de información actualizada.

Las bases de datos también permiten garantizar la **seguridad**. Un SGBD ofrece mecanismos para controlar quién puede ver, modificar o eliminar datos, evitando accesos no autorizados y protegiendo la información sensible. Además, permiten realizar copias de seguridad automáticas, minimizar pérdidas ante fallos y asegurar la continuidad del trabajo.

Por último, las bases de datos son necesarias porque facilitan que múltiples usuarios trabajen con los mismos datos al mismo tiempo sin interferir entre sí. Esto resulta especialmente importante en organizaciones donde diferentes departamentos o personas necesitan acceder simultáneamente a la información.

En resumen, las bases de datos son necesarias porque:

- **Organizan** los datos de forma estructurada y coherente.
- **Eliminan duplicidades** y minimizan errores.
- **Permiten consultas rápidas y eficientes.**
- **Aseguran la integridad y la seguridad** de la información.
- **Facilitan el acceso multiusuario** sin conflictos.
- **Apoyan la toma de decisiones** proporcionando información actualizada y fiable.

En un mundo donde la información es uno de los recursos más valiosos, las bases de datos se convierten en una herramienta esencial para transformar grandes cantidades de datos en conocimiento útil.

<br>

## 5.1.4. Coherencia de los datos

En una base de datos, la **coherencia** se refiere a que los datos se mantengan correctos, válidos y consistentes a lo largo del tiempo. Es decir, que reflejen fielmente la realidad que representan. Para lograr esta coherencia, los sistemas de gestión de bases de datos utilizan varios mecanismos, entre ellos las **transacciones**, los **estados** y los **procesos de actualización**.

### Transacciones: operaciones que deben funcionar como una unidad

Una transacción es un conjunto de operaciones que deben ejecutarse como si fueran un solo bloque indivisible. Su función es garantizar que la base de datos nunca quede en un estado incompleto o incoherente.

Por ejemplo, imaginemos una transferencia bancaria:

- Se resta dinero de una cuenta.
- Se suma la misma cantidad a otra cuenta.

Estas dos operaciones deben ejecutarse juntas. No tendría sentido que se realizara solo una parte, porque eso crearía un error en los datos. Por eso se consideran una única transacción: o se completan ambas operaciones, o no se completa ninguna.

### Estados de una transacción: cómo se controla el proceso

Para asegurar que las transacciones mantienen la coherencia, el SGBD controla distintos estados:

1. **Activo:** la transacción está en proceso; se están realizando operaciones.
2. **Parcialmente completada:** todas las operaciones se han ejecutado, pero los cambios aún no se han hecho permanentes.
3. **Comprometida (committed):** el sistema confirma la transacción; los cambios pasan a formar parte definitiva de la base de datos.
4. **Abortada:** por un error, una colisión o una violación de integridad, la transacción no puede completarse. El sistema deshace todos los cambios.

Este manejo de estados evita que actualizaciones incompletas o incorrectas afecten negativamente a los datos.

### Actualizaciones: aplicarlas con control para mantener la integridad

Cada vez que se modifica un dato en la base de datos (insertar, borrar o actualizar), el sistema debe asegurarse de que ese cambio no rompe ninguna regla lógica. Estas reglas se conocen como **restricciones de integridad**, como:

- claves primarias únicas,
- claves foráneas válidas,
- valores dentro de un rango permitido,
- relaciones correctas entre tablas.

Cuando la base de datos aplica una actualización dentro de una transacción, comprueba automáticamente que dichas reglas se cumplen. Si no es así, la transacción se **revierte** (rollback) y la base de datos vuelve al estado anterior, evitando inconsistencias.

### Un sistema coordinado para proteger los datos

El uso conjunto de transacciones, control de estados y actualizaciones supervisadas permite que:

- Las operaciones complejas se realicen de manera segura.
- Ningún dato quede en un estado intermedio o corrupto.
- Las relaciones entre datos se mantengan correctas.
- Varias personas puedan trabajar de forma simultánea sin interferir entre ellas.

En última instancia, estos mecanismos garantizan que la base de datos mantenga su **integridad** incluso en contextos con mucho movimiento de datos y múltiples usuarios, asegurando que represente siempre una versión fiable de la realidad.

<br>

## 5.1.5. Transacción de bases de datos

Una **transacción de bases de datos** es una unidad lógica de trabajo compuesta por una o varias operaciones que deben ejecutarse de manera completa y coherente. En otras palabras, es un conjunto de acciones que la base de datos trata como un único bloque indivisible: o se realizan todas correctamente, o no se realiza ninguna.

La idea fundamental es evitar que la base de datos quede en un estado inconsistente. Si una transacción incluye varias operaciones —por ejemplo, insertar un registro, actualizar otro o eliminar un tercero—, el sistema debe garantizar que todas se ejecutan de forma correcta antes de confirmar los cambios. Si algo sale mal en mitad del proceso (un error, una violación de integridad o un fallo de sistema), la transacción se **revierte** por completo y la base de datos vuelve al estado anterior, como si nada hubiera ocurrido.

Una transacción se entiende mejor si se piensa como una acción "todo o nada". Es la manera que tienen los sistemas de gestión de bases de datos de proteger la fiabilidad de la información, incluso cuando hay muchos usuarios accediendo a la vez.

<br>

## 5.1.6. Concepto de concurrencia

La **concurrencia** en bases de datos se refiere a la capacidad que tiene un sistema para permitir que **varios usuarios o procesos accedan y trabajen con los mismos datos al mismo tiempo**, sin que esto provoque errores, inconsistencias o pérdida de información. Esta característica es fundamental en entornos reales, donde es habitual que muchas personas interactúen simultáneamente con un mismo sistema: estudiantes consultando notas, empleados registrando ventas o usuarios realizando transacciones financieras.

La concurrencia es necesaria porque una base de datos no funciona en aislamiento; está integrada en sistemas que deben estar siempre disponibles. Sin concurrencia, solo un usuario podría operar con la base de datos a la vez, lo cual sería impráctico e ineficiente. Pero permitir que muchos usuarios trabajen simultáneamente introduce desafíos: ¿qué ocurre si dos personas intentan modificar el mismo dato al mismo tiempo? ¿Cómo evitar que una lectura se base en información incompleta? ¿Qué pasa si dos operaciones simultáneas llevan a resultados contradictorios?

Para resolver estos problemas, los sistemas de gestión de bases de datos utilizan mecanismos de control como bloqueos, niveles de aislamiento y transacciones ACID. El objetivo es equilibrar dos necesidades:

1. **Maximizar el acceso simultáneo** para que muchos usuarios puedan trabajar sin esperas innecesarias.
2. **Mantener la coherencia y la integridad de los datos**, evitando conflictos.

La concurrencia bien gestionada asegura que cada usuario perciba una base de datos estable y fiable, incluso cuando en segundo plano múltiples operaciones están ocurriendo al mismo tiempo.

## 5.1.7. Propiedades ACID

Las propiedades **ACID** describen las garantías fundamentales que un sistema de gestión de bases de datos debe ofrecer para que las transacciones se ejecuten de manera fiable, coherente y segura. Estas propiedades aseguran que incluso en situaciones de alta concurrencia, errores inesperados o fallos del sistema, los datos permanezcan correctos y la base de datos siga funcionando sin perder integridad.

Las siglas **ACID** corresponden a **Atómicas, Consistentes, Aisladas y Duraderas**. Cada una define un aspecto esencial del comportamiento de las transacciones.

### Atómicas (Atomicity)

La atomicidad establece que una transacción debe tratarse como una unidad indivisible: **o se ejecutan todas sus operaciones o no se ejecuta ninguna**.
Si en mitad de una transacción ocurre un error —un fallo eléctrico, una violación de una regla de integridad, un choque con otra operación—, el sistema debe revertir todos los cambios realizados hasta ese momento. Esto garantiza que la base de datos nunca quede en un estado intermedio o incompleto.

En esencia, la transacción funciona como un “todo o nada”.

### Consistentes (Consistency)

La propiedad de consistencia garantiza que una transacción solo puede llevar a la base de datos de un **estado válido a otro estado válido**, respetando siempre las reglas y restricciones establecidas.
Esto incluye claves primarias, claves foráneas, dominios de valores, relaciones lógicas y cualquier otra regla definida para asegurar que los datos representen correctamente la realidad.

Si una transacción rompe alguna de estas reglas, el sistema la aborta automáticamente.

### Aisladas (Isolation)

La aislamiento asegura que las transacciones no interfieren entre sí, incluso cuando se ejecutan simultáneamente.
Cada transacción debe comportarse como si fuese la única que se está ejecutando en el sistema, aunque en realidad haya muchas operaciones ocurriendo en paralelo.

Esto evita problemas como leer datos temporales o inconsistentes, sobrescribir cambios de otros usuarios o producir resultados contradictorios.

### Duraderas (Durability)

La durabilidad garantiza que, una vez una transacción se completa y se confirma (**commit**), sus cambios pasan a ser permanentes.
Incluso si el sistema falla inmediatamente después, los cambios no se pierden. Los sistemas de bases de datos utilizan mecanismos como registros de transacciones, archivos de recuperación y almacenamiento seguro para asegurar esta permanencia.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%201.%20Bases%20de%20datos.gif" alt="ACID" width="850" height="auto"/>
    <p><em>Figura 1: ACID. Fuente: SubStack</em></p>
  </div>

## 5.1.8. Funciones de consulta y actualización

En una base de datos, todo el trabajo que realizan los usuarios y las aplicaciones se puede agrupar en dos grandes tipos de funciones: **consultas y actualizaciones**. Estas funciones representan dos formas distintas de interactuar con los datos y son esenciales para comprender cómo se gestiona la información en un sistema moderno.

### Funciones de consulta: obtener información sin modificar los datos

Las **consultas** son operaciones diseñadas para **leer** datos de la base de datos sin alterarlos. Son fundamentales porque permiten a los usuarios responder preguntas y obtener información útil a partir de los datos almacenados.

Una consulta puede ser tan sencilla como recuperar todos los registros de una tabla, o tan compleja como combinar datos de varias tablas, aplicar filtros, ordenar resultados o realizar cálculos. Los lenguajes de consulta, como SQL, permiten transformar datos brutos en información significativa.

Ejemplos típicos de consultas incluyen:

- “Mostrar todos los estudiantes matriculados en un curso”.
- “Calcular la venta total del mes”.
- “Buscar los productos cuyo stock es inferior a un valor determinado”.

Lo más importante es que **las consultas no cambian el contenido de la base de datos**: son operaciones seguras, que solo leen y presentan información.

### Funciones de actualización: modificar el contenido de la base de datos

Las **actualizaciones** son operaciones que **cambian** los datos almacenados. Engloban tres tipos principales de acciones:

- **Inserción (INSERT):** añadir nuevos datos.
- **Modificación (UPDATE):** cambiar datos existentes.
- **Eliminación (DELETE):** borrar datos que ya no son necesarios.

Estas funciones afectan directamente al estado interno de la base de datos y, por tanto, deben realizarse con especial cuidado. Cada actualización debe respetar las reglas de integridad definidas (como claves foráneas, valores permitidos o unicidad), y normalmente se ejecuta dentro de una **transacción** para garantizar que la base de datos nunca quede en un estado incoherente.

Ejemplos habituales de actualizaciones:

- Registrar un nuevo cliente.
- Cambiar la dirección de un empleado.
- Eliminar un pedido cancelado.

Las actualizaciones pueden tener un impacto significativo en el sistema, pues modifican la información que otros usuarios podrían necesitar.

### Un equilibrio fundamental

Las bases de datos modernas deben manejar cientos o miles de consultas y actualizaciones simultáneas. Las consultas suelen ser más frecuentes, ya que los usuarios pasan más tiempo leyendo información que modificándola. Sin embargo, las actualizaciones son igual de críticas porque mantienen la base de datos actualizada y precisa.

Para garantizar la coherencia en entornos concurrentes, los sistemas de bases de datos aplican mecanismos como transacciones ACID, bloqueos y control de aislamiento, que permiten que ambas funciones coexistan sin comprometer la integridad de la información.

## 5.1.9. Validación y verificación de datos

En cualquier sistema de información, especialmente en bases de datos, no basta con almacenar datos: es fundamental asegurarse de que esos datos sean correctos, coherentes y fiables. Para lograrlo, entran en juego dos procesos que suelen confundirse, pero que cumplen funciones distintas y complementarias: la **validación** y la **verificación** de datos.

Aunque ambos persiguen la calidad de la información, lo hacen desde perspectivas diferentes.

### Validación: comprobar si los datos cumplen las reglas establecidas

La **validación** es el proceso mediante el cual la base de datos o el sistema comprueba que los datos introducidos **son aceptables según un conjunto de reglas o restricciones predefinidas**.
Estas reglas están diseñadas para evitar errores comunes: valores fuera de rango, formatos incorrectos o datos que no cumplen con las normas lógicas del sistema.

Ejemplos de validación incluyen:

- Comprobar que un correo electrónico tiene un formato válido.
- Verificar que una edad no es negativa.
- Asegurar que un campo obligatorio no se queda vacío.
- Revisar que una fecha existe realmente (por ejemplo, que no se introduzca “31 de febrero”).

Estas validaciones pueden realizarse tanto desde la interfaz de usuario como desde el propio SGBD, mediante **restricciones de integridad** (CHECK, NOT NULL, UNIQUE…) o reglas de negocio.

La validación **no garantiza que los datos sean verdaderos**, solo que son **lógicamente correctos y cumplen el formato requerido**.

### Verificación: comprobar si los datos son correctos respecto a la realidad

La **verificación** va un paso más allá. Su objetivo es comprobar si los datos **son auténticos, exactos o coinciden con la realidad** que representan.

Mientras que la validación se centra en el formato y la estructura, la verificación se ocupa del **contenido real**.

Ejemplos de verificación:

- Confirmar que un número de teléfono pertenece realmente al usuario.
- Comprobar que un DNI introducido existe y corresponde a una persona real.
- Revisar físicamente una factura para asegurar que la cantidad registrada es correcta.
- Comparar un registro con su fuente original (documento, sensor, sistema externo).

La verificación suele requerir una comprobación manual o una comparación contra otra base de datos o un sistema confiable. Por eso, es habitual en contextos donde la precisión es crucial, como bancos, hospitales o instituciones educativas.

### Por qué son necesarias: proteger la integridad de la información

Tanto la validación como la verificación contribuyen a mejorar la calidad de los datos, pero lo hacen desde ángulos distintos:

- **La validación evita errores de entrada y mantiene la coherencia interna.**
- **La verificación garantiza que los datos son verdaderos y exactos respecto al mundo real.**

Cuando ambas se aplican correctamente, reducen errores, evitan inconsistencias y fortalecen la integridad de la base de datos, permitiendo que la información resultante sea fiable y útil para la toma de decisiones.
