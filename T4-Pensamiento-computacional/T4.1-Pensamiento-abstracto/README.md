<h1 align="center">4.1. Pensamiento abstracto
<div align="center">

</div>

## Contenido:

- [4.1.17. Ejemplos de abstracción](#4117-ejemplos-de-abstracción)
- [4.1.18. Abstracción y soluciones computacionales para situaciones específicas](#4118-abstracción-y-soluciones-computacionales-para-situaciones-específicas)
- [4.1.19. Abstracción desde una situación específica](#4119-abstracción-desde-una-situación-específica)
- [4.1.20. Mundo real y abstracción](#4120-mundo-real-y-abstracción)

---

## 4.1.17. Ejemplos de abstracción

El **pensamiento abstracto** significa reflexionar sobre eventos, ideas, atributos y relaciones de una manera general que **oculta todos los detalles innecesarios** de los objetos específicos.
Toda la información que no es necesaria para lograr un objetivo se elimina e ignora, y se implementa una técnica de **generalización**.

Un pensador concreto puede identificar y contar **dos gatos** y **dos coches**, mientras que un pensador **abstracto** puede identificar su relación común, que es el **número dos**.

El **arte abstracto**, como su nombre indica, es un ejemplo típico de abstracción. Una pintura abstracta representa un principio o idea, pero no se ocupa de la descripción detallada ni de la representación de la realidad.

La explicación de los diversos componentes de la **placa base** requiere el uso de **abstracción**.
Aunque la **RAM** y la **CPU** se consideran partes físicas fundamentales, se sabe que son **abstracciones de puertas lógicas y circuitos integrados** que contienen millones de transistores.

Un nivel de abstracción ocurre en la mayoría de los programas informáticos.
Hace décadas, un programador tenía que trabajar con las **instrucciones de bajo nivel del circuito** de la CPU y del ordenador utilizado.

Hoy en día, los **lenguajes de programación de alto nivel** permiten al usuario utilizar comandos y sintaxis similares al inglés, en los cuales **una sola instrucción corresponde a muchas instrucciones máquina**.

En el lenguaje de programación **Java**, ```System.out.println``` muestra un mensaje en la pantalla.
El usuario no necesita entender el funcionamiento del monitor ni de los distintos procedimientos, interfaces, controladores de la tarjeta gráfica y bibliotecas que se utilizan para crear los píxeles correspondientes en la pantalla.

## 4.1.18. Abstracción y soluciones computacionales para situaciones específicas

### Programación orientada a objetos

La **programación orientada a objetos (POO)** usa la **abstracción** y se basa en el principio de que todas las tareas cotidianas pueden considerarse como **entidades**.
Estas entidades son **objetos** o **eventos**.

- La **mesa** es un objeto donde cenamos.
- El **coche** es un objeto; tiene **ruedas** y el conductor puede **cambiar de marchas**.

La POO utiliza **objetos de programación** que describen:

- **Datos** (propiedades).
- **Comportamientos** (métodos).

Esto facilita la **reutilización de código** y la **abstracción**.
Hace que el desarrollo de software complejo sea más rápido, sencillo y facilite su mantenimiento.

Es una **evolución de la programación estructurada**, que se basaba en **procedimientos** que podían interactuar y compartir datos como bloques de construcción de programas.

| **Objeto car1** | **Objeto car2** |
|-----------------|-----------------|
| **Datos:**      | **Datos:**      |
| integer speed = 0; | String Colour = Black |
| integer gear = 1;  | String Equipment = Silver |
|                  | String Availability = True |
|                  | Integer ManufacturerStock = 0 |
| **Métodos:**    | **Métodos:**    |
| changeGear       | changeColour    |
| Accelerate       | changeEquipment |
| Brake            | Availability    |

#### Abstracción en este ejemplo

- Car1 se podría usar en un programa que **simula la experiencia de conducción**.
- Car2 se podría usar en un programa **para ventas**.

En cada caso, el programador oculta los detalles innecesarios y se concentra únicamente en las propiedades y comportamientos importantes para esa implementación.

Supongamos que un vendedor usa un programa que facilita su trabajo. Cuando un cliente elige un coche y finaliza la compra, se crea un nuevo objeto. Cada venta tiene algunos atributos únicos. El vendedor trabaja con una colección de artículos (coches). Esta colección está organizada de una manera particular para representar la venta de coches. Se pueden aplicar algunos operadores comunes a todos los elementos de la colección (añadir un coche, leer los detalles de un coche, etc.).

Así, una colección es una estructura de datos que consiste en los datos y los métodos predefinidos que operan sobre los datos. Una colección, tal como se usa en la guía de informática, es un tipo abstracto de datos como colas y pilas. Un Tipo Abstracto de Datos, o ADT, es un grupo de operaciones y datos. En los lenguajes orientados a objetos, una colección es un objeto que reúne y contiene muchos elementos en una sola estructura. Una colección se utiliza para añadir, almacenar, gestionar, recuperar, manipular y comunicar los datos mediante métodos predefinidos.

### Manipulación de objetos

Supongamos que un programador quiere crear un objeto llamado ```Vehicle1``` de tipo ```vehicle``` con los siguientes campos de datos: [Colour: "red" – Type: "car" – Engine: 2000]. Todos los objetos vehicle tienen los mismos campos de datos: ```Colour```, ```Type``` y ```Engine```.

El programador usará el método set para definir las propiedades del objeto en particular:

```
Vehicle1 = new vehicle (setColour = "red", 
                        setType = "car", 
                        setEngine = 2000)
```

Supongamos que el programador quiere recuperar información de este objeto. El programador usará el método ```get``` para recuperar un campo de datos en particular de este objeto:

```
Vehicle1.getColour   will return "red"
Vehicle1.getEngine   will return 2000
Vehicle1.getType     will return "car"
```

### Modelado y simulación

El **modelado matemático** se refiere a un proceso en el que un sistema se entiende lo suficientemente bien y los científicos lo describen usando lenguaje matemático. Un **conjunto de reglas matemáticas** se utiliza para describir el funcionamiento del sistema en particular. Está claro que el **modelo matemático es una abstracción del sistema real**. Un modelo matemático contiene solo los detalles, reglas y objetos necesarios para estudiar el sistema real o un aspecto de este.

Un modelo matemático podría transformarse en un algoritmo y luego en un programa que replique el comportamiento de un sistema real. Una simulación por computadora se ejecuta en una computadora y reproduce el comportamiento de un sistema real. La simulación utiliza un modelo matemático abstracto que se expresa como un modelo computacional (programa de computadora) para simular el sistema. Una simulación por computadora siempre se basa en un modelo computacional.

## 4.1.19. Abstracción desde una situación específica

Un programa modular es más fácil de entender y facilita el uso de la **abstracción**.
El programador puede concentrarse en lo importante e ignorar todos los detalles innecesarios.

La vida y la programación serían muy aburridas sin el uso de la abstracción.
Por ejemplo, una persona puede crear una lista de tareas para terminar hoy:

```
Go to school
Buy a CS book
Visit my uncle
```

Sin abstracción, la lista se vería más o menos así:

```
Wake up 
Eat breakfast 
Brush my teeth 
Put my jacket on
 ~ 
Return to home
```

Y así sucesivamente...

La tarea “**ir a la escuela**” podría dividirse en cientos o incluso miles de pasos.
Es imposible considerar cada detalle minúsculo antes de pasar al siguiente paso.
Así que la vida es más fácil cuando las tareas pequeñas e insignificantes se consideran parte de una tarea más amplia.

Los **procedimientos** y **subprocedimientos** facilitan la abstracción.
Por ejemplo, el siguiente programa puede llamar a un **subprocedimiento** llamado ```computeSomething()```.
Cuando este subprocedimiento es llamado desde el programa principal, ejecuta una secuencia de instrucciones y devuelve un valor.

Si el programador confía en el rendimiento de ```computeSomething()```, entonces no tiene que preocuparse por los detalles que contiene este subprocedimiento.

Así que: la **modularización facilita la abstracción**.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%208.%20Pensamiento%20computacional.png" alt="Sub-procedure program" width="650" height="auto"/>
    <p><em>Figura 8: Programa que contiene un subproceso. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

## 4.1.20. Mundo real y abstracción

Un **mapa temático** es una abstracción de la realidad que muestra la **distribución espacial** y enfatiza un tema en particular, como la distribución promedio de ingresos en un área geográfica específica.

Los **mapas topográficos** muestran abstracciones de características físicas seleccionadas del mundo tridimensional real a una escala reducida en dos dimensiones, ya sea en papel o en una pantalla.

Los **mapas políticos** están diseñados para mostrar datos como las fronteras de países y estados, y la ubicación de las principales ciudades. Estos mapas son una abstracción del territorio político.

En estos casos, ocurren diversos niveles de **abstracción**.
La Tierra es única, pero el punto de interés guía la manera en que los científicos representan su superficie en un trozo de papel.

Este enfoque de “**ignorancia selectiva**” facilita el estudio y la comprensión de componentes e interacciones específicas.
