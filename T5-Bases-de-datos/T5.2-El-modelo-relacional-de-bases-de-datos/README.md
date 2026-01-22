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
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%203.%20Bases%20de%20datos.png" alt="ANSI arquitecture" width="600" height="auto"/>
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

<br>

## 5.2.6. Los diccionarios de datos

El diccionario de datos es un **repositorio centralizado** de metadatos que describe la estructura, las reglas y los elementos de una base de datos. El SGBD lo mantiene y utiliza para garantizar el funcionamiento correcto, seguro y eficiente del sistema.

<br>

## 5.2.7. El lenguaje de definición de datos

Cuando se diseña una base de datos, se parte de un **modelo de datos**, que describe cómo debe organizarse la información: qué entidades existirán, qué atributos las caracterizan y cómo se relacionan entre sí. Pero un modelo, por sí solo, es solo una representación conceptual. Para convertir ese diseño en una base de datos real y funcional, se necesita una herramienta clave: el **Lenguaje de Definición de Datos**, conocido como **DDL (Data Definition Language)**.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%204.%20Base%20de%20datos.jpg" alt="SQL language" width="600" height="auto"/>
    <p><em>Figura 4: El lenguaje SQL. Fuente: Geeks for Geeks</em></p>
  </div>

### Convertir el diseño conceptual en estructura real

Mediante el DDL, el diseñador define:

- **Tablas**, que representan entidades del modelo.
- **Columnas y sus tipos de datos**, que corresponden a los atributos.
- **laves primarias**, que garantizan la identificación única de los registros.
- **Claves foráneas**, que establecen las relaciones entre tablas.
- **Restricciones de integridad**, que aseguran que los datos cumplen reglas lógicas.

### Garantizar la integridad desde el principio

El DDL no solo crea la estructura: también define reglas que protegen la integridad de la base de datos.
Estas reglas pueden incluir:

- valores permitidos,
- longitudes máximas,
- integridad referencial,
- unicidad,
- obligatoriedad de ciertos campos.

### Principales sentencias del DDL

1. **CREATE** – Crear estructuras

Se utiliza para crear nuevos objetos en la base de datos, como bases de datos, tablas o vistas.

Ejemplo: creación de una tabla en un modelo relacional

```sql
CREATE TABLE Alumno (
    id_alumno INT PRIMARY KEY,
    nombre VARCHAR(50),
    email VARCHAR(100) UNIQUE,
    edad INT
);
```

En este ejemplo:

- Se crea la tabla `Alumno`
- `id_alumno` es la clave primaria
- Se definen tipos de datos y restricciones

2. **ALTER** – Modificar estructuras existentes

Permite cambiar la estructura de una tabla ya creada, por ejemplo:

- Añadir columnas
- Eliminar columnas
- Modificar tipos de datos

Ejemplo: añadir una nueva columna

```sql
ALTER TABLE Alumno
ADD telefono VARCHAR(15);
```

3. **DROP** – Eliminar estructuras

Se utiliza para eliminar completamente un objeto de la base de datos.

Ejemplo:

```sql
DROP TABLE Alumno;
```

> [!WARNING]  
> Esta acción es irreversible: se pierde la estructura y los datos.

4. **TRUNCATE** – Vaciar una tabla

Elimina todos los registros de una tabla, pero mantiene su estructura.

```sql
TRUNCATE TABLE Alumno;
```

Diferencia clave:

- `DROP` elimina la tabla
- `TRUNCATE` solo elimina los datos

### Restricciones de integridad en DDL

El DDL permite definir reglas que garantizan la coherencia de los datos, muy importantes en el modelo relacional.

Principales restricciones:

`PRIMARY KEY`: identifica de forma única cada fila
`FOREIGN KEY`: establece relaciones entre tablas
`UNIQUE`: evita valores duplicados
`NOT NULL`: impide valores nulos
`CHECK`: impone condiciones
`DEFAULT`: asigna valores por defecto

Ejemplo con clave foránea:

```sql
CREATE TABLE Matricula (
    id_matricula INT PRIMARY KEY,
    id_alumno INT,
    asignatura VARCHAR(50),
    FOREIGN KEY (id_alumno) REFERENCES Alumno(id_alumno)
);
```

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%205.%20Bases%20de%20datos.png" alt="Bases de datos" width="600" height="auto"/>
    <p><em>Figura 5: Relaciones entre tablas. Fuente: Astera.com</em></p>
  </div>

<br>

