<h1 align="center">1.2. Fundamentos de diseño de sistemas
<div align="center">

</div>

## Contenido:

- [1.2.1. Definición de términos clave](#121-definición-de-términos-clave)  
- [1.2.2. Funciones del computador en un mundo interconectado](#122-funciones-de-un-computador-en-un-mundo-interconectado)
- [1.2.3. Cuestiones éticas y sociales en un mundo interconectado](#123-cuestiones-éticas-y-sociales-en-un-mundo-interconectado)
- [1.2.4. Partes interesadas al planificar un nuevo sistema](#124-la-implantación-del-sistema-de-información) 
- [1.2.5. Ingeniería de requisitos](#125-ingeniería-de-requisitos) 
- [1.2.6. Representación de los requisitos](#126-representación-de-los-requisitos)
- [1.2.7. El propósito de un prototipo](#127-el-propósito-de-un-prototipo)
- [1.2.8. La importancia de la iteración en el proceso de diseño](#128-la-importancia-de-la-iteración-en-el-proceso-de-diseño)
- [1.2.9. Posibles consecuencias de no implicar al usuario final en el proceso de diseño](#129-posibles-consecuencias-de-no-implicar-al-usuario-final-en-el-proceso-de-diseño)
- [1.2.10 Cuestiones éticas y sociales asociadas a la introducción de un nuevo sistema de TI](#1210-cuestiones-éticas-y-sociales-asociadas-a-la-introducción-de-un-nuevo-sistema-de-TI)
- [1.2.11. El concepto de usabilidad](#1211-el-concepto-de-usabilidad)
- [1.2.12. Problemas de usabilidad en dispositivos digitales](#1212-problemas-de-usabilidad-en-dispositivos-digitales)
- [1.2.13. Métodos para mejorar la accesibilidad en los sistemas](#1213-métodos-para-mejorar-la-accesibilidad-en-los-sistemas)
- [1.2.14. Implicaciones morales, éticas, sociales, económicas y ambientales de la interacción entre humanos y máquinas](#1214-implicaciones-morales-éticas-sociales-económicas-y-ambientales-de-la-interacción-entre-humanos-y-máquinas)


## 1.2.1. Definición de términos clave

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

## 1.2.2. Funciones del computador en un mundo interconectado

En la actualidad, los computadores desempeñan múltiples funciones en un mundo cada vez más interconectado. Desde el acceso a la información hasta la gestión de infraestructuras críticas, su papel es fundamental en numerosos ámbitos. A continuación, se presentan las principales funciones que un computador puede desempeñar en una red:

### Computador como cliente
Un cliente es un dispositivo que solicita servicios o recursos a un servidor dentro de una red. Puede ser una computadora personal, un smartphone, una tablet o cualquier otro dispositivo conectado a internet.  
Ejemplos de funciones como cliente:
- Acceso a páginas web mediante un navegador.
- Uso de aplicaciones en la nube como Google Drive o Microsoft 365.
- Descarga de archivos desde servidores remotos.
- Comunicación a través de mensajería instantánea y correo electrónico.

### Computador como servidor
Un servidor es un computador diseñado para proporcionar servicios a otros dispositivos (clientes) en una red. Puede ser un servidor físico o virtual y está optimizado para manejar grandes volúmenes de datos y múltiples solicitudes simultáneas.  

Tipos de servidores y sus funciones:
- **Servidor web:** Aloja páginas web y aplicaciones accesibles a través de internet. Ejemplo: Apache, Nginx.
- **Servidor de archivos:** Almacena y gestiona archivos accesibles en red. Ejemplo: servidores NAS, Google Drive.
- **Servidor de bases de datos:** Gestiona el almacenamiento y acceso a bases de datos. Ejemplo: MySQL, PostgreSQL.
- **Servidor de impresión:** Administra impresoras y gestiona solicitudes de impresión en una red corporativa.
- **Servidor de juegos:** Facilita el acceso multijugador a videojuegos en línea.

### Servidor de correo electrónico
Los servidores de correo electrónico gestionan el envío, recepción y almacenamiento de correos electrónicos en una red. Utilizan protocolos específicos como:
- **SMTP (Simple Mail Transfer Protocol):** Para enviar correos.
- **IMAP (Internet Message Access Protocol) y POP3 (Post Office Protocol):** Para recibir y gestionar correos.

Ejemplo de servidores de correo:
- Microsoft Exchange.
- Gmail (Google Workspace).
- Postfix y Exim en servidores Linux.

### Servidor DNS
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

### Encaminador (Router)
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

### Cortafuegos (Firewall)
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

## 1.2.3. Cuestiones éticas y sociales en un mundo interconectado

El mundo interconectado actual ha generado numerosos beneficios en términos de comunicación, acceso a la información y globalización. Sin embargo, también plantea diversas cuestiones éticas y sociales que deben abordarse para garantizar un uso responsable de la tecnología. A continuación, se analizan algunos de los principales desafíos en este ámbito.

### Privacidad y protección de datos 
La privacidad es una de las principales preocupaciones en un mundo digital. Las empresas, gobiernos y plataformas tecnológicas recopilan grandes volúmenes de datos personales, lo que puede generar riesgos como:  
- **Exposición de información personal:** Filtraciones de datos en plataformas y redes sociales.  
- **Uso indebido de datos:** Comercialización de información sin el consentimiento del usuario.  
- **Vigilancia masiva:** Prácticas gubernamentales que pueden atentar contra la privacidad individual.  

Ejemplos de regulaciones para la protección de datos:  
- **GDPR (Reglamento General de Protección de Datos)** en la Unión Europea.  
- **Ley de Privacidad del Consumidor de California (CCPA)** en EE. UU.  

### Ciberseguridad y ciberdelincuencia
El aumento de la conectividad ha incrementado los riesgos de ciberataques y fraudes en línea. Entre las principales amenazas se encuentran:  
- **Phishing:** Engaños por correo o mensajes para obtener credenciales.  
- **Ransomware:** Secuestro de datos mediante malware con petición de rescate.  
- **Suplantación de identidad:** Uso fraudulento de datos personales.  
- **Ataques a infraestructuras críticas:** Hackeos a servicios esenciales como energía o salud.  

Medidas para la ciberseguridad:  
- Uso de autenticación de dos factores.  
- Encriptación de datos.  
- Educación digital en ciberseguridad.  

### Brecha digital 
El acceso desigual a la tecnología ha generado una **brecha digital** entre diferentes sectores de la población. Factores que influyen en esta desigualdad incluyen:  
- **Diferencias económicas:** Falta de acceso a dispositivos o internet en comunidades de bajos recursos.  
- **Diferencias geográficas:** Falta de infraestructuras digitales en zonas rurales.  
- **Barreras educativas:** Falta de conocimientos tecnológicos en ciertos sectores de la población.  

Estrategias para reducir la brecha digital:  
- Implementación de políticas de acceso gratuito a internet en espacios públicos.  
- Educación digital para grupos vulnerables.  
- Desarrollo de infraestructuras de conectividad en zonas rurales.  

### Ética en la inteligencia artificial y automatización 
El uso de **inteligencia artificial (IA)** plantea dilemas éticos, como:  
- **Discriminación algorítmica:** Sesgos en la IA que pueden perjudicar a ciertos grupos.  
- **Automatización del empleo:** Desplazamiento de trabajos humanos por máquinas.  
- **Responsabilidad en decisiones automatizadas:** Quién responde por errores de una IA (por ejemplo, en vehículos autónomos).  

Propuestas para una IA ética:  
- Creación de regulaciones sobre transparencia en algoritmos.  
- Supervisión humana en decisiones críticas.  
- Desarrollo de IA sin sesgos de discriminación.  

### Dependencia tecnológica y bienestar digital
El uso excesivo de la tecnología puede afectar la salud mental y la calidad de vida de los usuarios. Problemas asociados:  
- **Adicción a las redes sociales y dispositivos móviles.**  
- **Afectaciones en la concentración y productividad.**  
- **Problemas de sueño y ansiedad debido al uso excesivo de pantallas.**  

Recomendaciones para un uso equilibrado de la tecnología:  
- Establecer límites de tiempo en el uso de dispositivos.  
- Promover actividades fuera del entorno digital.  
- Desarrollar conciencia sobre el impacto de la hiperconectividad.  

## 1.2.4. Interesados a la hora de planificar un nuevo sistema

Los **stakeholders** son individuos, equipos, grupos u organizaciones que tienen un interés en la realización de un proyecto o que pueden verse afectados por el resultado de un proyecto. Por lo tanto, cualquier persona que tenga intereses en un sistema de información existente o propuesto puede describirse como un stakeholder del sistema.

El **usuario final** es la persona que va a utilizar el producto. Un stakeholder relevante también puede ser un usuario frecuente del sistema actual. Esta persona podrá identificar fallos y errores del sistema actual o inconvenientes que haya detectado. También podrá proponer mejoras que serán cruciales para la actualización del sistema.

El **gerente o supervisor** del procedimiento que el sistema lleva a cabo también puede tener algunos comentarios. Asimismo, se puede pedir consejo a **especialistas** que hayan tratado con una situación similar en el pasado.

## 1.2.5. Ingeniería de requisitos

> [!IMPORTANT]  
> La **ingeniería de requisitos** es la disciplina que nos ayuda a identificar, gestionar y mantener el conjunto de requisitos del software que hemos de desarrollar.

Denominamos ingeniería de requisitos a aquel subconjunto de la ingeniería del software que se encarga de las actividades siguientes:

- **Obtención de requisitos:** identificar las fuentes de información de los posibles requisitos del sistema y obtener cuáles son estos requisitos candidatos.
- **Gestión de requisitos:** estimar el coste que implica tener en cuenta cada requisito, priorizarlos según la importancia que tengan para los stakeholders y así poder seleccionar los requisitos que finalmente se tendrán en cuenta en la etapa actual de desarrollo del sistema.
- **Documentación de requisitos:** documentar los requisitos de manera que quede constancia del resultado del proceso de gestión de requisitos y que, al mismo tiempo, los stakeholders y los desarrolladores compartan la visión de cuál es el producto que se ha de desarrollar. Esta documentación puede formar parte o no de la documentación final del sistema.
- **Validación de requisitos:** comprobar que los requisitos elegidos para el producto que estamos desarrollando reflejan las expectativas de los stakeholders y, por lo tanto, que no ha habido errores en su obtención, priorización, selección y documentación.

Verificación de requisitos: verificar si el sistema desarrollado (o parcialmente desarrollado en el caso de ciclos de vida iterativos) satisface o no los requisitos y cuáles.

### Tipos de requisitos

En este apartado establecemos una taxonomía para tipificar los requisitos con el fin de evitar la ambigüedad a la hora de determinar el tipo de un requisito. Cada obra e incluso cada organización usa su propia taxonomía, pero hay ciertos puntos comunes en la mayoría de ellas.

> [!NOTE]  
> Una taxonomía es una colección de términos de vocabulario controlados que se organiza en una estructura jerárquica.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%204.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas"/>
    <p><em>Figura 4: Tipos de requisitos. Fuente: UOC</em></p>
  </div>

### Requisitos de producto

Los requisitos de producto definen aquellas necesidades o restricciones que los stakeholders tienen sobre el producto que se desarrollará como tal. Es decir, nos interesará que, una vez desarrollado, el producto satisfaga estos requisitos.
> [!NOTE]  
> Algunos ejemplos de requisitos de producto del caso práctico son:
> - Como usuario quiero poder consultar las recomendaciones de los agentes sobre un hotel.
> - El sistema debe conocer el nombre, los apellidos, la dirección de correo electrónico, la dirección y el teléfono de los clientes.
> - El sistema tiene que permitir a las agencias continuar trabajando aunque se pierda la conexión en Internet.

A su vez, los requisitos de producto se pueden clasificar en: 

#### Requisitos funcionales

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

#### Requisitos no funcionales

Los **requisitos no funcionales** son aquellos requisitos de producto que, como su nombre indica, no son funcionales sino calidades esperadas del sistema, como por ejemplo usabilidad, fiabilidad, rendimiento o mantenibilidad. Son, por lo tanto, restricciones sobre el conjunto de soluciones tales que si una solución no satisface aquella calidad, no se considera válida.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%206.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas"/>
    <p><em>Figura 6: Tipos de requisitos no funcionales. Fuente: UOC</em></p>
  </div>

#### Requisitos de proceso

Los **requisitos de proceso** establecen restricciones en el propio proceso de desarrollo de software en lugar de hacerlo sobre el producto final desarrollado. Cualquier necesidad o restricción que no sea del producto una vez terminado sino del proceso que se sigue para completarlo será, por lo tanto, un requisito de proceso.

Uno de los requisitos de proceso más importante es el coste de desarrollo, tanto en tiempo como en dinero. A pesar de no tratarse de una característica observable en el producto ya desarrollado, sí que lo es en el proceso. Y, evidentemente, los stakeholders tendrán necesidades y restricciones que imponer.

### Métodos para la obtención de requisitos

**La recopilación de diversos detalles sobre un sistema existente y la obtención de los requisitos de los stakeholders para un sistema planificado implica:**

#### Entrevistas con los stakeholders

Una entrevista es un procedimiento directo y presencial que se centra en obtener datos fiables y válidos en forma de respuestas verbales de una persona o de un grupo (grupo de stakeholders).

- **Entrevistas estructuradas:** están estrictamente estandarizadas y prescritas. Se presenta un conjunto de preguntas preparadas de la misma manera y en el mismo orden a cada stakeholder.

- **Entrevistas no estructuradas:** son flexibles. Se anima a los stakeholders a expresar libremente sus pensamientos y creencias personales.

Una entrevista es un proceso conversacional que consume tiempo, pero que permite al entrevistador aclarar preguntas y observar los comportamientos verbales y no verbales de los stakeholders.
Una desventaja es que las entrevistas no estructuradas a menudo producen datos demasiado difíciles de resumir, evaluar o someter a análisis estadístico.

#### Uso de cuestionarios

Su aplicación es efectiva cuando las preguntas están cuidadosamente diseñadas para obtener respuestas no ambiguas.
La **metodología de encuestas** hace referencia a un ámbito de la estadística aplicada que se centra en tomar muestras de una población, así como en mejorar las diferentes técnicas de recogida de datos (p. ej., cuestionarios).

- **Cuestionarios cerrados o restringidos:** incluyen respuestas de “sí” o “no”, preguntas de respuesta corta y casillas de verificación. Este tipo de cuestionario facilita el análisis estadístico, la presentación tabular de datos y los procesos de resumen.

- **Cuestionarios abiertos o no restringidos:** incluyen preguntas de respuesta libre, lo que permite obtener respuestas más profundas del stakeholder. Sin embargo, son difíciles de interpretar o resumir y hacen imposible el análisis estadístico.

Los cuestionarios garantizan la **uniformidad de las preguntas** y, por lo tanto, generan datos más fácilmente comparables que la información obtenida en una entrevista. Además, es un método que ahorra tiempo, resulta rentable y permite llegar rápidamente a muchos stakeholders. Sin embargo, es difícil evaluar la **motivación de los encuestados**, y los stakeholders pueden no responder, contestar solo a algunas preguntas o malinterpretar la cuestión.

#### Observación directa de los procedimientos actuales

Implica pasar tiempo en diferentes departamentos. Se considera un estudio de tiempos y movimientos, capaz de mostrar dónde se podrían hacer más eficientes los procedimientos y procesos, o dónde pueden estar presentes posibles cuellos de botella.

La observación directa permite recopilar distintos tipos de datos e información. Estar en el lugar durante un periodo de tiempo familiariza al analista con el caso de estudio, lo que facilita la participación en todas las actividades y procesos. La observación es independiente del sesgo del usuario, pero es un método que consume tiempo.

Sin embargo, a veces las personas cambian su comportamiento cuando saben que están siendo observadas. El término **“efecto Hawthorne”** se utiliza para describir situaciones en las que los trabajadores mejoran su rendimiento al saber que participan en un proceso de observación.

## 1.2.5. Ingeniería de requisitos

**Examinar los sistemas actuales** es un proceso que implica la revisión detallada del sistema en funcionamiento, el análisis de sus funciones y procedimientos, así como el estudio de la documentación empresarial y del sistema, como documentos de pedidos, documentos de logística y procedimientos y reportes informáticos utilizados por los responsables de operaciones y directivos.

Según Auston et al. (1992), la **búsqueda bibliográfica** hace referencia a la identificación, recuperación y gestión de diversas fuentes con el fin de encontrar información sobre un tema, detectar áreas de interés para estudios posteriores, extraer conclusiones y desarrollar guías para la práctica.

Hoy en día, la manera más eficiente de identificar estudios publicados y buscar información específica es mediante el uso de **bases de datos en línea, motores de búsqueda, etc**.

**Examinar productos competidores** puede incluir el análisis de factores competitivos, sus beneficios, vulnerabilidades, características exitosas, innovaciones introducidas, elementos de diseño, así como la aceptación de los usuarios y de los stakeholders.

Durante las fases de **análisis y diseño** deben identificarse todas las capacidades organizativas críticas que resulten esenciales para apoyar una planificación y desarrollo efectivos del nuevo sistema de TI. Un sistema de TI exitoso debe traducirse en una **ventaja competitiva**.

Según Hell (2011), las capacidades organizativas como la **interpretación de la información (sense-making), la toma de decisiones, la disponibilidad de recursos y la gestión de operaciones** están totalmente vinculadas a la implementación eficaz de un sistema de información, lo cual a su vez repercute positivamente en el rendimiento de la organización.

Los sistemas de información utilizados en las empresas modernas desempeñan un papel crítico, y la mayoría de las compañías utilizan los datos y la información como **activos para obtener ventajas competitivas**.

Debemos tener en cuenta que un sistema de información moderno debe planificarse para:

- aumentar la confianza del cliente,
- preservar la fortaleza de la marca,
- proteger la reputación de la organización,
- mantener la resiliencia corporativa,
- mejorar la estabilidad organizacional.

## 1.2.6. Representación de los requisitos

En el **desarrollo de sistemas de información** es fundamental plasmar de manera gráfica y clara los requisitos y la lógica del sistema. Esto facilita la comunicación entre los distintos miembros del equipo y permite detectar posibles errores o mejoras en etapas tempranas del diseño.

### Diagramas de flujo

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

### Diagramas de flujo de datos

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

### Diagramas de estructuras

Estos diagramas representan la organización y la jerarquía de los componentes o módulos del sistema.

### Elementos Comunes
- **Componentes/Módulos:** Se representan con cajas o rectángulos.
- **Relaciones:** Líneas o flechas que conectan los módulos para indicar dependencias o interacciones.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%209.%20Fundamentos%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="500" height="auto"/>
    <p><em>Figura 9: Diagrama de estructuras. Fuente: Manuel Cillero</em></p>
  </div>

## 1.2.7. El propósito de un prototipo

**Competencias de salida.** Los estudiantes deben ser capaces de:

- Explicar la necesidad de crear prototipos durante la etapa de diseño.
- Describir la necesidad de la retroalimentación del usuario/cliente.
- Explicar la necesidad de una colaboración eficaz.

Existen muchas ventajas en la creación de un **prototipo**.
Un prototipo es una versión preliminar, ya sea funcional o no funcional, del producto final, o una versión simple del sistema final que se utiliza como parte de la fase de diseño para demostrar cómo funcionará el producto final.

Un prototipo:

- Atrae la atención del cliente, ya que lo anima a usarlo y a “probarlo”.
- Proporciona lo suficiente del concepto para que los inversores decidan si quieren financiar la producción completa o no.
- Fomenta la participación activa entre usuarios y desarrolladores.
- Ofrece una idea del producto final.
- Ayuda a identificar problemas relacionados con la eficiencia o el diseño.
- Incrementa la velocidad de desarrollo del sistema.

## 1.2.8. La importancia de la iteración en el proceso de diseño

El proceso de diseño en sistemas y productos no es lineal, sino que requiere de una revisión constante y de la adaptación a nuevos requerimientos y descubrimientos. La iteración se convierte en una herramienta clave para alcanzar un diseño óptimo, permitiendo mejorar y refinar el producto a lo largo de todo el proceso.

### ¿Qué es la iteración?

La iteración consiste en repetir ciclos de trabajo en el proceso de diseño. Cada ciclo se utiliza para:
- **Evaluar el diseño actual:** Detectar errores o áreas de mejora.
- **Implementar cambios:** Incorporar ajustes que optimicen el producto.
- **Validar mejoras:** Asegurarse de que las modificaciones responden a las necesidades detectadas.

Esta metodología permite que, en cada vuelta, el diseño se acerque cada vez más a los objetivos planteados.

### El ciclo de diseño PAI

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

## 1.2.9. Posibles consecuencias de no implicar al usuario final en el proceso de diseño

Para que un sistema tenga éxito, el análisis y el diseño deben involucrar a todos los **stakeholders clave**, incluyendo al **cliente** (la persona u organización que financia el proyecto) y a los **usuarios finales** (las personas que utilizarán el sistema).

La **implicación, la colaboración y la participación activa** son fundamentales, ya que un proyecto con objetivos de los stakeholders mal definidos tiene pocas probabilidades de ser exitoso.

El sistema desarrollado puede terminar resolviendo un problema distinto o abordando cuestiones que están fuera del alcance del proyecto.

## 1.2.10 Cuestiones éticas y sociales asociadas a la introducción de un nuevo sistema de TI

Los **cajeros automáticos (ATM)** reemplazaron a los cajeros de banco, los sistemas de **peaje electrónico (E-pass) **sustituyeron a los cobradores de autopistas, las **agencias de viajes en internet** reemplazaron a las pequeñas agencias de viajes, los **sistemas automatizados de voz** sustituyeron a los representantes de atención al cliente, el correo electrónico reemplazó a los carteros, los **sistemas de reconocimiento de voz** sustituyeron a los mecanógrafos, y los **blogs, periodistas ciudadanos y usuarios de redes sociales** están reemplazando a los reporteros.

Las máquinas están reemplazando a los humanos en innumerables tareas, lo que ha forzado a millones de personas al desempleo. Un contraargumento es que los empleos no desaparecen, sino que cambian. Finalmente, los avances en **robótica** e **inteligencia artificial** podrían eventualmente reemplazar a una cantidad cada vez mayor de trabajadores con robots inteligentes. Esto podría generar una **alteración social** similar a la ocurrida durante la **Revolución Industrial** (cuando la introducción de máquinas tuvo un impacto semejante en la sociedad).

La introducción de **nuevos sistemas y aplicaciones de tecnologías de la información** (o el desarrollo constante de los ya existentes) ciertamente tiene un gran impacto en la sociedad y plantea preguntas éticas sobre hasta qué punto este desarrollo incontrolable puede o debe continuar.

Por ejemplo, la creación de **Facebook y Twitter**. Estas redes sociales se hicieron cada vez más populares, penetrando en la vida social y personal de los usuarios, hasta convertirse en un componente vital de ella. Facebook cambió la forma en que ocurren las interacciones sociales. Es importante señalar que la **interacción social** también es un elemento esencial del **cambio social**, que afecta a las ideas, creencias y valores morales.

Otros desarrollos de TI pueden tener un impacto social más indirecto, pero, dado que el **objetivo principal del desarrollo de sistemas de tecnologías de la información** debería ser mejorar la vida humana, este impacto debe ser examinado.

El **desarrollo continuo de sistemas informatizados** puede absorber a las personas y alejarlas del mundo físico, confinándolas en **entornos virtuales**. La participación en estos entornos puede llegar a desorientar completamente a algunos usuarios. Además, los entornos automatizados, como la “**casa inteligente**”, que se encarga de tareas cotidianas como revisar el contenido del refrigerador y realizar pedidos de suministros, pueden privar a las personas de oportunidades de socialización e interacción que antes ofrecían estas actividades. Considerando estos posibles resultados, surgen más cuestiones morales y éticas.

Un hallazgo sorprendente es que, en un **entorno empresarial**, la introducción de un nuevo sistema de información mejorado a menudo genera **mayor estrés en el personal**, ya que deben estudiar, aprender y familiarizarse con el nuevo sistema mientras cumplen con sus tareas habituales.

Es necesario determinar hasta qué punto los avances en TI son realmente **beneficiosos**, para garantizar que no afecten negativamente a la sociedad humana.

## 1.2.11. El concepto de usabilidad

> [!IMPORTANT]  
> La usabilidad hace referencia a la eficiencia, efectividad y satisfacción con la que un usuario puede interactuar con un sistema digital. Incluye aspectos como la ergonomía y la accesibilidad, permitiendo que el sistema sea intuitivo y fácil de manejar para diferentes tipos de usuarios.

**1) Facilidad de aprendizaje.** El sistema debe ser fácil de aprender, de tal manera que el usuario pueda empezar a trabajar con él lo más rápido posible.

**2) Eficiencia de uso.** Una vez que el usuario haya aprendido a utilizar el sistema, su nivel de productividad debe ser alto para poder completar determinadas tareas.

**3) Facilidad de memorización.** La curva de aprendizaje debe ser significativamente menor en un usuario que ya ha hecho uso del sistema. De esta manera, cuando tenga la necesidad de volver a utilizarlo, todo será más fácil de recordar y no tendrá que emplear tanto tiempo como un usuario que no ha 
utilizado dicho sistema.

**4) Errores.** El sistema debe generar el menor número de errores posible. Si se producen, es importante que se hagan saber de una forma rápida y clara al usuario, a la vez que le ofrece algún mecanismo para recuperarse de ese error.

**5) Satisfacción.** Este atributo se refiere a la impresión subjetiva del usuario respecto al sistema.

### Objetivos de la usabilidad

Es necesario marcar unos objetivos cuantificables que nos ayuden a saber en todo momento si nuestro sitio es fácil de usar por parte de los usuarios en los que hemos pensado. Facilitar al usuario el acceso a un sistema o satisfacer sus necesidades en el menor tiempo posible son factores que optimizan y mejoran la productividad de nuestras acciones y decisiones. No obstante, aún es necesario especificar más.

Apoyándonos en los conceptos que trabajamos al definir la usabilidad, podemos ir marcando objetivos que ayuden a mejorar el producto. Además, debemos formularnos varias preguntas en el equipo de trabajo:

- ¿El target con el que vamos a trabajar está claro?
- ¿Qué proceso, método o técnica vamos a utilizar para medir el objetivo?
- ¿Contaremos con recursos materiales y humanos para medirlo?
- ¿Todo el equipo de trabajo está de acuerdo en medir dicho objetivo?
- ¿El objetivo se adecua al proyecto en su conjunto y facilita la obtención de resultados relevantes?

### Principios de la usabilidad

Un principio sería una solución posible a un problema de diseño que ayuda a definir cómo debe mostrarse y comportarse un sistema, lo que mejora elementos de la interfaz. Conseguimos así que se proporcione a los usuarios lo necesario para interactuar exitosamente y que se presente la información de manera que se facilite su entendimiento.

#### Coherencia
Un sistema debe ser consistente en diseño gráfico e interacción en todas sus secciones, utilizando los mismos elementos visuales, terminología y organización para reducir la carga cognitiva del usuario.

#### Interacción
La interacción debe ser predecible, visible y reversible. Los usuarios deben recibir retroalimentación inmediata tras sus acciones y poder deshacer cambios si es necesario, evitando consecuencias irreversibles.

#### Información, Comunicación y Retroalimentación
Es clave proporcionar múltiples canales de comunicación con los usuarios, garantizando claridad en la estructura y en la forma de acceder a la información. La retroalimentación es fundamental para que los usuarios comprendan su progreso en cada acción.

#### Control
Los usuarios deben poder personalizar la interfaz según sus preferencias, lo que mejora su experiencia y productividad. Opciones como ajustar el tamaño del texto o modificar la disposición de los elementos permiten una mayor accesibilidad.

#### Opciones
Se deben ofrecer múltiples formas de acceder a la información, permitiendo a los usuarios elegir entre enlaces de texto, gráficos, buscadores, índices o mapas del sitio. La flexibilidad en la interfaz facilita la adaptación a diferentes capacidades y contextos de uso.

## 1.2.12. Problemas de usabilidad en dispositivos digitales

### Tabletas

- Los toques accidentales provocan selecciones no deseadas.
- Difícil de aprender las distintas funciones gestuales de los diferentes fabricantes.
- Escalado y control de zoom deficientes o de mala calidad.
- Controles difíciles de usar.
- Botones laterales pequeños.
- Instrucciones mal redactadas.

### Consolas de videojuegos

- Algunas consolas portátiles tienen pantallas relativamente pequeñas.
- Los botones pueden ser demasiado pequeños.
- Difíciles de usar en exteriores (brillo insuficiente).
- Vida de batería corta.


### Ordenadores personales (PCs)

- El uso excesivo del teclado puede provocar **RSI (síndrome de lesiones por esfuerzo repetitivo)**.
- El uso excesivo de una pantalla grande y brillante puede causar **problemas de visión** o cansancio ocular.
- Una **iluminación deficiente en la habitación** puede generar reflejos molestos en la pantalla.
- El ratón del PC está diseñado para **personas diestras**, lo que dificulta su uso a las personas zurdas.

## 1.2.13. Métodos para mejorar la accesibilidad en los sistemas

> [!IMPORTANT]  
> El **diseño centrado en el usuario (DCU)** asume que todo el proceso tiene que estar orientado hacia las necesidades y objetivos del usuario y éstos deben estar involucrados desde el comienzo en el proceso de diseño.

Pretendemos lograr que la experiencia de uso de los usuarios sea satisfactoria y esto implica conocer bien su comportamiento y sus reacciones ante los diseños que conceptualizamos y construimos. Involucrar a los usuarios en el proceso de diseño significa tener en cuenta sus necesidades, preferencias y limitaciones. Esto lo lograremos, como veremos más adelante, siguiendo las etapas propuestas y aplicando métodos en cada etapa.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%2010.%20Fundamento%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="708" height="auto"/>
    <p><em>Figura 10: Expectativas en el diseño. Fuente: adaptado de Flickr</em></p>
  </div>

El DCU algunos expertos lo dividen en 5 etapas. Algunas de las cuales tienen, carácter iterativo:

**1) Planificación del proceso centrado en el usuario:** identificación del propósito del sistema interactivo, necesidades, requerimientos y objetivos de sus usuarios potenciales.

**2) Análisis del contexto de uso:** la calidad de uso del sistema dependerá de la comprensión y la planificación de las características de los usuarios, de las tareas y también del entorno físico y organizativo en el que el sistema será utilizado.

**3) Análisis del usuario y requisitos de la organización:** identificación de los objetivos específicos del usuario y los requerimientos que el producto deberá satisfacer.

**4) Creación de soluciones de diseño:** elaboración de propuestas de diseño mediante simulaciones o prototipos haciendo uso de todo el conocimiento disponible.

**5) Evaluación de la usabilidad:** tarea esencial que, junto con la etapa anterior, se beneficia del diseño iterativo para alcanzar los objetivos propuestos.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/images/Figura%2011.%20Fundamento%20de%20dise%C3%B1o%20de%20sistemas.png" alt="Fundamentos de diseño de sistemas" width="708" height="auto"/>
    <p><em>Figura 11: Etapas del DCU. Fuente: UOC</em></p>
  </div>

## 1.2.14. Implicaciones morales, éticas, sociales, económicas y ambientales de la interacción entre humanos y máquinas

La **Inteligencia Artificial (IA)** y la **robótica** son dos campos de la informática que apuntan hacia un futuro muy diferente. Una pregunta difícil aún sin respuesta es: ¿cómo podemos **replicar a los seres vivos** utilizando chips de silicio, redes informáticas y software?

Los avances en IA hacen posible predecir que en un futuro cercano, las computadoras alcanzarán algún tipo de inteligencia. Sin embargo, la vida artificial no posee dos de las principales características asociadas con la vida orgánica planetaria:

- No está basada en carbono y agua.
- No ha evolucionado junto con otras formas de vida.

Muchos científicos están preocupados porque los avances en IA puedan conducir a situaciones **impredecibles y peligrosas**, sin control humano sobre los robots inteligentes.

Imagina una situación donde la **manipulación de sonido, imagen o video** engañe a tus sentidos para hacerte experimentar algo que nunca ocurrió. Es aceptable ver una película de ciencia ficción o escuchar voces digitalmente modificadas, pero es inaceptable **chantajear a alguien con un video alterado digitalmente**.

Las acciones deben considerarse bajo diferentes marcos:

- La **religión, la sociedad, la profesión y la familia** establecen el marco ético.
- Los **principios personales** establecen la moral.

A pesar de las predicciones en contra, la TI ha **aumentado drásticamente la cantidad de papel impreso**. Incluso cuando los usuarios son cuidadosos con la impresión, enormes cantidades de papel acaban cada día en el contenedor de reciclaje. Y aun reciclar papel requiere un **uso intensivo de químicos y energía**. Las consecuencias ambientales deben tenerse en cuenta al imprimir documentos desde la computadora.

Además, los **residuos electrónicos** contienen plomo, cadmio, mercurio, cromo, PVC y otros productos químicos peligrosos que terminan en vertederos, provocando contaminación.

La **brecha digital** existe no solo entre hogares de ingresos altos y bajos, sino también entre países. Portátiles, tabletas, teléfonos inteligentes, pizarras digitales interactivas, multimedia, tecnologías inalámbricas, motores de búsqueda, redes sociales, intercambio de archivos, música y fotografía digital, y otras tecnologías de vanguardia forman parte de la vida diaria de los afortunados, pero son solo un sueño para muchos otros.

Las consecuencias de la brecha digital generan una **creciente desigualdad** y una reducción de las oportunidades de educación, entretenimiento e ingresos.
