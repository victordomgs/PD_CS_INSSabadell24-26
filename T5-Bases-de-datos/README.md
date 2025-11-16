# Objetivo de evaluación para T5

- **Objetivo de evaluación 1:** clasifique, defina, dibuje con precisión, enumere, indique, rotule.
- **Objetivo de evaluación 2:** anote, aplique, calcule, describa, diseñe, distinga, estime, identifique, presente, rastree, resuma.
- **Objetivo de evaluación 3:** analice, comente, compare, compare y contraste, contraste, deduzca, demuestre, derive, determine, dibuje aproximadamente, discuta, elabore, ¿en qué medida…?, evalúe, examine, explique, formule, interprete, investigue, justifique, prediga, sugiera.

Las notas que siguen a algunos enunciados de evaluación sirven como orientación adicional a los profesores. En estas, se muestran enlaces a otros temas (VÍNCULO), y se pueden sugerir ideas para la promoción de determinados objetivos generales de la asignatura (OBJ. GEN.), de Teoría del Conocimiento (TdC), del Programa de los Años Intermedios (PAI), de cuestiones sociales o éticas (S/E) y de la dimensión internacional (INT).


## A: Bases de datos  
### A.1 Conceptos básicos (5 horas)

| Enunciado de evaluación | Obj. | Notes para el profesor |
|-------------------------|------|-------------------------|
| **A.1.1** Resuma las diferencias entre datos e información. | 2 | Los datos no tienen significado. Para que resulten útiles, los datos deben interpretarse para generar información. |
| **A.1.2** Resuma las diferencias entre un sistema de información y una base de datos. | 2 | Los alumnos deben saber que estos términos no son sinónimos. Las bases de datos son un componente de un sistema de información. **PAI** Tecnología. |
| **A.1.3** Discuta por qué son necesarias las bases de datos. | 3 | Deben tratarse temas como los beneficios de compartir datos. **S/E** Por ejemplo, información correcta de consumidores o clientes. |
| **A.1.4** Describa el uso de transacciones, estados y actualizaciones para mantener la coherencia de los datos (y la integridad). | 2 | Por ejemplo, para garantizar la coherencia de los datos en una transferencia de dinero entre dos cuentas es necesario completar dos operaciones (extraer de una cuenta e ingresar en otra). La transacción no se realizará si no se completan ambas operaciones. **S/E** Por ejemplo, garantizar la información correcta de consumidores o clientes. |
| **A.1.5** Defina el término “transacción de bases de datos”. | 1 | |
| **A.1.6** Explique la concurrencia en una situación en que se compartan datos. | 3 | |
| **A.1.7** Explique la importancia de las propiedades ACID en una transacción de bases de datos. | 3 | ACID significa: <br> • Atomicidad <br> • Coherencia <br> • Aislamiento (isolation) <br> • Durabilidad |
| **A.1.8** Describa las dos funciones que se deben realizar sobre las bases de datos. | 2 | Funciones de consulta y funciones de actualización. |
| **A.1.9** Explique la función de la validación de datos y la verificación de datos. | 3 | |

### A.2 El modelo relacional de bases de datos (15 horas)