## 5.2.8. Modelos de datos

Un modelo de datos es una **forma de describir cómo se estructuran, organizan y relacionan los datos** dentro de una base de datos. Define **qué datos se almacenan, cómo se relacionan entre sí y qué reglas deben cumplir**.

Los modelos de datos permiten pasar de una **necesidad del mundo real** a una **base de datos estructurada y coherente**.

### Niveles de abstracción de los modelos de datos

Los modelos de datos se pueden clasificar según su nivel de abstracción:

#### 1. Modelo conceptual

Es el modelo más abstracto, independiente de cualquier sistema gestor.

- Representa la información del mundo real
- Se centra en qué datos existen y cómo se relacionan
- No incluye detalles técnicos

Normalmente se representa mediante:

- Diagramas entidad–relación (E-R)

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%2014.%20Una%20relaci%C3%B3%20amb%20una%20altra%20relaci%C3%B3.png" alt="Bases de datos" width="600" height="auto"/>
    <p><em>Figura 6: Diagrama E-R. Fuente: Astera.com</em></p>
  </div>

#### 2. Modelo lógico

Describe la estructura de la base de datos **siguiendo un modelo concreto**, normalmente el **modelo relacional**, pero sin depender aún de un SGBD específico.

Características:

- Entidades → tablas
- Atributos → columnas
- Relaciones → claves foráneas
- Se definen claves primarias

Ejemplo:

- Tabla Customers(customerID, firstName, lastName, birthDate, moneySpent, anniversary)
- Tabla Orders(orderID, customerID, employeeID, productID, orderTotal, orderDate)

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%206.%20Bases%20de%20datos.png" alt="Bases de datos" width="600" height="auto"/>
    <p><em>Figura 7: Modelo lógico. Fuente: planetscale.com</em></p>
  </div>

#### 3. Modelo físico

Es el nivel más cercano a la implementación real. Depende del SGBD, incluye tipos de datos concretos y considera aspectos de rendimiento y almacenamiento. La implementación se realiza con el lenguaje de definición de datos.

<br>

## 5.2.9. Términos clave de las bases de datos

| Término        | Descripción                  |
| -------------- | ---------------------------- |
| Base de datos  | Conjunto organizado de datos |
| SGBD           | Software que gestiona la BD  |
| Tabla          | Estructura principal         |
| Registro       | Fila de la tabla             |
| Campo          | Columna de la tabla          |
| Clave primaria | Identificador único          |
| Clave foránea  | Relación entre tablas        |
| Dominio        | Valores permitidos           |
| Restricción    | Regla de integridad          |
| Vista          | Tabla virtual                |

<br>

## 5.2.10. Tipologias de relaciones

Se define el grado de una relación como el número de conjuntos de entidades que participan en el conjunto de relaciones, o lo que es lo mismo, el número de entidades que participan en una relación. Las relaciones en las que participan dos entidades son binarias o de grado dos. Si participan tres, serán ternarias o de grado tres. Los conjuntos de relaciones pueden tener cualquier grado, aunque lo ideal es tener relaciones binarias.

Las relaciones en las que solo participa una entidad se denominan de anillo o de grado uno; relacionan una entidad consigo misma y se denominan relaciones reflexivas. Por ejemplo, la entidad EMPLEADO puede tener una relación JEFE DE consigo misma: un empleado es JEFE DE muchos empleados y, a la vez, el jefe también es un empleado.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%206.%20Relacions%20de%20grau%201.png" alt="BD" width="450" height="auto"/>
    <p><em>Figura 8: Relacions de grau 1.</em></p>
  </div>

En la Figura 9 se muestra una relación de grado dos, que representa a un proveedor que suministra artículos, y otra de grado tres, que representa a un cliente de un banco que tiene varias cuentas, y cada una en una sucursal.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%207.%20Relacions%20de%20grau%202%20i%203.png" alt="BD" width="550" height="auto"/>
    <p><em>Figura 9: Relacions de grau 2 i 3.</em></p>
  </div

En el modelo E-R se representan ciertas restricciones a las que deben ajustarse los datos contenidos en una base de datos. Estas son las restricciones de las cardinalidades de asignación, que expresan el número de entidades a las que puede asociarse otra entidad mediante un conjunto de relaciones.

Las cardinalidades de asignación se describen para conjuntos binarios de relaciones. Son las siguientes:

