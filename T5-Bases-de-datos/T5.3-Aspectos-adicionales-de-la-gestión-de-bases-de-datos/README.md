<h1 align="center">5.3. Aspectos adicionales de la gestión de bases de datos
<div align="center">

</div>

## Contenido:

- [5.3.1. Función de un administrador de BBDD](#531-función-de-un-administrador-de-BBDD)
- [5.3.2. Usuarios finales en una BBDD](#532-usuarios-finales-en-una-BBDD)
- [5.3.3. Métodos de recuperación de BBDD](#533-métodos-de-recuperación-de-BBDD)
- [5.3.4. Sistemas de bases de datos integrados](#534-sistemas-de-bases-de-datos-integrados)
- [5.3.5. Uso de las bases de datos](#535-uso-de-las-bases-de-datos)
- [5.3.6. Privacidad de los datos](#536-privacidad-de-los-datos)
- [5.3.7. Ética en la gestión de las bases de datos](#537-ética-en-la-gestión-de-las-bases-de-datos)
- [5.3.8. Data matching y data mining](#538-data-matching-y-data-mining)

---

## 5.3.1. Función de un administrador de BBDD

Un administrador de bases de datos (DBA) es la persona responsable de gestionar, mantener y proteger una base de datos para que funcione correctamente, sea segura y esté siempre disponible para los usuarios y aplicaciones.

Las funciones principales del administrador son: 

- **Instalación y configuración del sistema gestor de bases de datos:** configurar cuántos usuarios pueden conectarse simultáneamente a la base de datos de una plataforma educativa.
- **Gestión de usuarios y permisos:** en una BBDD concreta un profesor puede modificar notas, un alumno solo puede consultar sus calificaciones y un administrador tiene el control total sobre la BBDD.
- **Seguridad de los datos:** cifrar los datos personales con tal de cumplir normativa vigente en protección de datos.
- **Copias de seguridad y recuperación:** realizar copias automáticas cada noche del sistema.
- **Mantener y actualizar las versiones del SGBD.**

<br>

## 5.3.2. Usuarios finales en una BBDD

Los **usuarios finales** son las personas que **utilizan la base de datos para consultar o introducir información**, pero **no gestionan su estructura ni configuración interna**.

A diferencia del administrador de BBDD, los usuarios finales interactúan con la base de datos **a través de aplicaciones o interfaces gráficas**, no directamente con el sistema gestor.

<br>

## 5.3.3. Métodos de recuperación de BBDD

Los métodos de recuperación de bases de datos son los procedimientos que permiten restaurar la información cuando ocurre un fallo, error o pérdida de datos.

### Copias de seguridad (Backups)

Es el método más importante y más utilizado. Consiste en crear copias de los datos originales que se almacenan en un lugar seguro. Los tipos principales son: backup completo, backup incremental y backup diferencial.

#### Backup completo

Copia **toda la base de datos**. Es una restauración muy sencilla aunque ocupa mucho espacio y tarda mas tiempo en ejecutarse.

#### Backup incremental

Solo copia los **cambios realizados desde la última copia**. Es un tipo de copia rápido y ocupa poco espacio, la complejidad lógica de esta es mayor.

#### Backup diferencial

Copia todos los cambios realizados **desde el último backup completo**.

Ejemplo: 

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%207.%20Bases%20de%20datos.png" alt="SGBD" width="450" height="auto"/>
  </div>

- En la copia total del día 1 sólo están los archivos A, B, C, D, E y F.
- El día 3 se modifican B y F.
- El día 7 se modifica A y se crea G.
- El dia 10 se modifican B y E.
- El día 15 se modifican E y G, además se crea el archivo H.
- El día 21 se elimina B, se modifica A y se crea el archivo nuevo I.
- El día 28 se modifican A y H, además se crea también J.
- El día 29 se modifican I y J, eliminando C.

Considerando que únicamente tenemos los ficheros que hemos comentado anteriormente. Cuando un fichero se modifique a la nueva versión indicala de la siguiente manera: A', A'', ...

Para simplificar la tarea suponemos: 
- Los dias laborales son de lunes a sábado.
- Cada mes los únicos dias festivos son los domingos.

### Logs de transacciones

Los **logs** registran todas las operaciones realizadas en la base de datos. Gracias a ellos se puede: 

- Repetir operaciones válidas (REDO)
- Deshacer operaciones incorrectas (UNDO)

Esto permite recuperar la base de datos hasta un **punto exacto en el tiempo.**

<br>

## 5.3.4. Sistemas de bases de datos integrados

Un **sistema de base de datos integrado** es aquel en el que la base de datos **forma parte de un sistema informático mayor**, trabajando junto con otras aplicaciones y servicios para gestionar la información de forma unificada.

No funciona de manera aislada, sino que está **conectado con diferentes módulos y programas** que comparten los mismos datos.

<br>

## 5.3.5. Uso de las bases de datos

Las **bases de datos** se utilizan para **almacenar, organizar, gestionar y recuperar información de forma eficiente y segura**.

<br>

## 5.3.6. Privacidad de los datos

La **privacidad de los datos** se refiere al **derecho de las personas a controlar cómo se recopila, almacena, utiliza y comparte su información personal** dentro de sistemas informáticos y bases de datos.

En el contexto de las bases de datos, la privacidad implica que los datos personales deben ser **protegidos contra accesos no autorizados y usos indebidos**.

## 5.3.7. Ética en la gestión de las bases de datos

La **ética en la gestión de bases de datos** se refiere al conjunto de **principios morales y normas de conducta** que deben guiar el uso, almacenamiento y tratamiento de la información.

No todo lo que es técnicamente posible es éticamente correcto. Por eso, los profesionales y usuarios deben actuar de forma **responsable, transparente y respetuosa** con los datos.

## 5.3.8. Data matching y data mining

Las bases de datos no solo se utilizan para almacenar información, sino también para **analizar y relacionar datos con el objetivo de obtener conocimiento útil**.

Dos técnicas importantes en este contexto son:

- Data matching (emparejamiento de datos): consiste en comparar datos procedentes de diferentes fuentes para identificar registros que corresponden a la misma persona, objeto o entidad.
- Data mining (minería de datos): proceso de analizar grandes volúmenes de datos para descubrir patrones, relaciones o tendencias ocultas.
