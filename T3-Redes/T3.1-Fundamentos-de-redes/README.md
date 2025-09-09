<h1 align="center">3.1. Fundamentos de redes
<div align="center">

</div>

## Contenido:

[3.1.1. Diferentes tipos de redes](#311-diferentes-tipos-de-redes)

[3.1.2. Importancia de los estándares en la construcción de redes](#311-importancia-de-los-estándares-en-la-construcción-de-redes)

[3.1.3. Capas en la comunicación de red](#313-capas-en-la-comunicación-de-red)

[3.1.4. Introducción a VPN](#314-introducción-a-vpn)

[3.1.5. Uso de VPN](#314-uso-de-vpn)

---

A continuación se muestran algunos de los conceptos esenciales que se trabajarán a lo largo del temario: 

| **Término** | **Definición** |
|-------------|----------------|
| **topología en bus** | Red de computadoras en la que un “bus” conecta todos los dispositivos mediante un cable común. |
| **cable** | Cable de cobre (normalmente coaxial y par trenzado) y fibra óptica (hecha de vidrio). Los cables permiten la conexión de computadoras a través de una red. |
| **dígito de verificación** | Dígito adicional añadido a los datos numéricos que se utiliza para comprobar la integridad de los datos después de la entrada, transmisión, almacenamiento o procesamiento. |
| **integridad de datos** | Precisión de los datos después de la entrada, transmisión, almacenamiento o procesamiento. |
| **suma de verificación** | Procedimiento de detección de errores que genera una suma a partir de los dígitos de un número. |
| **paquete de datos** | Parte de un mensaje que se transmite a través de una red. Contiene datos como dígitos de verificación y dirección de destino. |
| **puerta de enlace** | Enlace que reside entre redes de computadoras y es responsable de convertir los datos en el formato adecuado para que puedan ser entendidos por la red receptora. |
| **intercambio de señales** | Intercambio de señales predeterminadas para indicar que se ha establecido una conexión entre dos sistemas. |
| **concentrador** | Punto de conexión de red para dispositivos. Los datos que llegan a un hub se copian y se envían a todos los dispositivos de la red. |
| **ISDN (Integrated Services Digital Network)** (Red Digital de Servicios Integrados) | Estándar internacional de comunicaciones que permite la transmisión de audio, video y otros datos a través de líneas telefónicas digitales. |
| **local area network (LAN)** (red de área local) | Red de computadoras donde todas las máquinas conectadas se encuentran en un área geográfica limitada (ej. una casa, escuela, etc.). La conexión puede realizarse mediante cables y/o transmisión por microondas. |
| **transmisión por microondas** | Comunicación electrónica sin necesidad de cables. |
| **modem (modulador/demodulador)** | Equipo electrónico que convierte señales digitales de computadora en señales de audio y viceversa. Las señales de audio se transmiten a través de líneas telefónicas, lo que permite la comunicación a distancia. |
| **network** (red) | Sistemas informáticos que están interconectados y pueden compartir recursos y datos. |
| **packet** (paquete) | Grupo de bits. Puede incluir señales de control, bits de error, información codificada, así como el destino de los datos. |
| **packet switching** (conmutación de paquetes) | Método de comunicación en red que crea y transmite pequeñas unidades de datos, llamadas paquetes, a través de la red de manera independiente del mensaje completo. |
| **networking** (uso de redes) | Utilización de una red. |
| **bit de paridad** | Procedimiento de detección de errores que añade un bit binario a un grupo de dígitos binarios. La suma de todos los dígitos, incluido el bit añadido, establece la precisión de los datos después de la entrada, transmisión, almacenamiento o procesamiento. |
| **protocol** (protocolo) | Reglas internacionales que garantizan la transferencia de datos entre sistemas. Un protocolo reconocido como estándar para un tipo específico de transferencia se llama protocolo estándar. Ejemplo: TCP/IP es un protocolo estándar. |
| **TCP/IP (Transmission Control Protocol / Internet Protocol)** | Protocolos de comunicación usados para conectar hosts en Internet. |
| **wide area network (WAN)** (red de área amplia) | Red de computadoras donde todos los equipos conectados están en un área geográfica mayor que la de una LAN o una MAN (red de área metropolitana). |

---

## 3.1.1. Diferentes tipos de redes

Una red informática está compuesta por dos o más sistemas informáticos que están conectados y son capaces de comunicarse e intercambiar datos. Dichos sistemas informáticos están conectados mediante cable o medios inalámbricos. Hay dos términos clave en las redes informáticas que desempeñan un papel importante:

- Servidor
- Cliente

### Servidor
Un servidor puede ser tanto un sistema informático como una aplicación de software que proporciona un servicio a los otros sistemas informáticos conectados a la misma red. Por ejemplo, un servidor puede ofrecer al resto de ordenadores de la red la capacidad de almacenar y compartir archivos, adoptando el rol de servidor de archivos.

### Cliente
Un cliente puede ser tanto un sistema informático como una aplicación de software que solicita un servicio a un servidor conectado a la misma red. Por ejemplo, una aplicación cliente de correo electrónico puede solicitar a una aplicación de servidor de correo electrónico que recupere los correos electrónicos nuevos que se hayan recibido.

En resumen, un sistema informático servidor es un host que ejecuta aplicaciones de software de servidor y comparte sus recursos con clientes que hacen solicitudes. Un cliente, en cambio, no comparte ninguno de sus recursos, sino que solicita contenido a un servidor. Los servidores, por tanto, esperan solicitudes de contenido por parte de los clientes.

Existen varias maneras de conectar dos o más sistemas informáticos para crear una red. Sin embargo, los tres siguientes son los componentes de red más utilizados y que desempeñan un papel esencial en la creación de una red: Hub, Switch y Router. Aunque estos tres componentes se han integrado en una sola caja, siguen siendo dispositivos diferentes que son esenciales para el trabajo en red y presentan diferencias significativas entre ellos. Un host típico que incluye un hub o un switch y un router cableado o inalámbrico sería similar al dispositivo representado en la Figura 1.

  <div style="text-align: center;">
    <img src="https://thumb.pccomponentes.com/w-530-530/articles/1081/10813982/1416-tp-link-er706w-router-inalambrico-vpn-gigabit-omada-ax3000-doble-banda.jpg" alt="Switch Hub" width="321" height="auto"/>
    <p><em>Figura 1: Switch Hub. Fuente: PcCompomentes</em></p>
  </div>

### Concentradores (Hubs)
Un hub es el punto de conexión para los dispositivos en una sola red. Los dispositivos de red y los sistemas informáticos se conectan a un hub utilizando cables Ethernet que se conectan a un puerto. Por ejemplo, el hub de la Figura 3.1 tiene ocho puertos, lo que significa que ocho dispositivos o sistemas informáticos pueden conectarse a él. Así, un hub consta de múltiples puertos.
Cuando un dispositivo de red quiere enviar datos a otro dispositivo en la red, los envía al hub. El hub entonces copia los datos y los envía a todos los dispositivos conectados a sus puertos. El dispositivo que espera recibir los datos los acepta. Todos los demás simplemente los ignoran. Aunque enviar los datos a todos los puertos garantiza que llegarán a su destino, también se genera mucho tráfico en la red, ya que todos los demás puertos, aunque ignoren los datos, igualmente los reciben. Esto ralentiza la red.

### Conmutadores (Switches)
Un switch también es un punto de conexión para múltiples dispositivos en una sola red. Sin embargo, a diferencia de un hub, el switch puede identificar qué dispositivo de red está conectado a qué puerto. Esto permite que el switch transmita los datos exactamente al puerto y al dispositivo de red para los cuales están destinados.
Esto significa que cuando un dispositivo de red quiere enviar datos a otro dispositivo en la red, los envía al switch y el switch transmite los datos únicamente al receptor apropiado en lugar de a todos los puertos y dispositivos conectados a ellos. De esta forma, las redes conectadas con un switch son más rápidas que las redes conectadas con un hub.

### Enrutadores (Routers)
Un router es un dispositivo más sofisticado que tanto un hub como un switch. Su función es unir múltiples redes y servir de intermediario entre ellas para que los datos puedan intercambiarse de manera efectiva y eficiente entre los dispositivos de red.
Por ejemplo, un router se utiliza para conectar una red doméstica a Internet. Un hub o un switch no podrían realizar esta tarea de una manera sencilla.

Como se ha mencionado, un hub o un switch y un router suelen estar integrados en una sola caja, lo que permite la creación de una red cableada o inalámbrica, así como la conexión de esa red a otras redes, como Internet.

Existen varios tipos diferentes de redes que pueden establecerse, así como distintos protocolos o “reglas” que deben seguirse para que los sistemas informáticos implicados puedan intercambiar datos de manera eficiente.
Los tipos de red que se describirán brevemente son los siguientes:

- Red de Área Local (LAN)
- Red de Área Local Inalámbrica (WLAN)
- Red de Área Local Virtual (VLAN)
- Red de Área Amplia (WAN)
- Red de Área de Almacenamiento (SAN)
- Internet
- Extranet
- Red Privada Virtual (VPN)
- Red de Área Personal (PAN)
- Red entre Pares (P2P)

Todos los tipos de redes descritos a continuación han contribuido al fenómeno de la globalización en las últimas décadas. La globalización ha sido acelerada por los avances técnicos relacionados con el desarrollo de las redes. Todas estas diferentes redes han desempeñado su papel en la interconexión de sistemas informáticos, ya sea a nivel local o global, permitiendo así que personas de todo el mundo se comuniquen, hagan negocios, etc.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%202.%20Redes.png" alt="Computer Network type" width="470" height="auto"/>
    <p><em>Figura 2: Redes por tamaño espacial. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

### Red de Área Local (LAN)
Una LAN es una red informática que conecta sistemas informáticos dentro de un área geográfica limitada, como una habitación, una casa, un edificio de oficinas o una escuela. Los sistemas informáticos interconectados mediante una LAN suelen tener altas tasas de transferencia de datos entre ellos.

Comúnmente se utiliza un modo de operación cliente-servidor. Esto permite que un único sistema informático actúe como servidor y sea responsable de proporcionar diversos servicios a los clientes de la red.

Las LAN permiten compartir dispositivos periféricos entre los sistemas informáticos conectados. Esto significa que dispositivos periféricos, como impresoras, escáneres o discos duros externos, pueden ser utilizados por cualquier sistema informático de la LAN que lo desee. Esto elimina la necesidad de comprar ciertos periféricos para cada ordenador.

Por ejemplo, en lugar de tener que comprar varias impresoras, se puede adquirir una sola impresora y conectarla al servidor de la LAN, de modo que el resto de los sistemas informáticos (los clientes) accedan y compartan la impresora a través del servidor.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%203.%20Redes.png" alt="Local Area Network" width="470" height="auto"/>
    <p><em>Figura 3: Local Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

Otro beneficio de formar una LAN es que, además de los periféricos, también se pueden compartir datos. Esto permite el intercambio de información entre clientes, eliminando la necesidad de enviar físicamente los datos mediante otros medios, como el intercambio de CD o memorias USB. Esto incrementa la flexibilidad y reduce la pérdida de tiempo.

La tecnología más común utilizada para construir LAN cableadas es un hub o un switch con cableado Ethernet. La Figura 4 muestra una LAN cableada compuesta por un servidor, tres clientes y una impresora conectada al servidor a través de un hub o un switch.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%204.%20Redes.png" alt="Local Area Network" width="420" height="auto"/>
    <p><em>Figura 4: Local Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>


### Red de Área Local Inalámbrica (WLAN)

Una WLAN conecta dos o más sistemas informáticos dentro de un área geográfica limitada, de forma similar a una LAN. La diferencia con una LAN es que los dispositivos de una WLAN están conectados mediante algún tipo de método de conexión inalámbrica. Esto permite que los usuarios tengan dispositivos móviles y portátiles conectados a la red y puedan desplazarse libremente.

Las WLAN tienen todos los beneficios de las LAN, además de la facilidad de la conexión inalámbrica, que permite el uso de dispositivos móviles en movimiento. Sin embargo, las WLAN pueden ser menos seguras que las LAN cableadas, ya que un posible intruso no necesita tener una conexión física con la red. Por ejemplo, un intruso podría intentar acceder a la WLAN de una escuela incluso desde fuera del recinto escolar si la señal de la red inalámbrica es lo suficientemente fuerte.

La tecnología más común utilizada para construir LAN inalámbricas es **Wi-Fi**, que permite el intercambio de datos entre sistemas informáticos utilizando ondas de radio. La Figura 5 muestra una LAN compuesta por un servidor, tres clientes y una impresora conectada al servidor. Dos de los clientes están conectados de manera inalámbrica a través de un hub o switch inalámbrico.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%205.%20Redes.png" alt="Local Area Network" width="420" height="auto"/>
    <p><em>Figura 5: Local Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

> [!NOTE]  
> Cuadro comparativo de las similitudes y diferencias entre LAN y WLAN:
> | **LAN - WLAN** | **Similitudes** | **Diferencias** |
> |----------------|-----------------|-----------------|
> |                | Ambas actúan a nivel local. | Usan diferentes medios de transmisión. |
> |                | Ambas permiten la comunicación. | Una LAN es más segura. |
> |                | Ambas se utilizan para conectar dispositivos. | La LAN es más rápida. |
> |                | Ambas permiten compartir recursos. | Las WLAN ofrecen mayor flexibilidad. |


### Virtual Local Area Network (VLAN)

Imagina que una empresa ha creado una LAN y ha conectado todos sus sistemas informáticos y departamentos entre sí. Departamentos como contabilidad, recursos humanos, ventas y producción han sido interconectados, y todos los sistemas informáticos, de cualquier departamento, pueden acceder a los recursos compartidos de cualquier otro departamento. Eso puede no ser deseable, ya que algunos departamentos pueden no querer o no necesitar intercambiar datos entre sí, y tener acceso a los recursos compartidos de otros podría causar confusión en lugar de ayudar.

La solución a este problema sería configurar una LAN para cada departamento, de modo que cada uno tenga su propia red aislada que no pueda ser accedida desde el exterior. Estas LAN podrían conectarse entre sí, enlazando el switch de cada LAN a un switch central, de forma que sea posible comunicarse entre ellas cuando sea necesario, pero sin tener acceso directo a los recursos compartidos de los demás.

En lugar de tener que instalar switches y cableado adicional para crear LAN separadas para cada departamento, se puede utilizar una VLAN para dividir la LAN inicial (donde están conectados todos los departamentos) en redes lógicas separadas. Cada red lógica separada no puede ver los sistemas informáticos ni los recursos compartidos de las demás redes lógicas, salvo que se configure específicamente para permitir dicho acceso.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%206.%20Redes.png" alt="Virutal Local Area Network" width="570" height="auto"/>
    <p><em>Figura 6: Virtual Local Area Network con dos redes lógicas separadas. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

La Figura 6 muestra una VLAN compuesta por dos servidores (cada uno para un departamento diferente de una empresa) y cuatro clientes (dos en cada departamento). La VLAN está configurada de tal manera que la LAN se segmenta en dos redes lógicas más pequeñas y separadas.

> [!NOTE] 
> Cuadro comparativo de las similitudes y diferencias entre LAN y VLAN:
> | **LAN - VLAN** | **Similitudes** | **Diferencias** |
> |----------------|-----------------|-----------------|
> |                | Ambas actúan a nivel local. | Una VLAN ofrece mejor rendimiento. |
> |                | Ambas tienen los mismos atributos. | Una VLAN es más segura. |
> |                | Ambas permiten la comunicación. | La formación de grupos de trabajo virtuales es sencilla. |
> |                | Ambas se utilizan para conectar dispositivos. | Las VLAN ofrecen mayor flexibilidad. Incluso si alguien que usa un portátil se mueve a otro lugar, seguirá en su VLAN dedicada. |
> |                | Ambas permiten compartir recursos. | La partición de recursos es más sencilla. |
> |                |  | Las VLAN son independientes del medio y de la topología física de la red. |
> |                |  | A veces la gestión/administración de una VLAN es compleja. |

> [!NOTE] 
> Pros y contras de LAN y VLAN
> | **LAN** | Pros | Cons | **VLAN** | Pros | Cons |
> |---------|------|------|----------|------|------|
> |         | A veces la gestión de una LAN es más sencilla. | Una LAN ofrece peor rendimiento. |          | Una VLAN ofrece mejor rendimiento. | A veces la gestión de una VLAN es compleja. |
> |         |      | Una LAN no es tan segura. |          | Una VLAN es más segura. | Una red puede acomodar un número máximo de VLAN (este número es grande, por lo que no es una desventaja real). |
> |         |      | No permite la formación de grupos de trabajo virtuales. |          | La formación de grupos de trabajo virtuales es sencilla. |      |
> |         | LANs ofrecen menos flexibilidad. |      |          | Las VLAN ofrecen mayor flexibilidad. Incluso si alguien que usa un portátil se mueve a otro lugar, seguirá en su VLAN dedicada. |      |
> |         |      | La partición de recursos es más difícil. |          | La partición de recursos es más sencilla. |      |
> |         | LANs dependen del medio y de la topología física de la red. |      |          | Las VLAN son independientes del medio y de la topología física de la red. |      |

### Red de Área Amplia (WAN)

Una WAN es una red informática que conecta sistemas informáticos dentro de una gran área geográfica. El ejemplo más evidente de una WAN es **Internet**.
Una WAN cubre un área extensa, como una ciudad, un país o incluso una red de países, lo que permite que individuos, empresas y gobiernos realicen sus actividades diarias sin importar su ubicación.

Típicamente, una WAN está compuesta por **LANs interconectadas** a lo largo de un área geográfica amplia. La Figura 7 muestra una WAN compuesta por cuatro LANs conectadas entre sí en distintas partes del mundo.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%207.%20Redes.png" alt="Wide Area Network" width="370" height="auto"/>
    <p><em>Figura 7: Wide Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

### Red de Área de Almacenamiento (SAN)

Una SAN es una red creada para que **grandes dispositivos de almacenamiento** puedan ser accesibles desde los servidores de forma conveniente y sencilla.

En una red (por ejemplo, la LAN de una empresa) puede haber varios servidores conectados.
En la Figura 8, se muestra una LAN con cuatro clientes (dos de ellos conectados de forma inalámbrica) y tres servidores, todos conectados mediante un Hub/Switch.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%208.%20Redes.png" alt="Wide Area Network" width="570" height="auto"/>
    <p><em>Figura 8: WAN conectada a una LAN empresarial. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

Los **tres servidores** proporcionan servicios distintos a los clientes:

- Un **servidor de correo**, responsable de gestionar los emails.
- Un **servidor de aplicaciones**, encargado de gestionar aplicaciones centralizadas que pueden ser utilizadas por los clientes.
- Un **servidor de bases de datos**, encargado de gestionar los datos de la empresa almacenados en una base de datos (por ejemplo, una lista de clientes con sus datos).

Estos servidores requieren espacio de almacenamiento para guardar su información y crear **copias de seguridad** que eviten la pérdida de datos en caso de fallo del almacenamiento.
Aquí es donde se necesita la **red de área de almacenamiento (SAN)**: una red que conecta los servidores con los dispositivos de almacenamiento para que dispongan del espacio necesario para realizar sus tareas.

La SAN de la Figura 8 está compuesta por tres **dispositivos de almacenamiento** conectados a los tres servidores mediante un switch y cableado Ethernet.

### Internet

Internet es una WAN global que conecta millones de sistemas informáticos.
Al ser una WAN, Internet conecta un gran número de redes más pequeñas entre sí, creando así la red WAN más grande, utilizada por miles de millones de usuarios en todo el mundo.

Internet proporciona a los usuarios una amplia variedad de servicios, como la **World Wide Web (WWW)**, que consiste en sitios web y páginas web, además de soporte para correo electrónico, transferencia de archivos y otros servicios.
Por lo tanto, **Internet no es lo mismo que la WWW**, sino que la WWW es un **servicio dentro de Internet**.

A diferencia de otras redes, **Internet está descentralizada por diseño**. Esto significa que sus recursos no están almacenados ni controlados de manera centralizada por un único servidor.
Cada sistema informático conectado a Internet es independiente y puede compartir servicios con la comunidad global, convirtiéndose, en esencia, en un **servidor por sí mismo**.

En la mayoría de los casos, el acceso a Internet se realiza a través de un **Proveedor de Servicios de Internet (ISP)**, que es una empresa que proporciona servicios de conexión a cambio de una cuota mensual.
A diferencia de la mayoría de las LAN y WAN, **Internet no pertenece a una sola entidad** (persona u organización).

### Internet de las Cosas (IoT)

El Internet de las Cosas (IoT) es la red de “cosas” individuales que pueden conectarse a Internet, comunicarse e intercambiar datos.
Cada “cosa” cuenta con el hardware y software necesarios y tiene asignada una dirección IP.

Ejemplos de “cosas” en el IoT incluyen:

- Un paciente con un implante.
- Un coche con un sistema de emergencia.
- Un sistema de alarma con aviso avanzado.
- Un animal salvaje con un sistema de rastreo.

Cada objeto físico tiene un sistema embebido único que lo identifica de manera exclusiva.

### Extranet

Una extranet es una red informática que utiliza Internet para permitir el acceso controlado de usuarios específicos a una LAN o WAN concreta.

Por ejemplo, imagina una empresa que gestiona una red de sistemas informáticos para sus operaciones diarias. Esta red privada está contenida dentro de la empresa, ya sea una LAN o una WAN, y solo puede ser accedida por el personal que tenga las credenciales necesarias (por ejemplo, nombre de usuario y contraseña).

La empresa puede desear **compartir de manera segura una parte de su red (y de su información)** con proveedores, socios, clientes u otras empresas, sin hacer que toda su red esté disponible para ellos o para el público en general.

A esta parte de la red que se extiende a usuarios externos autorizados se le denomina extranet.

Las extranets requieren técnicas de **seguridad y privacidad**, de manera que el público o los usuarios externos no puedan acceder a datos confidenciales.

En otras palabras, una extranet puede considerarse como una **intranet que es parcialmente accesible para usuarios externos autorizados**.

Un **firewall** controla los derechos de acceso y permite el ingreso a la intranet únicamente a las personas autorizadas.

### Red Privada Virtual (VPN)

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%209.%20Redes.png" alt="Virtual Private Network" width="370" height="auto"/>
    <p><em>Figura 9: Virtual Private Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

Imagina que una empresa tiene una LAN que conecta dos o más sistemas informáticos dentro de un área geográfica limitada, como su oficina.
Ahora imagina que algunos empleados necesitan viajar al extranjero por trabajo, pero aun así requieren acceder a la LAN de la empresa para utilizar archivos y recursos compartidos.
Eso no sería posible con una LAN, o incluso con una WLAN, si el empleado está lejos y no puede conectarse físicamente mediante cable o de forma inalámbrica.

Aquí es donde una VPN resuelve el problema.

Una VPN es una red informática que conecta dos o más sistemas, similar a una LAN o una WLAN, pero que además permite a clientes en ubicaciones remotas conectarse a la red y **aparecer como si estuvieran dentro de la LAN**, como si estuvieran presentes físicamente.

En otras palabras, una VPN permite la creación de una LAN gestionada a través de una aplicación de servidor, a la cual los clientes pueden conectarse también desde ubicaciones remotas, incluso a través de otra red (por ejemplo, Internet).

Una VPN ofrece **todos los beneficios de una LAN**, permitiendo a los usuarios compartir datos y recursos sin comprometer la seguridad.
Además, una VPN puede **conectar de manera segura y rentable oficinas geográficamente dispersas de una empresa**, dentro de una red que dispone de todas las funcionalidades de una única LAN.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2010.%20Redes.png" alt="Virtual Private Network" width="370" height="auto"/>
    <p><em>Figura 10: A virtual private network (VPN). Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

La Figura 10 muestra una VPN compuesta por un servidor, dos clientes y una impresora conectada al servidor.
Uno de los clientes está conectado a la VPN de forma remota a través de Internet, utilizando un nombre de usuario y una contraseña.

### Personal Area Network (PAN)

Una PAN es una red que interconecta dispositivos centrados en el espacio de trabajo de una persona.
Se puede entender como una **LAN que solo da soporte a un individuo** en lugar de a un grupo de personas, y que cubre un rango muy corto, de un máximo de **10 metros**.

Un ejemplo típico de PAN sería un ordenador portátil, un smartphone y una tableta interconectados y compartiendo datos como correos electrónicos, calendarios, fotografías, etc.

Los dispositivos en una PAN pueden conectarse tanto de forma **cableada** (normalmente mediante USB) como de forma inalámbrica (normalmente mediante Bluetooth), según las tecnologías utilizadas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2011.%20Redes.png" alt="Personal Area Network" width="370" height="auto"/>
    <p><em>Figura 11: Personal Area Network (PAN). Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

Una PAN que utiliza un grupo de dispositivos inalámbricos mediante tecnología **Bluetooth** para interconectarse también se conoce como **piconet**.

### Red entre Pares (P2P)

Una **P2P** es una red que **no utiliza el modelo cliente/servidor**, en el que los clientes solicitan recursos y los servidores los proporcionan.

En lugar de ello, una red P2P emplea una **arquitectura de red distribuida** donde todos los sistemas informáticos (llamados nodos o peers) están **descentralizados** y actúan **tanto como clientes como servidores al mismo tiempo**, consumiendo y suministrando recursos de y hacia los demás sistemas conectados a la red.

El modelo P2P elimina la dependencia de servidores centralizados, evitando posibles **cuellos de botella**, y permite que cada ordenador aporte parte de sus recursos para que otros puedan utilizarlos.

## 3.1.2. Importancia de los estándares en la construcción de redes

Imagina que una empresa necesita configurar una LAN con varios clientes y servidores.
Si el hardware no sigue algunas reglas comunes (o estándares específicos), es posible que los sistemas informáticos no puedan interconectarse para crear la red.

**Información útil:** existen dos organizaciones que estandarizan los protocolos de red:

- **Institute of Electrical and Electronics Engineers (IEEE)**
- **Internet Engineering Task Force (IETF)**

Si existieran muchos estándares distintos y los fabricantes de hardware o software siguieran cada uno diferentes, el resultado sería **hardware y software incompatibles**.
Por ejemplo, en una situación hipotética sin estándares, podría desarrollarse un sistema informático que solo admitiese **puertos USB**, mientras que un switch se desarrollase únicamente con soporte para **puertos Ethernet**. Estos dos elementos de hardware no podrían conectarse entre sí, ya que estarían utilizando estándares de comunicación diferentes.

Los **estándares** desempeñan un papel fundamental en la construcción de redes.
Los estándares describen una **base común** en la que los fabricantes de hardware y software (Apple, Microsoft, Linux, etc.) pueden apoyarse para construir sistemas capaces de comunicarse entre sí.

En este sentido, los estándares pueden considerarse como un **“lenguaje internacional común”** que permite la **compatibilidad** entre todos los sistemas informáticos a nivel global.

## 3.1.3. Capas en la comunicación de red
## 3.1.4. Introducción a VPN
## 3.1.5. Uso de VPN