- **1:1, uno a uno.** A cada elemento de la primera entidad le corresponde solo uno de la segunda entidad, y a la inversa. Por ejemplo, un cliente de un hotel ocupa una habitación, o un curso de alumnos pertenece a un aula, y a esa aula solo asiste ese grupo de alumnos. Véase la Figura 8.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%208.%20Representaci%C3%B3%20de%20relacions%201%20a%201.png" alt="BD" width="550" height="auto"/>
    <p><em>Figura 10: Representació de relacions 1 a 1.</em></p>
  </div>
  
- **1:N, uno a muchos.** A cada elemento de la primera entidad le corresponden uno o más elementos de la segunda entidad, y a cada elemento de la segunda entidad le corresponde solo uno de la primera entidad. Por ejemplo, un proveedor suministra muchos artículos (véase la Figura 9).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%209.%20Representaci%C3%B3%20de%20relacions%201%20a%20molts.png" alt="BD" width="550" height="auto"/>
    <p><em>Figura 11: Representació de relacions 1 a molts.</em></p>
  </div>

- **N:1, muchos a uno.** Es el mismo caso que el anterior pero a la inversa; a cada elemento de la primera entidad le corresponde un elemento de la segunda, y a cada elemento de la segunda entidad le corresponden varios de la primera.
  
- - **N:M, muchos a muchos.** Cada elemento de la primera entidad le corresponden muchos elementos de la segunda, y a cada elemento de la segunda entidad le corresponden varios de la primera.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%2010.%20Representaci%C3%B3%20de%20relacions%20molts%20a%20molts.png" alt="BD" width="550" height="auto"/>
    <p><em>Figura 12: Representació de relacions molts a molts.</em></p>
  </div>

La cardinalidad de una entidad sirve para conocer su grado de participación en la relación, es decir, el número de correspondencias en las que interviene cada elemento de la entidad. Mide la obligatoriedad de correspondencia entre dos entidades.

Se representa entre paréntesis indicando los valores máximo y mínimo: (máximo, mínimo). Los valores para la cardinalidad son: (0,1), (1,1), (0,N), (1,N) y (M,N). El valor 0 se indica cuando la participación de la entidad es opcional.

En la Figura 13, que se muestra a continuación, se representa el diagrama E-R en el que contamos con las siguientes entidades:

- **EMPLEADO** está formada por los atributos Núm. Emple, Apellido, Salario y Comisión, siendo el atributo Núm. Emple la clave principal (representada mediante subrayado).
- **DEPARTAMENTO** está formada por los atributos Núm. Depart, Nombre y Localidad, siendo el atributo Núm. Depart la clave principal.

Se han definido dos relaciones:

- La relación «pertenece» entre las entidades EMPLEADOS y DEPARTAMENTO, cuyo tipo de correspondencia es 1:N; es decir, a un departamento le pertenecen cero o más empleados (0,N). Un empleado pertenece a un departamento y solo a uno (1,1).
- La relación «responsable», que asocia la entidad EMPLEADO consigo misma. Su tipo de correspondencia es 1:N; es decir, un empleado es jefe de cero o más empleados (0,N). Un empleado tiene un jefe y solo uno (1,1). Véase la Figura 13.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/M0372_M0377_BBDD_ASIX/blob/main/BA1-RA1_RA2/images/Figura%2011.%20Diagrama%20E-R%20de%20les%20relacions%20entre%20departaments%20i%20empleats.png" alt="BD" width="950" height="auto"/>
    <p><em>Figura 13: Diagrama E-R de les relacions entre departaments i empleats.</em></p>
  </div

<br>

## 5.2.11. Redundancia de datos

La redundancia de datos se produce cuando la misma información se almacena varias veces dentro de una base de datos. Esto suele ocurrir cuando el diseño de la base de datos no está bien estructurado o no sigue correctamente los principios del modelo relacional.

Un ejemplo de redundancia seria la siguiente tabla mal diseñada:

| id_matricula | nombre_alumno | email_alumno                          | asignatura  |
| ------------ | ------------- | ------------------------------------- | ----------- |
| 1            | Ana López     | [ana@email.com](mailto:ana@email.com) | Matemáticas |
| 2            | Ana López     | [ana@email.com](mailto:ana@email.com) | Física      |

### Problemas derivados de la redundancia de datos

- **Inconsistencia de datos.** Si se modifica un dato en un registro y no se actualiza en los demás, la información queda incoherente. Por ejemplo, si Ana cambia su correo electrónico y solo se actualiza una fila, la base de datos contendrá dos correos diferentes para la misma persona.