| Enunciado de evaluación | Obj. | Notas para el profesor |
|-------------------------|------|-------------------------|
| **A.2.1** Defina los términos “sistema de gestión de bases de datos (SGBD)” y “sistema de gestión de bases de datos relacional (SGBDR)”. | 1 | |
| **A.2.2** Resuma las funciones y herramientas de un SGBD. | 2 | Se deben tener en cuenta varias funciones y herramientas de gestión, centrándose en la creación, manipulación y consultas de bases de datos. |
| **A.2.3** Describa cómo se puede usar un SGBD para potenciar la seguridad de los datos. | 2 | Entre las características se incluyen la validación de datos, los permisos de acceso y el bloqueo de datos. |
| **A.2.4** Defina el término “esquema”. | 1 | |
| **A.2.5** Identifique las características de los tres niveles del esquema: conceptual, lógico y físico. | 2 | |
| **A.2.6** Resuma la naturaleza del diccionario de datos. | 2 | |
| **A.2.7** Explique la importancia del lenguaje de definición de datos en la implementación de un modelo de datos. | 3 | |
| **A.2.8** Explique la importancia de los modelos de datos en el diseño de una base de datos. | 3 | |
| **A.2.9** Defina los siguientes términos relacionados con las bases de datos: “tabla”, “registro”, “campo”, “clave principal”, “clave secundaria”, “clave externa”, “clave candidata”, “clave primaria compuesta” y “composición”. | 1 | Estos son los términos aceptados.<br><br>Una tabla es equivalente a un archivo o una relación.<br>Un registro equivale a una tupla o fila.<br>Un campo es equivalente a un atributo o columna.<br>Solo es necesario conocer una composición interna. |
| **A.2.10** Identifique los distintos tipos de relaciones en una base de datos: una a una, una a muchas y muchas a muchas. | 2 | **OBJ. GEN. 4** Demostrar iniciativa en la aplicación crítica de las habilidades de pensamiento para entender las relaciones entre las entidades en un contexto propuesto.<br><br>**VÍNCULO** Pensamiento abstracto. |
| **A.2.11** Resuma los problemas generados por los datos redundantes. | 2 | **S/E, OBJ. GEN. 8** Problemas relacionados con la integridad y fiabilidad de los datos. |
| **A.2.12** Resuma la importancia de la integridad referencial en una base de datos normalizada. | 2 | **S/E, OBJ. GEN. 8** Problemas relacionados con la integridad y fiabilidad de los datos. |
| **A.2.13** Describa las diferencias entre la primera forma normal (1FN), la segunda forma normal (2FN) y la tercera forma normal (3FN). | 2 | Por ejemplo:<br>• En la 1FN no se repiten filas o columnas<br>• La 2FN se basa en la dependencia funcional completa<br>• La 3FN implica la eliminación de dependencias transitivas |
| **A.2.14** Describa las características de una base de datos normalizada. | 2 | Los alumnos deben comprender las características de una base de datos normalizada hasta la 3FN. |
| **A.2.15** Evalúe la idoneidad de los distintos tipos de datos. | 3 | Se espera que los alumnos justifiquen la selección de un tipo de datos concreto en una situación dada. Por ejemplo, un número entero o un punto flotante.<br><br>**S/E, OBJ. GEN. 8** La cuestión de la privacidad de las partes interesadas.<br><br>**S/E, OBJ. GEN. 8** Cuando se planifique un nuevo sistema, debe considerarse al usuario final como parte interesada fundamental.<br><br>Comparar las diferentes necesidades de cada parte interesada.<br><br>¿Quiénes son las partes interesadas pertinentes? |
| **A.2.16** Elabore un diagram entidad-relación (ERD) para una situación propuesta. | 3 | Los alumnos deben elaborar diagramas entidad-relación en 3FN para una base de datos relacional.<br><br>**OBJ. GEN. 4** Demostrar habilidades que permitan la comprensión de las relaciones entre las entidades en una situación específica.<br><br>**VÍNCULO** Pensamiento abstracto.<br><br>**PAI** Tecnología: Bases de datos. |
| **A.2.17** Elabore una base de datos relacional hasta la 3FN usando objetos como tablas, consultas, formularios, informes y macros. | 3 | Los alumnos deberán demostrar conocimientos sobre diseño de bases de datos en la prueba 2 del NM y del NS derivada de las actividades prácticas.<br><br>**TdC** Utilitarismo, el mayor beneficio para la mayoría. El fin justifica los medios.<br><br>**OBJ. GEN. 4, 6** Demostrar iniciativa en la aplicación crítica de las habilidades de pensamiento y de resolución de problemas para entender las relaciones entre las entidades de una situación dada.<br><br>**OBJ. GEN. 5** Necesidad de colaborar eficazmente con el usuario final para resolver problemas complejos.<br><br>**S/E, OBJ. GEN. 8** Conciencia sobre el impacto social y las consideraciones éticas durante el desarrollo de sistemas que potencialmente ofrezcan acceso a datos sensibles. |
| **A.2.18** Explique cómo una consulta puede ofrecer una vista en una base de datos. | 3 | |
| **A.2.19** Describa la diferencia entre una consulta simple y una compuesta. | 2 | Los alumnos deben saber usar:<br>• Operadores booleanos como AND, OR y NOT<br>• Crear consultas parametrizadas<br>• Crear campos derivados<br><br>**PAI** Matemáticas: Formas de números, álgebra, patrones y sucesiones, lógica y algoritmos. |
| **A.2.20** Resuma los distintos métodos de elaborar una consulta. | 2 | No es obligatorio que los alumnos escriban consultas en SQL.<br><br>Los alumnos deben ser conscientes de que el lenguaje es una herramienta para consultar datos.<br><br>**PAI** Matemáticas: Formas de números, álgebra, patrones y sucesiones, lógica y algoritmos. |

