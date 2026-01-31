<h1 align="center">2.3. Sistemas operativos y sistemas de aplicación
<div align="center">

</div>

## Contenido:

- [2.3.1. Describa las principales funciones de un sistema operativo](#231-describa-las-principales-funciones-de-un-sistema-operativo)
- [2.3.2. Resuma el uso de varios programas de aplicación](#232-resuma-el-uso-de-varios-programas-de-aplicación)
- [2.3.3. Identifique características comunes de las aplicaciones](#233-identifique-características-comunes-de-las-aplicaciones)

---

<br>

## 2.3.1. Describa las principales funciones de un sistema operativo

Un sistema operativo (SO) es el software fundamental que gestiona los recursos de hardware y software de un ordenador y proporciona servicios comunes para los programas informáticos. Actúa como intermediario entre el usuario y el hardware del ordenador, garantizando un funcionamiento eficiente y seguro del sistema.

Las funciones de un sistema operativo son múltiples y garantizan que el sistema funcione de manera fluida, eficiente y segura. A continuación, se analizan las distintas funciones críticas de un sistema operativo, mostrando cómo mantiene la integridad del sistema mientras ejecuta procesos en segundo plano y gestiona los recursos.

### Gestión de la memoria

La gestión de la memoria es una función fundamental de un sistema operativo (SO) e implica el control y la coordinación de la memoria principal (RAM) de un ordenador. El SO se asegura de que la memoria se asigne de forma eficiente a los procesos y aplicaciones, mantiene la estabilidad del sistema y protege las áreas de memoria frente a accesos no autorizados.

Cuando se abre o ejecuta una aplicación, el SO la carga en la RAM. Primero, localiza la aplicación en el dispositivo de almacenamiento (normalmente un disco duro o una unidad de estado sólido) y lee el archivo ejecutable (.exe en Windows o .app en Mac). Este archivo contiene todo el código de la aplicación y sus datos iniciales.

A continuación, el SO asigna el espacio de memoria necesario para la aplicación. Esto incluye espacio para el código, los datos y cualquier otro recurso requerido. El SO garantiza que la aplicación disponga de suficiente espacio para ejecutarse sin interferir con otros procesos.

Una vez que la aplicación está cargada en la RAM, el SO gestiona continuamente la memoria para asegurar un funcionamiento eficiente y la estabilidad del sistema. Mientras la aplicación se está ejecutando, el SO puede asignar y liberar memoria dinámicamente según las necesidades de la aplicación. Además, el SO se asegura de que cada proceso opere dentro de su propio espacio de memoria. Esto evita que los procesos interfieran entre sí, lo que mejora la seguridad y la estabilidad del sistema.

Si las aplicaciones requieren más memoria de la disponible en la RAM, el SO puede utilizar **memoria virtual** para mantener el sistema funcionando correctamente. La memoria virtual consiste en que el SO asigna parte del espacio del disco duro (HDD) o de la unidad de estado sólido (SSD) para utilizarlo como si fuera RAM. Esta no es una situación ideal, ya que el acceso a un dispositivo de almacenamiento es mucho más lento que el acceso a la RAM; sin embargo, al intercambiar en la RAM los procesos con mayor prioridad y mover a la memoria virtual los de menor prioridad, el SO puede seguir ejecutando el sistema a un nivel óptimo.

> [!NOTE]  
> **Memoria virtual:** una técnica de gestión de memoria que permite a un ordenador utilizar más memoria de la que está físicamente disponible mediante la transferencia temporal de datos desde la RAM al almacenamiento en disco, lo que posibilita la ejecución de programas más grandes y la multitarea.

> [!TIP]  
> Piensa en la gestión de la memoria como en la organización de libros en una estantería. El sistema operativo asigna a cada libro (proceso) su propio espacio en la estantería (memoria). Del mismo modo que no permitirías que los libros se superpongan o se mezclen, el sistema operativo se asegura de que cada proceso tenga su propia área protegida en la memoria.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2071.%20Relaci%C3%B3n%20entre%20memoria%20virtual%20y%20memoria%20f%C3%ADsica.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 48: Relación entre memoria virtual y memoria física. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

### Gestión de archivos

La gestión de archivos es una función crucial de un sistema operativo (SO) y comprende el almacenamiento, la recuperación, la organización y la manipulación de datos en los dispositivos de almacenamiento. El SO proporciona una forma estructurada de gestionar archivos y directorios, garantizando la estabilidad y la seguridad del sistema.

El SO emplea un sistema de archivos jerárquico para organizar los archivos de manera lógica y estructurada. Los archivos se organizan en directorios (o carpetas), que pueden contener a su vez otros directorios, creando una estructura en forma de árbol. Esta organización facilita a los usuarios y a las aplicaciones la localización y gestión de los datos.

El SO permite una serie de operaciones estándar que los usuarios y las aplicaciones pueden realizar sobre archivos y directorios, entre las que se incluyen: crear nuevos archivos y directorios; leer y escribir datos en archivos; eliminar archivos; cambiar el nombre de archivos; y mover o copiar archivos y directorios a diferentes ubicaciones.

Para garantizar la coherencia y evitar conflictos, el SO impone reglas para la denominación de archivos, asegurando que no existan dos archivos con el mismo nombre dentro de un mismo directorio. Los archivos suelen tener extensiones, como .jpg o .exe, que indican el tipo de archivo y la aplicación asociada, aunque, dependiendo de la configuración del sistema operativo, estas extensiones pueden estar ocultas para el usuario.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2072.%20Windows%20File%20Explorer%20view.png" alt="Walden" width="350" height="auto"/>
    <p><em>Figura 49: Windows File Explorer. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2073.%20MacOS%20finder%20view.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 50: MacOS finder view. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2074.%20Los%20tipos%20de%20archivo%20m%C3%A1s%20comunes.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 51: Tipología de archivos. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>
  
Al gestionar el almacenamiento de archivos, el sistema operativo utiliza diversos métodos para mejorar el rendimiento; esto incluye la forma en que asigna los archivos en el medio de almacenamiento físico, gestiona el espacio libre y realiza tareas de mantenimiento sobre los datos almacenados.

Una tarea de mantenimiento importante es la desfragmentación, que reorganiza los datos fragmentados en un disco duro (HDD). La fragmentación se produce con el tiempo a medida que los archivos se crean, modifican y eliminan, provocando que queden dispersos en diferentes sectores del disco. La **desfragmentación** tiene como objetivo reorganizar estos fragmentos de archivos en secuencias contiguas, mejorando así el rendimiento del sistema.

> [!NOTE]  
> **Extensión de archivo:** un sufijo al final del nombre de un archivo que indica el tipo de archivo y el programa asociado para abrirlo o procesarlo (por ejemplo, .docx para documentos de Word, .jpg para imágenes).
> **Desfragmentación:** el proceso de reorganizar los datos en un disco duro para que los archivos se almacenen en bloques contiguos, reduciendo la fragmentación y mejorando la velocidad de acceso y el rendimiento general del sistema.

### Gestión de dispositivos

La gestión de dispositivos del sistema operativo garantiza que los dispositivos de hardware funcionen de manera eficiente y se integren sin problemas con las aplicaciones de software. El SO controla y coordina el uso de componentes de hardware como impresoras, unidades de disco, pantallas, teclados e interfaces de red mediante un software especializado llamado controladores de dispositivos (device drivers). Los **controladores de dispositivos** son programas esenciales que permiten al SO comunicarse con el hardware conectado. Cada componente de hardware requiere un controlador específico para funcionar de forma correcta y eficiente. El SO utiliza estos controladores para proporcionar una interfaz uniforme, permitiendo que las aplicaciones interactúen con el hardware sin necesidad de conocer sus características específicas.

- **Controladores de dispositivos (device drivers):** programas de software especializados que permiten al sistema operativo comunicarse y controlar dispositivos de hardware, como impresoras, tarjetas gráficas o adaptadores de red, proporcionando las instrucciones y protocolos necesarios.
- **Buffering (almacenamiento en búfer):** proceso de almacenamiento temporal de datos en un área de memoria (búfer) mientras se transfieren entre dos dispositivos o procesos, lo que ayuda a gestionar las diferencias en la velocidad de transferencia de datos y garantiza un funcionamiento fluido y sin interrupciones.
- **Caching (caché):** proceso de almacenamiento temporal de datos de acceso frecuente en un área de almacenamiento de alta velocidad (caché) para reducir el tiempo de acceso y mejorar el rendimiento del sistema, permitiendo una recuperación más rápida de los datos.
- **Spooling:** proceso de poner en cola datos o tareas en un búfer, normalmente para dispositivos de entrada/salida como impresoras, de modo que puedan procesarse de forma secuencial y a su propio ritmo, permitiendo que el sistema continúe trabajando en otras tareas simultáneamente.
- **Plug and Play (PnP):** tecnología que permite al sistema operativo detectar, configurar e instalar automáticamente los controladores de nuevos dispositivos de hardware cuando se conectan al ordenador, haciendo posible su funcionamiento sin necesidad de una configuración manual por parte del usuario.

El SO también se encarga de la gestión de entrada/salida (E/S) para coordinar la transferencia de datos entre el ordenador y los dispositivos periféricos. Para ello, emplea técnicas como el buffering, el caching y el spooling con el fin de optimizar el rendimiento y la fiabilidad del sistema. El buffering utiliza áreas de almacenamiento temporal para mantener los datos mientras se transfieren entre dispositivos, adaptándose a las diferencias de velocidad entre la CPU y los periféricos. El caching almacena datos de uso frecuente para reducir los tiempos de acceso y mejorar la eficiencia general del sistema. El spooling pone los datos en cola y los envía de forma ordenada a dispositivos como las impresoras, que no pueden manejar flujos de datos intercalados.

Los sistemas operativos modernos han incorporado formas más sencillas y amigables de conectar dispositivos, como la tecnología Plug and Play (PnP). Gracias a PnP, el SO puede identificar automáticamente un dispositivo que se ha conectado, instalar los controladores necesarios y configurar los ajustes sin necesidad de intervención del usuario. Además, el SO es capaz de detectar errores y actuar para recuperarse de ellos, reiniciando el dispositivo, reinicializando los controladores o notificando al usuario del problema.

Por último, el SO proporciona mecanismos de seguridad y control de acceso para garantizar que solo los usuarios y procesos autorizados puedan acceder a determinados dispositivos, manteniendo la integridad y la seguridad del sistema.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2075.%20Device%20drivers%20como%20intermediarios%20entre%20el%20sistema%20operativo%20y%20el%20hardware.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 52: Device drivers como intermediarios entre el sistema operativo y el hardware. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

### Planificación (Scheduling)

El sistema operativo planifica la ejecución de múltiples procesos determinando qué proceso se ejecuta en cada momento. El **planificador (scheduler)** es el responsable de asignar tiempo de CPU a los procesos, garantizando un uso eficiente y justo de los recursos del sistema. Esta función es fundamental en entornos de multitarea, donde múltiples aplicaciones y procesos en segundo plano se ejecutan de forma concurrente. Mediante la implementación de distintos algoritmos de planificación, el SO busca optimizar el rendimiento, reducir los tiempos de espera y mantener la estabilidad del sistema.

En la sección A1.3.3 se profundizará en enfoques concretos de planificación, como first come, first served (primero en llegar, primero en ser atendido), round robin, planificación por colas multinivel y planificación por prioridades. Cada método presenta sus propias ventajas y compromisos, y su idoneidad depende de los requisitos y objetivos específicos del sistema.

#### Seguridad

La seguridad del sistema operativo está diseñada para proteger la integridad, la confidencialidad y la disponibilidad de la información y de los recursos del sistema informático. Para ello, incorpora mecanismos que protegen frente a amenazas, evitan accesos no autorizados y garantizan que los usuarios y las aplicaciones puedan operar de forma segura.

#### Autenticación de usuarios

La autenticación de usuarios puede utilizarse de diversas formas. Inicialmente, el SO puede requerir que el usuario se autentique para iniciar sesión en el sistema, solicitando credenciales como un nombre de usuario y una contraseña, datos biométricos o tokens de seguridad. Una vez iniciada la sesión, y en función de la configuración del usuario, el SO puede permitir o denegar el acceso a determinados archivos, carpetas o aplicaciones del sistema. Esto posibilita que un mismo sistema tenga múltiples usuarios con distintos niveles de acceso, como un administrador y un usuario estándar.

> [!NOTE] 
> **Tokens de seguridad:** dispositivos físicos o digitales que generan o almacenan credenciales de autenticación, como contraseñas de un solo uso o claves criptográficas, utilizados para verificar la identidad de un usuario y asegurar el acceso a sistemas, redes o servicios en línea.

#### Cifrado

El sistema operativo puede proporcionar herramientas y marcos de trabajo para cifrar archivos, canales de comunicación y dispositivos. El cifrado garantiza que los datos, incluso si son interceptados o accedidos por personas no autorizadas, no puedan ser leídos sin la clave de descifrado correspondiente.

#### Auditoría y monitorización

Todas las actividades del sistema, como los inicios de sesión de los usuarios, el acceso a archivos, los errores del sistema y las acciones del administrador, son registradas por el SO en archivos de registro (logs). Estos registros se utilizan con fines de auditoría y monitorización, y pueden ayudar a los administradores a detectar actividades sospechosas y posibles brechas de seguridad. Asimismo, también pueden emplearse para identificar problemas y áreas de mejora en el rendimiento del sistema.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2076.%20Visor%20de%20eventos.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 53: Visor de eventos. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### Protección contra malware

El sistema operativo incluye mecanismos para detectar y prevenir infecciones de malware y accesos no autorizados. Entre estos mecanismos se encuentran el software antivirus, los cortafuegos (firewalls) y los sistemas de detección de intrusiones (IDS). Estas herramientas analizan la presencia de software malicioso, supervisan el tráfico de red y bloquean intentos de acceso no autorizados, protegiendo el sistema frente a virus, gusanos, troyanos y otras amenazas maliciosas.

- **Malware:** término general que engloba cualquier software diseñado con intención maliciosa, como virus, gusanos, troyanos, spyware y ransomware, que puede dañar sistemas, robar datos o interrumpir el funcionamiento normal.
- **Virus:** programas de software malicioso que se adjuntan a archivos o programas legítimos y se propagan a otros archivos o sistemas, a menudo causando daños o interrupciones.
- **Gusanos (worms):** malware autorreplicante que se propaga a través de redes sin necesidad de adjuntarse a otros programas, explotando vulnerabilidades para infectar múltiples sistemas.
- **Troyanos (trojans):** programas engañosos que aparentan ser legítimos, pero contienen código malicioso oculto que puede crear puertas traseras, robar datos o causar daños una vez que el usuario los ejecuta.

### Contabilidad (Accounting)

Las funciones de contabilidad del sistema operativo son esenciales para supervisar y gestionar el uso de los recursos del sistema. Estas funciones registran el consumo de recursos por parte de usuarios y procesos, proporcionando datos valiosos para que los administradores del sistema analicen el rendimiento, asignen costes y optimicen la utilización de los recursos. Los principales aspectos de la contabilidad en un SO incluyen:

#### Seguimiento del uso de recursos

El SO monitoriza de forma continua el consumo de distintos recursos por parte de usuarios y procesos. Esto incluye el seguimiento de:

- **Uso de la CPU:** la cantidad de tiempo de CPU consumido por cada proceso o usuario.
- **Uso de la memoria:** la cantidad de memoria RAM asignada y utilizada por cada proceso.
- **Uso del disco:** el espacio de almacenamiento ocupado por los archivos y directorios pertenecientes a cada usuario.
- **Uso de red:** el volumen de datos enviados y recibidos a través de la red por cada proceso o usuario.

#### Contabilidad de procesos

La contabilidad de procesos implica mantener registros detallados de cada proceso que se ejecuta en el sistema. Estos registros incluyen información como:

- **Identificador de proceso (process ID):** un identificador único para cada proceso.
- **Identificador de usuario (user ID):** el identificador del usuario que inició el proceso.
- **Tiempo de ejecución:** el tiempo total de CPU utilizado por el proceso.
- **Tiempos de inicio y fin:** marcas de tiempo que indican cuándo comenzó y cuándo finalizó el proceso.
- **Consumo de recursos:** detalles sobre la cantidad de memoria, E/S de disco y otros recursos utilizados por el proceso.

#### Contabilidad de usuarios

La contabilidad de usuarios registra el uso de recursos por parte de usuarios individuales o grupos de usuarios. Esta información es fundamental para:

- **Asignación de costes:** en entornos multiusuario, como universidades o empresas, los datos de uso de recursos pueden emplearse para asignar costes a distintos departamentos o proyectos en función de su consumo.
- **Gestión de cuotas:** aplicar límites al uso de recursos para evitar que un único usuario monopolice los recursos del sistema; esto puede incluir cuotas de disco (limitando el espacio de almacenamiento que puede usar un usuario) y cuotas de memoria.

#### Monitorización del rendimiento

Las funciones de contabilidad del SO son clave para la monitorización del rendimiento. Mediante el análisis de los datos de uso de recursos, los administradores del sistema pueden identificar:

- **Cuellos de botella:** áreas donde los recursos están siendo sobreutilizados, provocando una degradación del rendimiento.
- **Infrautilización:** recursos que se usan poco, lo que indica posibles áreas de optimización.
- **Tendencias:** patrones de uso de recursos a lo largo del tiempo, que pueden servir para la planificación de capacidad y futuras ampliaciones del sistema.

#### Auditoría e informes

El SO genera informes detallados a partir de los datos de contabilidad recopilados. Estos informes pueden utilizarse para:

- **Auditoría:** garantizar el cumplimiento de las políticas de la organización y de los requisitos normativos mediante la revisión del uso de recursos y los patrones de acceso.
- **Análisis de seguridad:** detectar actividades inusuales o sospechosas mediante el análisis de anomalías en el uso de recursos.
- **Gestión de recursos:** tomar decisiones informadas sobre la asignación de recursos, la configuración del sistema y futuras inversiones.

#### Facturación y repercusión de costes (Billing and chargeback)

En entornos donde el uso de recursos debe facturarse a usuarios o departamentos individuales, como en servicios de computación en la nube o instituciones académicas, las funciones de contabilidad del SO permiten:

- **Facturación basada en el uso:** cobrar a los usuarios en función de su consumo real de recursos, como horas de CPU, uso de memoria y ancho de banda de red.
- **Repercusión de costes (chargeback):** asignar los costes a distintos departamentos o proyectos según su uso de recursos, fomentando la responsabilidad y el uso eficiente de los recursos.

### Interfaz gráfica de usuario (GUI)

Al ofrecer elementos visuales como ventanas, iconos, menús y punteros, el sistema operativo proporciona un entorno fácil de usar para interactuar con el ordenador y permite al usuario ejecutar comandos, gestionar archivos y ejecutar aplicaciones.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2077.%20Ubuntu%20GUI.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 54: Ubuntu GUI. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### Elementos de la interfaz de usuario

Los elementos de la interfaz de usuario proporcionados por el sistema operativo permiten al usuario interactuar con el sistema de forma intuitiva. Estos elementos incluyen **ventanas**, que muestran el contenido de aplicaciones, documentos o información del sistema. Los **iconos** ofrecen una representación gráfica de aplicaciones, archivos y funciones del sistema, proporcionando un acceso rápido a los elementos más utilizados. Los **menús** presentan listas de comandos u opciones para acceder a distintas funciones, facilitando la navegación y el uso del sistema. Los **punteros**, normalmente representados por una flecha o cursor, se controlan mediante un dispositivo de entrada como el ratón y permiten seleccionar, arrastrar e interactuar con los elementos de la interfaz gráfica de forma fluida.

#### Gestión de aplicaciones

La interfaz gráfica facilita la gestión y la interacción con múltiples aplicaciones, mejorando la productividad y la experiencia del usuario. El cambio de tareas permite moverse rápidamente entre aplicaciones abiertas, con funciones como la barra de tareas o el conmutador de aplicaciones (Alt + Tab), que hacen posible una navegación eficiente. La gestión de ventanas ayuda a organizar el espacio de trabajo mediante la colocación, superposición y organización en mosaico de las ventanas. Funciones como el ajuste de ventanas a los bordes o esquinas de la pantalla crean un efecto de pantalla dividida para la multitarea. El entorno de escritorio, donde los usuarios pueden colocar iconos, accesos directos y widgets, permite personalizar y organizar el espacio de trabajo según las preferencias individuales.

#### Gestión de archivos y del sistema

La interfaz gráfica simplifica las tareas de gestión de archivos y del sistema mediante herramientas e interfaces visuales. Una herramienta de gestión de archivos basada en GUI, como el Explorador de archivos, permite navegar por los directorios, ver las propiedades de los archivos y realizar operaciones como copiar, mover, eliminar y cambiar el nombre de archivos y carpetas. Esta herramienta suele incluir funciones de búsqueda, ordenación y filtrado para facilitar la gestión de archivos. La GUI también proporciona acceso a la configuración del sistema y a los paneles de control, permitiendo a los usuarios configurar el hardware, el software y las preferencias del sistema a través de interfaces gráficas intuitivas. La funcionalidad de **arrastrar y soltar** ofrece un método sencillo y cómodo para transferir archivos y datos entre aplicaciones y directorios.

#### Accesibilidad

La interfaz gráfica incluye funciones que mejoran la accesibilidad para usuarios con discapacidad, garantizando que el sistema sea utilizable por todas las personas. Los **lectores de pantalla** convierten el texto y los elementos de la interfaz gráfica en voz o en Braille, ayudando a los usuarios con discapacidad visual a navegar por el sistema. Los **temas de alto contraste** y los **ampliadores de pantalla** mejoran la legibilidad para usuarios con baja visión.

Los **atajos de teclado** permiten realizar acciones rápidamente sin depender del ratón o del panel táctil, lo que beneficia a usuarios con movilidad reducida.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2078.%20MacOS%20accesibilidad.png" alt="Walden" width="550" height="auto"/>
    <p><em>Figura 55: Accesibilidad MacOS. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### Retroalimentación visual

La interfaz gráfica de usuario proporciona retroalimentación visual inmediata a las acciones del usuario, mejorando la experiencia general de uso. Los **indicadores de progreso**, como las barras de progreso y las animaciones de carga, informan a los usuarios sobre el estado de operaciones en curso, como transferencias de archivos o instalaciones de software. Las **notificaciones**, en forma de mensajes emergentes y alertas, mantienen a los usuarios informados sobre eventos importantes, actualizaciones o errores. Los **tooltips** (pequeños cuadros de texto informativos que aparecen cuando el usuario pasa el cursor sobre iconos o elementos de la interfaz) ofrecen información adicional u orientación.

#### Personalización y adaptación

La interfaz gráfica permite a los usuarios personalizar su entorno informático según sus preferencias, haciendo que el sistema sea más agradable y eficiente de utilizar. Los usuarios pueden cambiar la apariencia de la GUI seleccionando distintos temas, fondos de pantalla y estilos de ventana, creando una experiencia más personalizada. Los **widgets** y **gadgets** —pequeñas aplicaciones que proporcionan acceso rápido a información y herramientas como el tiempo, calendarios y monitores del sistema— mejoran la funcionalidad y la estética del escritorio. Estas opciones de personalización permiten a los usuarios adaptar su espacio de trabajo a sus necesidades y preferencias, aumentando la satisfacción y la productividad generales.

### Virtualización

La **virtualización** es una característica clave de los sistemas operativos modernos que permite ejecutar múltiples **máquinas virtuales (VM)** en una sola máquina física. Cada máquina virtual funciona de manera independiente, con su propio sistema operativo y aplicaciones. El sistema operativo gestiona este proceso mediante un hipervisor, que asigna tiempo de CPU, memoria y almacenamiento a cada VM, garantizando un uso eficiente de los recursos y permitiendo que cada máquina virtual funcione como si estuviera en un equipo físico independiente.

> [!NOTE] 
> - **Hipervisor:** software que crea y gestiona máquinas virtuales permitiendo que múltiples sistemas operativos se ejecuten simultáneamente en una sola máquina física, compartiendo los recursos de hardware subyacentes.
> - **Balanceo de carga (load balancing):** proceso de distribución del tráfico de red o de aplicaciones entre varios servidores o recursos para garantizar un rendimiento, fiabilidad y disponibilidad óptimos, evitando que un único servidor se sobrecargue.

La virtualización mejora la seguridad y la estabilidad al aislar las máquinas virtuales entre sí, evitando que los problemas de una VM afecten a las demás. También permite la creación de **instantáneas (snapshots)** y copias de seguridad, lo que posibilita guardar el estado actual de una máquina virtual y restaurarlo si es necesario. Las **migraciones en vivo**, que trasladan máquinas virtuales de un host físico a otro sin interrumpir los servicios, son otra característica fundamental que facilita el balanceo de carga y el mantenimiento del hardware.

Además, la virtualización da soporte a la **recuperación ante desastres** y a los **servicios en la nube**. Al permitir que las máquinas virtuales se respalden y restauren fácilmente, el sistema operativo garantiza que las aplicaciones y los datos críticos puedan recuperarse con rapidez en caso de fallo. La virtualización también posibilita el escalado dinámico de la infraestructura informática en entornos cloud, permitiendo a las organizaciones adaptarse con rapidez a cambios en la demanda.

### Redes (Networking)

Los sistemas operativos gestionan y facilitan la comunicación en red. Una de las funciones principales del SO en el ámbito de las redes es establecer y mantener conexiones de red. El sistema operativo gestiona las interfaces y los protocolos de red, permitiendo que los dispositivos se conecten a redes de área local (LAN), redes de área amplia (WAN) y a Internet. Configura los parámetros de red, asigna direcciones IP mediante **DHCP (Dynamic Host Configuration Protocol)** y gestiona el hardware subyacente, como las tarjetas de red (NIC), asegurando una comunicación eficaz entre dispositivos.

El SO también proporciona servicios esenciales para la transmisión de datos y la comunicación entre dispositivos. Implementa diversos protocolos de red, como **TCP/IP (Transmission Control Protocol / Internet Protocol)**, que regulan cómo se fragmentan, direccionan, transmiten, enrutan y reciben los datos. El sistema operativo garantiza la integridad de los datos y una transmisión eficiente mediante el control de errores, el control de flujo y la prevención de la congestión. Además, da soporte a protocolos y servicios de nivel superior, como **HTTP** para la navegación web, **FTP** para la transferencia de archivos y **SMTP** para la comunicación por correo electrónico, facilitando la interacción fluida entre aplicaciones y recursos de red.

La **seguridad y el control de acceso** son funciones críticas de red gestionadas por el sistema operativo. El SO emplea **cortafuegos**, **cifrado** y **mecanismos de autenticación** para proteger los datos durante su transmisión por la red. Los cortafuegos supervisan y controlan el tráfico de red entrante y saliente según reglas de seguridad predefinidas, ayudando a prevenir accesos no autorizados y ataques. El sistema operativo también es compatible con **redes privadas virtuales (VPN)**, que cifran los datos y crean conexiones seguras sobre redes públicas, garantizando la privacidad y la seguridad de los usuarios remotos. Estas medidas protegen las comunicaciones de red y aseguran que solo los usuarios y dispositivos autorizados puedan acceder a los recursos de la red.

<br>

## 2.3.2. Resuma el uso de varios programas de aplicación

Un sistema informático tiene la capacidad de ejecutar al menos una aplicación de software, que ha sido instalada por el fabricante para completar algunas tareas predefinidas. Por ejemplo, una cámara digital es por sí sola un sistema informático. Consta tanto de componentes de hardware como de software y sigue el modelo de entrada, proceso, salida y almacenamiento descrito en el ejemplo de la sección 2.1.1. Los componentes de software de la cámara digital están preinstalados en el momento de su fabricación y completan tareas predefinidas (por ejemplo, cuando se presiona el botón del obturador, se ejecuta el software responsable de capturar la imagen en formato digital y almacenarla en memoria después de procesarla). Estos componentes de software de la cámara digital solo pueden modificarse recibiendo versiones actualizadas del fabricante.

Sin embargo, los sistemas informáticos incluyen dispositivos como ordenadores de sobremesa y portátiles, tabletas, teléfonos inteligentes, etc. Estos permiten al usuario instalar una gran cantidad de aplicaciones de software en ellos. Esto posibilita el uso de una variedad de aplicaciones en lugar de limitarse a completar una única tarea predefinida. Las principales aplicaciones de software que pueden instalarse en dichos sistemas informáticos incluyen:

- Procesadores de texto
- Hojas de cálculo
- Sistemas de gestión de bases de datos
- Navegadores web
- Correo electrónico
- Diseño asistido por computadora (CAD)
- Software de procesamiento gráfico

<br>

## 2.3.3. Identifique características comunes de las aplicaciones

Las aplicaciones de software instaladas en los sistemas informáticos suelen incluir una **interfaz gráfica de usuario (GUI)** para permitir que el usuario interactúe con ellas de varias formas, en lugar de solo escribir comandos. Una GUI incluye componentes como íconos gráficos e indicadores visuales, así como barras de herramientas, menús y cuadros de diálogo. Estos permiten que la interacción entre el usuario y la aplicación de software se realice de manera más fluida mediante la manipulación directa de los elementos gráficos.

Las aplicaciones de software han mejorado enormemente a lo largo de los años. Las primeras aplicaciones de software funcionaban con comandos que debían escribirse, lo que llamamos interfaces de **línea de comandos (CLI)**. Más tarde se aprovecharon las ventajas de las GUI.

| Interfaces de Línea de Comandos (CLI) | Interfaces Gráficas de Usuario (GUI) |
|---------------------------------------|---------------------------------------|
| **Ventajas**                          | **Ventajas**                          |
| • Más fáciles de implementar por un programador | • Los usuarios no necesitan recordar comandos específicos – más fácil para usuarios nuevos |
| • Requieren menos memoria para ejecutarse | • Los usuarios usan íconos para recordar comandos |
| • Pueden ejecutarse en sistemas sin monitor gráfico | • Los comandos están agrupados en menús y barras de herramientas |
| • Más rápido escribir un comando que usar un ratón – los usuarios experimentados pueden encontrarlo útil | |
| **Desventajas**                       | **Desventajas**                       |
| • Los usuarios deben recordar comandos específicos – difícil para usuarios nuevos | • Más complejas de implementar por un programador |
|                                       | • Requieren más memoria               |
|                                       | • Requieren un monitor gráfico y un dispositivo apuntador |