- **Mayor consumo de almacenamiento.** Al repetir la misma información varias veces, se ocupa más espacio del necesario, especialmente en bases de datos grandes con miles de registros.

- **Dificultad de mantenimiento.** Las operaciones de actualización se vuelven más complejas, ya que hay que modificar múltiples filas en lugar de una sola.

- **Anomalías de actualización.** La redundancia provoca anomalías en la modificación de datos: inserció, borrado y actualización.

## 5.2.12. Integridad referencial

La **integridad referencial** es un conjunto de reglas que garantizan que las relaciones entre tablas de una base de datos sean **coherentes y válidas**. Su objetivo principal es asegurar que los valores de las **claves foráneas** siempre hagan referencia a registros existentes en la tabla relacionada.

En un modelo relacional, las tablas no funcionan de forma aislada, sino que están conectadas entre sí mediante relaciones. La integridad referencial evita que estas relaciones se rompan.

### Clave primaria y clave foránea

Para entender la integridad referencial es necesario recordar dos conceptos clave:

- **Clave primaria (Primary Key):** identifica de forma única cada registro de una tabla. Ejemplo: `id_alumno` en la tabla ALUMNOS.

- **Clave foránea (Foreign Key):** es un atributo que referencia la clave primaria de otra tabla. Ejemplo: `id_alumno` en la tabla MATRICULAS apunta a id_alumno en ALUMNOS.

#### Ejemplo: 

Supongamos las siguientes tablas:

**Tabla ALUMNOS**

| id_alumno | nombre      |
| --------- | ----------- |
| 1         | Ana López   |
| 2         | Carlos Ruiz |

**Tabla MATRICULAS**

| id_matricula | id_alumno | asignatura  |
| ------------ | --------- | ----------- |
| 1            | 1         | Matemáticas |
| 2            | 2         | Física      |

Aquí:

- `id_alumno` es clave primaria en ALUMNOS.
- `id_alumno` es clave foránea en MATRICULAS.

La integridad referencial obliga a que:

- Todo valor de `id_alumno` en MATRICULAS exista previamente en la tabla ALUMNOS.

#### Un ejemplo de violación de integridad referencial sería:

Si intentamos insertar el siguiente registro:

| id_matricula | id_alumno | asignatura |
| ------------ | --------- | ---------- |
| 3            | 5         | Química    |

Se produce un error porque **no existe ningún alumno con id = 5** en la tabla ALUMNOS.

Esto generaría un registro “huérfano”, es decir, una matrícula asociada a un alumno inexistente.

Existen diferentes técnicas que pueden emplear los sistemas gestores de bases de datos, aplicando estas **acciones referenciales**: RESTRICT, CASCADE, SET NULL o SET DEFAULT.

## 5.2.13. Formas normales

Las **formas normales** son un conjunto de reglas que se utilizan para **organizar correctamente las tablas de una base de datos relacional**, con el objetivo de:

- Reducir la redundancia de datos.
- Evitar anomalías de actualización.
- Mejorar la integridad y consistencia de la información.
- Facilitar el mantenimiento de la base de datos.

El proceso de aplicar estas reglas se denomina normalización.

### ¿Qué es la normalización?

La **normalización** es el proceso de dividir una base de datos en varias tablas relacionadas entre sí para que cada dato se almacene una sola vez y dependa únicamente de la clave primaria.

### Primera Forma Normal (1FN)

Una tabla está en **Primera Forma Normal** cuando:

- Todos los atributos contienen **valores atómicos** (no divisibles).
- No existen **grupos repetidos** ni listas dentro de una misma columna.
- Cada registro puede identificarse de forma única.

#### Ejemplo NO normalizado en 1FN

| id_alumno | nombre | asignaturas         |
| --------- | ------ | ------------------- |
| 1         | Ana    | Matemáticas, Física |

Problemas: 

- Hay varios valores en un mismo campo.
- No se pueden hacer consultas eficientes.
- No cumple el modelo relacional.

#### En 1FN

| id_alumno | nombre | asignatura  |
| --------- | ------ | ----------- |
| 1         | Ana    | Matemáticas |
| 1         | Ana    | Física      |

Ahora:

- Cada celda contiene un único valor.
- Los datos son atómicos.

### Segunda Forma Normal (2FN)

Una tabla está en **Segunda Forma Normal** cuando:

- Cumple la 1FN.
- Todos los atributos no clave dependen **completamente de la clave primaria**.