### A.3 Aspectos adicionales de la gestión de bases de datos (10 horas)

| Enunciado de evaluación | Obj. | Notas para el profesor |
|-------------------------|------|-------------------------|
| **A.3.1** Explique la función de un administrador de bases de datos. | 3 | Un conferenciante visitante o el administrador de la red del colegio podrían explicar esta función.<br><br>**S/E** Cuestiones relacionadas con la privacidad, la seguridad y la integridad de los datos.<br><br>**VÍNCULO** Sistemas en organizaciones. |
| **A.3.2** Explique cómo los usuarios finales pueden interactuar con una base de datos. | 3 | Actividades prácticas para mostrar el uso de SQL, QBE, consultas visuales e interfaces en lenguaje natural. |
| **A.3.3** Describa distintos métodos de recuperación de bases de datos. | 2 | **S/E** Cuestiones relacionadas con el coste de implementar estos sistemas frente a la importancia de los datos. |
| **A.3.4** Resuma cómo funcionan los sistemas de bases de datos integrados. | 3 | **OBJ. GEN. 9** Apreciar el desarrollo continuo de los sistemas informáticos. |
| **A.3.5** Resuma el uso de las bases de datos en áreas como: control de existencias, registros policiales y sanitarios, y datos de empleados. | 2 | **S/E** Cuestiones relacionadas con la privacidad, la seguridad y la integridad de los datos.<br><br>**VÍNCULO** Sistemas en organizaciones. |
| **A.3.6** Sugiera métodos para garantizar la privacidad de los datos personales y la responsabilidad de los encargados de que los datos no se vendan ni se publiquen de ninguna forma. | 3 | Los alumnos deben conocer las implicaciones de los grandes sistemas de bases de datos.<br><br>También se deben tratar algunos principios de legislación, como la protección de datos y el buen uso de la informática. No es necesario estudiar la legislación específica de ningún país.<br><br>**S/E** Cuestiones relacionadas con la privacidad, la seguridad y la integridad de los datos.<br><br>**VÍNCULO** Sistemas en organizaciones. |
| **A.3.7** Discuta la necesidad de que algunas bases de datos estén abiertas a consultas de terceros (policía, gobierno, etc.). | 3 | **S/E** Cuestiones relacionadas con la privacidad, la seguridad y la integridad de los datos.<br><br>**VÍNCULO** Sistemas en organizaciones.<br><br>**OBJ. GEN. 8** Conocimiento del impacto social y de las consideraciones éticas de almacenar grandes cantidades de datos. |
| **A.3.8** Explique la diferencia entre cotejo informático de datos (*data matching*) y minería de datos (*data mining*). | 3 | |
