<h1 align="center">Fundamentos de diseño de sistemas
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:

[1. Conceptos fundamentales](#1-conceptos-fundamentales)  
  - [1.1. Definición de términos clave](#11-definición-de-términos-clave)  
  - [1.2. Funciones del computador en un mundo interconectado](#12-funciones-del-computador-en-un-mundo-interconectado)  
  - [1.3. Cuestiones éticas y sociales en un mundo interconectado](#13-cuestiones-éticas-y-sociales-en-un-mundo-interconectado)  

[2. Planificación y diseño de sistemas](#2-planificación-y-diseño-de-sistemas)  
  - [2.1. Ingeniería de requisitos](#21-ingeniería-de-requisitos)
  - [2.2. Representación de los requisitos](#22-representación-de-los-requisitos)
    - [2.2.1. Diagramas de flujos](#221-diagramas-de-flujos)
    - [2.2.2. Diagramas de flujo de datos](#222-diagramas-de-flujo-de-datos)
    - [2.2.3. Diagramas de estructuras](#223-diagramas-de-estructuras)

[3. La importancia de la iteración en el proceso de diseño: El ciclo PAI](#3-la-importancia-de-la-iteración-en-el-proceso-de-diseño:-El-ciclo-PAI)  
  - [3.1. ¿Qué es la iteración?](#31-¿qué-es-la-iteración?)
  - [3.2. El ciclo de diseño PAI](#32-el-ciclo-de-diseño-PAI)


# 1. Conceptos fundamentales
## 1.1. Definición de términos clave

En el diseño de sistemas es fundamental comprender ciertos conceptos clave que forman la base de cualquier sistema de información. A continuación, se definen los términos más relevantes:

### **Hardware**  
El hardware es el conjunto de componentes físicos y tangibles de un sistema informático. Incluye dispositivos como la **Unidad Central de Procesamiento (CPU)**, la **memoria RAM**, los **discos duros**, los **periféricos de entrada y salida** (teclado, ratón, pantalla, impresora), y otros elementos que permiten el funcionamiento del sistema.

Ejemplos de hardware:  
- Procesadores (Intel, AMD).  
- Memoria RAM (DDR4, DDR5).  
- Discos duros y SSD.  
- Tarjetas gráficas (NVIDIA, AMD).  
- Periféricos (teclado, ratón, impresora).  

### **Software**  
El software se refiere a los programas y aplicaciones que permiten la ejecución de tareas en un sistema informático. Se divide en varias categorías:  

1. **Software de sistema:** Controla el hardware y proporciona servicios esenciales. Ejemplo: **sistemas operativos (Windows, Linux, macOS).**  
2. **Software de aplicación:** Programas diseñados para el usuario final. Ejemplo: **navegadores web, procesadores de texto, juegos.**  
3. **Software de desarrollo:** Herramientas para crear software. Ejemplo: **compiladores, entornos de desarrollo (IDE), bibliotecas.**  

### **Periférico**  
Los periféricos son dispositivos externos conectados a un sistema informático que permiten la interacción con el usuario o la ampliación de sus capacidades. Se clasifican en:  

- **Periféricos de entrada:** Dispositivos que permiten introducir datos al sistema. Ejemplo: teclado, ratón, escáner, micrófono.  
- **Periféricos de salida:** Dispositivos que muestran o transmiten información procesada. Ejemplo: monitor, impresora, altavoces.  
- **Periféricos de entrada/salida:** Dispositivos que pueden recibir y enviar datos. Ejemplo: pantalla táctil, impresora multifuncional, unidades de almacenamiento externas.  

### **Red**  
Una red es un conjunto de dispositivos interconectados que comparten recursos e información. Puede clasificarse en diferentes tipos según su alcance y propósito:  

- **LAN (Red de Área Local):** Conecta dispositivos en un área reducida (oficina, hogar, escuela).  
- **WAN (Red de Área Amplia):** Cubre grandes distancias, como internet.  
- **MAN (Red de Área Metropolitana):** Conecta múltiples redes dentro de una ciudad.  
- **WLAN (Red de Área Local Inalámbrica):** Usa Wi-Fi para conectar dispositivos sin cables.  

Las redes permiten la comunicación entre **clientes y servidores**, el acceso a internet y la transferencia de datos entre dispositivos.  

### **Recursos Humanos**  
Los recursos humanos en un sistema de información incluyen a todas las personas involucradas en su diseño, desarrollo, implementación y mantenimiento. Pueden clasificarse en varios roles:  

- **Usuarios finales:** Quienes interactúan con el sistema.  
- **Desarrolladores:** Ingenieros y programadores que crean el software.  
- **Administradores de sistemas:** Encargados de gestionar servidores y redes.  
- **Analistas de sistemas:** Profesionales que diseñan soluciones informáticas basadas en los requisitos del negocio.  
- **Soporte técnico:** Personal encargado de la asistencia y mantenimiento del sistema.  

Los recursos humanos son un elemento clave en el éxito de cualquier sistema de información, ya que garantizan su correcto funcionamiento y evolución.  

## 1.2. Funciones del computador en un mundo interconectado

En la actualidad, los computadores desempeñan múltiples funciones en un mundo cada vez más interconectado. Desde el acceso a la información hasta la gestión de infraestructuras críticas, su papel es fundamental en numerosos ámbitos. A continuación, se presentan las principales funciones que un computador puede desempeñar en una red:

### **1. Computador como cliente**
Un cliente es un dispositivo que solicita servicios o recursos a un servidor dentro de una red. Puede ser una computadora personal, un smartphone, una tablet o cualquier otro dispositivo conectado a internet.  
Ejemplos de funciones como cliente:
- Acceso a páginas web mediante un navegador.
- Uso de aplicaciones en la nube como Google Drive o Microsoft 365.
- Descarga de archivos desde servidores remotos.
- Comunicación a través de mensajería instantánea y correo electrónico.

### **2. Computador como servidor**
Un servidor es un computador diseñado para proporcionar servicios a otros dispositivos (clientes) en una red. Puede ser un servidor físico o virtual y está optimizado para manejar grandes volúmenes de datos y múltiples solicitudes simultáneas.  

Tipos de servidores y sus funciones:
- **Servidor web:** Aloja páginas web y aplicaciones accesibles a través de internet. Ejemplo: Apache, Nginx.
- **Servidor de archivos:** Almacena y gestiona archivos accesibles en red. Ejemplo: servidores NAS, Google Drive.
- **Servidor de bases de datos:** Gestiona el almacenamiento y acceso a bases de datos. Ejemplo: MySQL, PostgreSQL.
- **Servidor de impresión:** Administra impresoras y gestiona solicitudes de impresión en una red corporativa.
- **Servidor de juegos:** Facilita el acceso multijugador a videojuegos en línea.

### **3. Servidor de correo electrónico**
Los servidores de correo electrónico gestionan el envío, recepción y almacenamiento de correos electrónicos en una red. Utilizan protocolos específicos como:
- **SMTP (Simple Mail Transfer Protocol):** Para enviar correos.
- **IMAP (Internet Message Access Protocol) y POP3 (Post Office Protocol):** Para recibir y gestionar correos.

Ejemplo de servidores de correo:
- Microsoft Exchange.
- Gmail (Google Workspace).
- Postfix y Exim en servidores Linux.

### **4. Servidor DNS**
El **Servidor DNS (Domain Name System)** convierte los nombres de dominio (como `www.google.com`) en direcciones IP comprensibles para los computadores.  
Funciones clave:
- Traducción de nombres de dominio a direcciones IP.
- Gestión del tráfico de internet asegurando que los usuarios accedan a los sitios correctos.
- Mejora en la velocidad de acceso mediante caché de direcciones IP.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%201.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas%20.jpg" alt="Fundamentos de diseño de sistemas" width="400" height="auto"/>
    <p><em>Figura 1: Funcionamiento DNS. Fuente: DinaHosting</em></p>
  </div>
  
Ejemplos de servidores DNS:
- Google DNS (8.8.8.8 y 8.8.4.4).
- Cloudflare DNS (1.1.1.1).
- OpenDNS.

### **5. Encaminador (Router)**
Un **router** es un dispositivo que dirige el tráfico de red entre diferentes redes.  
Funciones principales:
- Conectar múltiples dispositivos a internet.
- Gestionar el tráfico de red para optimizar el rendimiento.
- Aplicar reglas de seguridad, como firewalls y control de acceso.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%202.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="534" height="auto"/>
    <p><em>Figura 2: Proceso de internet. Fuente: AVG</em></p>
  </div>
  
Ejemplo: Los routers domésticos permiten la conexión de computadoras, teléfonos y televisores inteligentes a internet.

### **6. Cortafuegos (Firewall)**
Un **firewall** es un sistema de seguridad que supervisa y controla el tráfico de red basado en reglas de seguridad predefinidas.  
Funciones principales:
- Filtrar tráfico no autorizado para prevenir ciberataques.
- Bloquear accesos a sitios web maliciosos o restringidos.
- Proteger la integridad de los sistemas informáticos.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%203.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="507" height="auto"/>
    <p><em>Figura 3: Funcionamiento de un Firewall. Fuente: Avast</em></p>
  </div>

Existen firewalls de software (como Windows Defender Firewall) y de hardware (como Cisco ASA o Fortinet).

## 1.3. Cuestiones éticas y sociales en un mundo interconectado

El mundo interconectado actual ha generado numerosos beneficios en términos de comunicación, acceso a la información y globalización. Sin embargo, también plantea diversas cuestiones éticas y sociales que deben abordarse para garantizar un uso responsable de la tecnología. A continuación, se analizan algunos de los principales desafíos en este ámbito.

### **1. Privacidad y protección de datos**  
La privacidad es una de las principales preocupaciones en un mundo digital. Las empresas, gobiernos y plataformas tecnológicas recopilan grandes volúmenes de datos personales, lo que puede generar riesgos como:  
- **Exposición de información personal:** Filtraciones de datos en plataformas y redes sociales.  
- **Uso indebido de datos:** Comercialización de información sin el consentimiento del usuario.  
- **Vigilancia masiva:** Prácticas gubernamentales que pueden atentar contra la privacidad individual.  

Ejemplos de regulaciones para la protección de datos:  
- **GDPR (Reglamento General de Protección de Datos)** en la Unión Europea.  
- **Ley de Privacidad del Consumidor de California (CCPA)** en EE. UU.  

### **2. Ciberseguridad y ciberdelincuencia**  
El aumento de la conectividad ha incrementado los riesgos de ciberataques y fraudes en línea. Entre las principales amenazas se encuentran:  
- **Phishing:** Engaños por correo o mensajes para obtener credenciales.  
- **Ransomware:** Secuestro de datos mediante malware con petición de rescate.  
- **Suplantación de identidad:** Uso fraudulento de datos personales.  
- **Ataques a infraestructuras críticas:** Hackeos a servicios esenciales como energía o salud.  

Medidas para la ciberseguridad:  
- Uso de autenticación de dos factores.  
- Encriptación de datos.  
- Educación digital en ciberseguridad.  

### **3. Brecha digital**  
El acceso desigual a la tecnología ha generado una **brecha digital** entre diferentes sectores de la población. Factores que influyen en esta desigualdad incluyen:  
- **Diferencias económicas:** Falta de acceso a dispositivos o internet en comunidades de bajos recursos.  
- **Diferencias geográficas:** Falta de infraestructuras digitales en zonas rurales.  
- **Barreras educativas:** Falta de conocimientos tecnológicos en ciertos sectores de la población.  

Estrategias para reducir la brecha digital:  
- Implementación de políticas de acceso gratuito a internet en espacios públicos.  
- Educación digital para grupos vulnerables.  
- Desarrollo de infraestructuras de conectividad en zonas rurales.  

### **4. Ética en la inteligencia artificial y automatización**  
El uso de **inteligencia artificial (IA)** plantea dilemas éticos, como:  
- **Discriminación algorítmica:** Sesgos en la IA que pueden perjudicar a ciertos grupos.  
- **Automatización del empleo:** Desplazamiento de trabajos humanos por máquinas.  
- **Responsabilidad en decisiones automatizadas:** Quién responde por errores de una IA (por ejemplo, en vehículos autónomos).  

Propuestas para una IA ética:  
- Creación de regulaciones sobre transparencia en algoritmos.  
- Supervisión humana en decisiones críticas.  
- Desarrollo de IA sin sesgos de discriminación.  

### **5. Dependencia tecnológica y bienestar digital**  
El uso excesivo de la tecnología puede afectar la salud mental y la calidad de vida de los usuarios. Problemas asociados:  
- **Adicción a las redes sociales y dispositivos móviles.**  
- **Afectaciones en la concentración y productividad.**  
- **Problemas de sueño y ansiedad debido al uso excesivo de pantallas.**  

Recomendaciones para un uso equilibrado de la tecnología:  
- Establecer límites de tiempo en el uso de dispositivos.  
- Promover actividades fuera del entorno digital.  
- Desarrollar conciencia sobre el impacto de la hiperconectividad.  

# 2. Planificación y diseño de sistemas de software
## 2.1. Ingeniería de requisitos

> [!IMPORTANT]  
> La **ingeniería de requisitos** es la disciplina que nos ayuda a identificar, gestionar y mantener el conjunto de requisitos del software que hemos de desarrollar.

Denominamos ingeniería de requisitos a aquel subconjunto de la ingeniería del software que se encarga de las actividades siguientes:

- **Obtención de requisitos:** identificar las fuentes de información de los posibles requisitos del sistema y obtener cuáles son estos requisitos candidatos.
- **Gestión de requisitos:** estimar el coste que implica tener en cuenta cada requisito, priorizarlos según la importancia que tengan para los stakeholders y así poder seleccionar los requisitos que finalmente se tendrán en cuenta en la etapa actual de desarrollo del sistema.
- **Documentación de requisitos:** documentar los requisitos de manera que quede constancia del resultado del proceso de gestión de requisitos y que, al mismo tiempo, los stakeholders y los desarrolladores compartan la visión de cuál es el producto que se ha de desarrollar. Esta documentación puede formar parte o no de la documentación final del sistema.
- **Validación de requisitos:** comprobar que los requisitos elegidos para el producto que estamos desarrollando reflejan las expectativas de los stakeholders y, por lo tanto, que no ha habido errores en su obtención, priorización, selección y documentación.

Verificación de requisitos: verificar si el sistema desarrollado (o parcialmente desarrollado en el caso de ciclos de vida iterativos) satisface o no los requisitos y cuáles.

### 2.1.1. Requisitos y stakeholders

Para poder desarrollar un sistema informático, obviamente, hay que entender qué sistema hay que desarrollar y, por lo tanto, hay que entender bien los requisitos de todo tipo que los diferentes stakeholders tienen sobre el sistema. Varias de las actividades de la ingeniería del software hacen referencia a estos requisitos y, de hecho, podemos considerar que estos son una pieza clave para el éxito o fracaso de todo proyecto de desarrollo de software.

> [!IMPORTANT]  
> Los **requisitos** son características observables de un sistema que expresan una necesidad o restricción que un stakeholder tiene sobre él.

Los requisitos nos sirven, por lo tanto, para delimitar cuáles de las posibles soluciones a un problema son adecuadas (las que cumplen los requisitos) y cuáles no.

> [!IMPORTANT]  
> Los **stakeholders** son aquellas personas o entidades que tienen algún impacto o interés en este sistema.

A pesar de que todos los usuarios de un sistema son stakeholders, puesto que todos lo usan y, por lo tanto, tienen intereses en él, no todos los stakeholders son usuarios, puesto que puede haber muchas personas o entidades que, a pesar de que no utilicen el sistema, se ven afectadas por su implantación y que, por lo tanto, también tienen intereses en él.

## 2.2. Tipos de requisitos

En este apartado establecemos una taxonomía para tipificar los requisitos con el fin de evitar la ambigüedad a la hora de determinar el tipo de un requisito. Cada obra e incluso cada organización usa su propia taxonomía, pero hay ciertos puntos comunes en la mayoría de ellas.

> [!NOTE]  
> Una taxonomía es una colección de términos de vocabulario controlados que se organiza en una estructura jerárquica.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%204.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas"/>
    <p><em>Figura 4: Tipos de requisitos. Fuente: UOC</em></p>
  </div>

### 2.2.1. Requisitos de producto

Los requisitos de producto definen aquellas necesidades o restricciones que los stakeholders tienen sobre el producto que se desarrollará como tal. Es decir, nos interesará que, una vez desarrollado, el producto satisfaga estos requisitos.
> [!NOTE]  
> Algunos ejemplos de requisitos de producto del caso práctico son:
> - Como usuario quiero poder consultar las recomendaciones de los agentes sobre un hotel.
> - El sistema debe conocer el nombre, los apellidos, la dirección de correo electrónico, la dirección y el teléfono de los clientes.
> - El sistema tiene que permitir a las agencias continuar trabajando aunque se pierda la conexión en Internet.

A su vez, los requisitos de producto se pueden clasificar en: 

**1. Requisitos funcionales**

Los requisitos funcionales hacen referencia a la funcionalidad que debe proporcionar el sistema y los datos que tiene que conocer y guardar. Nos indican qué cálculos hace el sistema, qué datos mantiene, cómo los manipula, etc.
Podemos distinguir, dentro de los requisitos funcionales, entre los requisitos de **funcionalidad** y los de **datos**.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%205.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas"/>
    <p><em>Figura 5: Tipos de requisitos funcionales. Fuente: UOC</em></p>
  </div>

Los **requisitos de funcionalidad**, en general, describen cuál tiene que ser el comportamiento del sistema explicando qué respuesta debe dar ante los estímulos que le llegan desde el exterior. Por respuesta nos referimos a qué respuesta observable desde fuera, considerando el sistema como una caja negra.

> [!NOTE]  
> Algunos ejemplos de requisitos funcionales de funcionalidad del caso práctico son:
> - Como usuario quiero poder consultar las recomendaciones de los agentes sobre un hotel.
> - Como directora de marketing, quiero que los clientes puedan recomendar en las redes sociales los viajes que ofrecemos.

Los **requisitos de datos** describen qué datos tiene que conocer el sistema. Estos son, típicamente, datos que el sistema guardará de modo persistente.

> [!NOTE]  
> Un par de ejemplos pueden ser:
> - El sistema tiene que conocer el cliente de un viaje; en particular, debe saber el nombre, los apellidos, la dirección de correo electrónico, la dirección postal y el teléfono.
> - El sistema tiene que conocer el hotel u hoteles de un viaje. De los hoteles tiene que saber el nombre, la dirección y el teléfono. En relación con el viaje tiene que saber las fechas de entrada y salida, las horas de check-in y check-out, el tipo de habitación, las observaciones del hotel y la opinión del agente que ha reservado el viaje.

**1. Requisitos no funcionales**

Los **requisitos no funcionales** son aquellos requisitos de producto que, como su nombre indica, no son funcionales sino calidades esperadas del sistema, como por ejemplo usabilidad, fiabilidad, rendimiento o mantenibilidad. Son, por lo tanto, restricciones sobre el conjunto de soluciones tales que si una solución no satisface aquella calidad, no se considera válida.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%206.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas"/>
    <p><em>Figura 6: Tipos de requisitos no funcionales. Fuente: UOC</em></p>
  </div>

### 2.2.2. Requisitos de proceso

Los **requisitos de proceso** establecen restricciones en el propio proceso de desarrollo de software en lugar de hacerlo sobre el producto final desarrollado. Cualquier necesidad o restricción que no sea del producto una vez terminado sino del proceso que se sigue para completarlo será, por lo tanto, un requisito de proceso.

Uno de los requisitos de proceso más importante es el coste de desarrollo, tanto en tiempo como en dinero. A pesar de no tratarse de una característica observable en el producto ya desarrollado, sí que lo es en el proceso. Y, evidentemente, los stakeholders tendrán necesidades y restricciones que imponer.

## 2.2. Representación de los requisitos

En el **desarrollo de sistemas de información** es fundamental plasmar de manera gráfica y clara los requisitos y la lógica del sistema. Esto facilita la comunicación entre los distintos miembros del equipo y permite detectar posibles errores o mejoras en etapas tempranas del diseño.

### 2.2.1. Diagramas de flujo

Los diagramas de flujo de sistemas son representaciones gráficas que muestran el recorrido de los datos y el procesamiento de la información dentro de un sistema.

#### Elementos Comunes
- **Inicio/Fin:** Se representan con óvalos.
- **Procesos:** Se indican con rectángulos.
- **Decisiones:** Se usan rombos para representar bifurcaciones en el flujo.
- **Entradas/Salidas:** Se muestran con paralelogramos.
- **Conectores:** Flechas que indican la dirección del flujo.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%207.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="500" height="auto"/>
    <p><em>Figura 7: Diagrama de flujo. Fuente: Epitech</em></p>
  </div>

### 2.2.2. Diagramas de flujo de datos

Los diagramas de flujo de datos se centran en la forma en que la información se mueve y transforma a lo largo del sistema.

#### Elementos Comunes
- **Procesos:** Actividades o funciones que transforman la información.
- **Almacenes de Datos:** Representan bases de datos o lugares de almacenamiento.
- **Flujos de Datos:** Indicados con flechas, representan el movimiento de información.
- **Entidades Externas:** Actores o sistemas externos que interactúan con el sistema.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%208.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="500" height="auto"/>
    <p><em>Figura 8: Diagrama de flujo de datos. Fuente: Manuel Cillero</em></p>
  </div>

### 2.2.3. Diagramas de estructuras

Estos diagramas representan la organización y la jerarquía de los componentes o módulos del sistema.

### Elementos Comunes
- **Componentes/Módulos:** Se representan con cajas o rectángulos.
- **Relaciones:** Líneas o flechas que conectan los módulos para indicar dependencias o interacciones.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%209.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="500" height="auto"/>
    <p><em>Figura 9: Diagrama de estructuras. Fuente: Manuel Cillero</em></p>
  </div>

# 3. La importancia de la iteración en el proceso de diseño: El ciclo PAI

El proceso de diseño en sistemas y productos no es lineal, sino que requiere de una revisión constante y de la adaptación a nuevos requerimientos y descubrimientos. La iteración se convierte en una herramienta clave para alcanzar un diseño óptimo, permitiendo mejorar y refinar el producto a lo largo de todo el proceso.

## 3.1. ¿Qué es la iteración?

La iteración consiste en repetir ciclos de trabajo en el proceso de diseño. Cada ciclo se utiliza para:
- **Evaluar el diseño actual:** Detectar errores o áreas de mejora.
- **Implementar cambios:** Incorporar ajustes que optimicen el producto.
- **Validar mejoras:** Asegurarse de que las modificaciones responden a las necesidades detectadas.

Esta metodología permite que, en cada vuelta, el diseño se acerque cada vez más a los objetivos planteados.

## 3.2. El ciclo de diseño PAI

El Ciclo PAI es una metodología que estructura el proceso de diseño en tres fases fundamentales:

1. **Planificación:**
   - Definir objetivos y requisitos.
   - Establecer una visión clara del producto.
   - Diseñar estrategias y establecer criterios de éxito.
   
2. **Acción:**
   - Desarrollar el diseño o prototipo inicial.
   - Poner en práctica las ideas y soluciones planteadas.
   - Construir una primera versión funcional del producto.

3. **Iteración:**
   - Evaluar el prototipo mediante pruebas y retroalimentación.
   - Identificar errores, oportunidades de mejora y nuevas necesidades.
   - Ajustar y perfeccionar el diseño, reiniciando el ciclo según sea necesario.

### Beneficios de la iteración en el diseño

- **Mejora Continua:** Cada ciclo permite detectar y corregir fallos, elevando la calidad del producto.
- **Flexibilidad y Adaptación:** Facilita la incorporación de nuevos requerimientos y la adaptación ante cambios.
- **Reducción de Riesgos:** Al validar ideas y corregir errores de forma temprana, se minimizan los riesgos en etapas posteriores.
- **Optimización de Recursos:** Permite utilizar de forma eficiente tiempo y esfuerzo, evitando retrabajos significativos.

### Ejemplo práctico

Imaginemos el desarrollo de una aplicación móvil:

1. **Planificación:** Se definen las funcionalidades esenciales, se crea un mapa de navegación y se establecen los objetivos de usabilidad.
2. **Acción:** Se desarrolla un prototipo básico de la aplicación con las funcionalidades definidas.
3. **Iteración:** Se prueba el prototipo con usuarios reales, se recogen sus opiniones y se detectan problemas en la navegación y la interfaz. Con esta retroalimentación se realizan los ajustes necesarios y se vuelve a probar la aplicación.

Este ciclo se repite hasta que el producto cumpla con los estándares de calidad y satisfaga las necesidades del usuario.

