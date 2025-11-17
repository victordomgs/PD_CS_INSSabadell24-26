<h1 align="center">5.2. El modelo relacional de bases de datos
<div align="center">

</div>

## Contenido:

- [5.2.1. Sistema de gestión de bases de datos](#521-sistema-de-gestión-de-bases-de-datos)
- [5.2.2. Funciones y herramientas de un SGBD](#522-funciones-y-herramientas-de-un-SGBD)
- [5.2.3. Uso de un SGBD](#523-uso-de-un-SGBD)
- [5.2.4. Esquema de una base de datos](#524-esquema-de-una-base-de-datos)
- [5.2.5. Los tres niveles del esquema](#525-los-tres-niveles-del-esquema)
- [5.2.6. Diccionario de datos](#526-diccionario-de-datos)
- [5.2.7. El lenguaje de definición de datos](#527-el-lenguaje-de-definición-de-datos)
- [5.2.8. Modelos de datos](#528-modelos-de-datos)
- [5.2.9. Términos clave de las bases de datos](#529-términos-clave-de-las-bases-de-datos)
- [5.2.10. Tipologias de relaciones](#5210-tipologias-de-relaciones)
- [5.2.11. Redundancia de datos](#5211-redundancia-de-datos)
- [5.2.12. Integridad referencial](#5212-integridad-referencial)
- [5.2.13. Formas normales](#5213-formas-normales)
- [5.2.14. Bases de datos normalizadas](#5214-bases-de-datos-normalizadas)
- [5.2.15. Tipologia de datos](#5215-tipologia-de-datos)
- [5.2.16. Diagrama ERD](#5216-diagrama-ERD)
- [5.2.17. Elaboración de una base de datos relacional](#5217-elaboración-de-una-base-de-datos-relacional)
- [5.2.18. Consultas en bases de datos](#5218-consultas-en-bases-de-datos)
- [5.2.19. Consultas simples y compuestas](#5219-consultas-simples-y-compuestas)
- [5.2.20. Elaboración de consultas](#5220-elaboración-de-consultas)

---

## 5.2.1. Sistema de gestión de bases de datos

Un **Sistema de Gestión de Bases de Datos**, conocido habitualmente por sus siglas en inglés **DBMS (Database Management System)**, es el software que permite crear, gestionar, manipular y controlar una base de datos. Puede entenderse como la capa intermedia entre los datos almacenados y los usuarios o aplicaciones que necesitan acceder a ellos.

Sin un DBMS, trabajar con grandes cantidades de datos sería complejo, lento y propenso al error. Este sistema proporciona un conjunto de herramientas y mecanismos que permiten organizar los datos de forma eficiente, mantener su coherencia y garantizar su seguridad. En esencia, convierte a la base de datos en un recurso accesible, fiable y útil para cualquier organización.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%202.%20Bases%20de%20datos.png" alt="SGBD" width="650" height="auto"/>
    <p><em>Figura 1: Principales SGBD de la actualidad. Fuente: fp-informatica</em></p>
  </div>

<br>

## 5.2.2. Funciones y herramientas de un SGBD

Un **Sistema de Gestión de Bases de Datos (SGBD)** no solo almacena datos: proporciona un conjunto de **funciones y herramientas** diseñadas para garantizar que esos datos se puedan gestionar de forma eficaz, segura y coherente. Estas capacidades permiten que el SGBD actúe como un entorno completo donde los usuarios, administradores y aplicaciones pueden interactuar con la base de datos sin necesidad de conocer los detalles internos de cómo se almacena la información.

### 1. Lenguajes para definir y manipular datos

Uno de los pilares de un SGBD son los lenguajes que ofrece para interactuar con la información:

- **DDL (Data Definition Language):** permite crear, modificar o eliminar la estructura de la base de datos, como tablas, vistas o índices.
- **DML (Data Manipulation Language):** permite insertar, modificar, consultar y eliminar datos.
- **DCL (Data Control Language):** gestiona permisos y accesos.
- **TCL (Transaction Control Language):** controla transacciones y asegura propiedades ACID (por ejemplo, COMMIT y ROLLBACK).

Estos lenguajes proporcionan una interfaz estándar entre los usuarios y el sistema.

### 2. Gestión del almacenamiento y optimización

El SGBD decide cómo se guardarán realmente los datos en disco —qué estructuras usar, cómo organizarlos y cómo recuperarlos rápidamente. Incluye herramientas como:

- **Índices**, para acelerar las consultas.
- **Gestores de memoria**, para optimizar el uso de RAM y disco.
- **Planificadores de consultas**, que determinan la forma más eficiente de ejecutar una sentencia.

Estas herramientas permiten que incluso bases de datos muy grandes funcionen con rapidez.

### 3. Control de concurrencia

Los SGBD deben manejar el acceso simultáneo de muchos usuarios o procesos. Para ello utilizan:

- **Bloqueos (locks)** para evitar conflictos.
- **Niveles de aislamiento** para equilibrar seguridad y eficiencia.
- **Gestión de transacciones**, usando las propiedades ACID para asegurar que los datos permanezcan coherentes.

Gracias a esto, un SGBD puede soportar miles de operaciones simultáneas sin que se corrompan los datos.

### 4. Seguridad y control de acceso

La protección de los datos es fundamental. El SGBD controla:

- **Usuarios y roles**, asignando permisos específicos.
- **Autenticación**, para verificar identidades.
- **Autorización**, para definir qué acciones puede realizar cada usuario.
- **Registros de auditoría**, que permiten rastrear actividades y detectar accesos indebidos.

Este conjunto de herramientas garantiza la confidencialidad y la integridad de la información.

### 5. Copias de seguridad y recuperación ante fallos

Un SGBD incorpora mecanismos para proteger los datos frente a pérdidas accidentales o fallos del sistema:

- **Backups**, completos o incrementales.
- **Journaling o registros de transacciones**, para restaurar cambios recientes.
- **Herramientas de recuperación**, que reconstruyen la base de datos tras un error.

Estas funciones aseguran la durabilidad de los datos incluso ante eventos imprevistos.

### 6. Herramientas de administración y monitorización

El administrador de la base de datos (DBA) dispone de utilidades para supervisar y ajustar el rendimiento del sistema:

- Paneles de control y estadísticas.
- Herramientas para gestionar el espacio de almacenamiento.
- Monitores de actividad de usuarios.
- Analizadores de rendimiento de consultas.

Estas herramientas ayudan a mantener el sistema rápido, saludable y seguro.

### 7. Interfaces para aplicaciones

Un SGBD proporciona APIs, controladores y protocolos estándar (como ODBC o JDBC) que permiten que aplicaciones externas se conecten fácilmente a la base de datos. Esto facilita la creación de aplicaciones web, móviles o de escritorio que utilicen los datos sin tener que gestionar directamente su almacenamiento.

<br>

## 5.2.3. Uso de un SGBD

El uso de un Sistema de Gestión de Bases de Datos (SGBD) es fundamental en cualquier entorno donde se trabaje con grandes cantidades de información que deben almacenarse, organizarse y consultarse de manera eficiente. Un SGBD actúa como intermediario entre los usuarios y los datos, proporcionando un entorno seguro, estructurado y controlado para gestionar la información.

### Acceder a los datos sin conocer los detalles internos

Una de las principales ventajas de utilizar un SGBD es que permite a los usuarios trabajar con la información sin preocuparse por cómo se almacena realmente en el disco. Tanto un profesor consultando las notas de sus alumnos como un empleado registrando un pedido lo hacen a través de herramientas o aplicaciones que se comunican con el SGBD.
Este se encarga de traducir las órdenes en operaciones sobre los datos.

De este modo, el SGBD ofrece una capa de abstracción:

- Los usuarios ven datos y resultados.
- El sistema se encarga de la gestión interna, el almacenamiento y la seguridad.

### Permitir la interacción de múltiples usuarios

En la mayoría de organizaciones, muchas personas necesitan acceder a la base de datos al mismo tiempo. El SGBD gestiona este acceso simultáneo mediante técnicas de control de concurrencia y transacciones ACID, garantizando que los datos permanezcan coherentes incluso cuando decenas o cientos de operaciones ocurren simultáneamente.

Esto es esencial en sistemas de uso diario como plataformas de ventas, matriculación o inventarios.

### Facilitar consultas y actualizaciones

El uso más habitual de un SGBD implica dos tipos de operaciones:

- **Consultas**, para obtener información: buscar registros, filtrar resultados, hacer cálculos o combinar tablas.
- **Actualizaciones**, para modificar los datos almacenados: insertar nuevos registros, cambiar valores o eliminar información obsoleta.

Para ello, el SGBD utiliza lenguajes como **SQL**, que proporcionan una forma estandarizada de interactuar con la base de datos.

### Garantizar seguridad y control

El uso de un SGBD también incluye mecanismos de seguridad que permiten controlar:

- quién accede a la base de datos,
- qué acciones puede realizar cada usuario,
- qué datos son visibles u ocultos,
- cómo se registran las actividades dentro del sistema.

Esto resulta indispensable en entornos que manejan información sensible, como hospitales, centros educativos o bancos.

### Automatizar tareas y mantener la integridad

Los SGBD permiten configurar reglas y procesos automáticos, como:

- restricciones de integridad,
- disparadores (triggers),
- procedimientos almacenados,
- tareas de mantenimiento.

Gracias a estas herramientas, el sistema ayuda a mantener la calidad de los datos y a automatizar procesos repetitivos.

### Conectar aplicaciones y sistemas

Finalmente, un SGBD sirve como base para que múltiples aplicaciones compartan la misma información. Por ejemplo:

- una aplicación web,
- un panel de administración,
- un sistema de informes,
- un programa de análisis de datos.

Todos pueden conectar con el mismo SGBD, garantizando que trabajan con datos actualizados.

<br>

## 5.2.4. Esquema de una base de datos

El esquema es la **descripción estructural y lógica** de una base de datos, que especifica sus tablas, campos, relaciones y reglas de integridad. Representa el diseño que organiza y da forma a los datos, aunque por sí mismo no contiene datos.

<br>

## 5.2.5. Los tres niveles del esquema

Cuando se diseña una base de datos, no se trabaja directamente con los datos ni tampoco solo con la estructura interna del sistema. En realidad, se utilizan **distintos niveles de abstracción** que permiten separar lo que el usuario ve, lo que el sistema interpreta y la forma en que la información se almacena físicamente.

Este enfoque se organiza en **tres niveles de esquema**: conceptual, lógico y físico.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%203.%20Bases%20de%20datos.png" alt="ANSI arquitecture" width="450" height="auto"/>
    <p><em>Figura 3: Arquitectura de 3 niveles. Fuente: Dongee</em></p>
  </div>

### 1. Nivel conceptual: la visión global de la base de datos

El **esquema conceptual** representa la **descripción general de la base de datos**, independiente de cualquier tecnología o software concreto.
Es la visión “intermedia”, centrada en los elementos principales y en las reglas que rigen los datos.

Aquí se definen:

- las entidades (por ejemplo, Alumno, Curso, Pedido),
- los atributos importantes,
- las relaciones entre entidades,
- y las reglas que deben cumplirse.

El objetivo del esquema conceptual es **describir qué información existe y cómo se relaciona**, sin decidir todavía cómo se almacenará ni en qué tablas concretas.

Podemos pensar en él como una maqueta abstracta de la base de datos: clara, ordenada y comprensible incluso para personas no técnicas.

### 2. Nivel lógico: la estructura técnica de la base de datos

El **esquema lógico** transforma el diseño conceptual en una estructura específica de un modelo de datos concreto, como el modelo relacional.
En este nivel, las entidades y relaciones se convierten en elementos formales de la base de datos:

- tablas,
- columnas,
- claves primarias,
- claves foráneas,
- índices lógicos,
- restricciones de integridad.

Aunque sigue sin preocuparse por cómo se guardarán físicamente los datos, el esquema lógico ya está preparado para implementarse en un SGBD real.
Es aquí donde se aplican técnicas de **normalización** y se definen las estructuras que garantizan la integridad de los datos.

### 3. Nivel físico: cómo se almacenan realmente los datos

El **esquema físico** describe **cómo se guardan los datos en el almacenamiento real**, en el disco o en la memoria del servidor.
Se centra en aspectos internos del SGBD que afectan al rendimiento, como:

- organización de archivos,
- métodos de acceso a datos,
- índices físicos,
- particiones,
- estructuras de almacenamiento,
- utilización de memoria y cachés.

Este diseño tiene como objetivo optimizar **la velocidad y la eficiencia**, pero es invisible para los usuarios finales y para la mayoría de los programadores.