Esto es especialmente importante cuando la clave primaria es **compuesta** (formada por más de un atributo).

#### Ejemplo NO normalizado en 2FN

Tabla MATRICULAS:

| id_alumno | id_asignatura | nombre_alumno | nombre_asignatura |
| --------- | ------------- | ------------- | ----------------- |
| 1         | 1             | Ana           | Matemáticas       |

Problema:

- `nombre_alumno` depende solo de `id_alumno`.
- `nombre_asignatura` depende solo de `id_asignatura`.
- No dependen de la clave completa.

#### En 2FN

Se separan las tablas:

**ALUMNOS**
| id_alumno | nombre |
| --------- | ------ |
| 1         | Ana    |

**ASIGNATURAS**
| id_asignatura | nombre      |
| ------------- | ----------- |
| 1             | Matemáticas |

**MATRICULAS**
| id_alumno | id_asignatura |
| --------- | ------------- |
| 1         | 1             |

Ahora:

- Cada atributo depende completamente de su clave primaria.
- Se elimina redundancia.

### Tercera Forma Normal (3FN)

Una tabla está en Tercera Forma Normal cuando:

- Cumple la 2FN.
- No existen dependencias transitivas.

Esto significa que:

Un atributo no clave no debe depender de otro atributo no clave.

#### Ejemplo NO normalizado en 3FN

Tabla ALUMNOS:

| id_alumno | nombre | codigo_postal | ciudad    |
| --------- | ------ | ------------- | --------- |
| 1         | Ana    | 08001         | Barcelona |

Problema:

- `ciudad` depende de `codigo_postal`, no directamente de `id_alumno`.
- Existe dependencia transitiva.

#### En 3FN

Se separan las tablas:

**ALUMNOS**
| id_alumno | nombre | codigo_postal |
| --------- | ------ | ------------- |
| 1         | Ana    | 08001         |

**CODIGO_POSTALES**
| codigo_postal | ciudad    |
| ------------- | --------- |
| 08001         | Barcelona |

Ahora:

- Todos los atributos dependen directamente de la clave primaria.
- Se elimina dependencia transitiva.

## 5.2.15. Tipologia de datos

La tipología de datos hace referencia a los distintos tipos de datos que pueden almacenarse en una base de datos. Cada atributo de una tabla debe tener asociado un tipo de dato que define:

- Qué tipo de información puede almacenarse.
- El formato del valor.
- El espacio de almacenamiento necesario.
- Las operaciones que se pueden realizar sobre ese dato.

### Tipos numéricos

Se utilizan para almacenar valores numéricos sobre los que se pueden realizar operaciones matemáticas.

#### Ejemplos comunes:

| Tipo              | Descripción                   | Ejemplo |
| ----------------- | ----------------------------- | ------- |
| INT               | Números enteros               | 25      |
| SMALLINT          | Enteros pequeños              | 120     |
| BIGINT            | Enteros grandes               | 1000000 |
| DECIMAL / NUMERIC | Números con decimales exactos | 12.50   |
| FLOAT / DOUBLE    | Números reales aproximados    | 3.1416  |

### Tipos de texto (cadena de caracteres)

Se utilizan para almacenar información alfanumérica.

| Tipo       | Descripción       | Ejemplo             |
| ---------- | ----------------- | ------------------- |
| CHAR(n)    | Longitud fija     | "ES"                |
| VARCHAR(n) | Longitud variable | "Ana López"         |
| TEXT       | Texto largo       | Descripción extensa |

### Tipos de fecha y tiempo

Permiten almacenar información temporal y realizar operaciones relacionadas con fechas.

| Tipo                 | Descripción  | Ejemplo             |
| -------------------- | ------------ | ------------------- |
| DATE                 | Fecha        | 2025-03-21          |
| TIME                 | Hora         | 14:30:00            |
| DATETIME / TIMESTAMP | Fecha y hora | 2025-03-21 14:30:00 |

### Tipos booleanos (lógicos)

Se utilizan para representar valores de tipo verdadero o falso.

| Tipo    | Valores posibles |
| ------- | ---------------- |
| BOOLEAN | TRUE / FALSE     |

### Tipos especiales

Algunos SGBD incluyen tipos avanzados para necesidades específicas.

| Tipo | Uso                                        |
| ---- | ------------------------------------------ |
| BLOB | Archivos binarios (imágenes, vídeos, PDFs) |
| ENUM | Lista cerrada de valores posibles          |
| JSON | Datos estructurados en formato JSON        |
