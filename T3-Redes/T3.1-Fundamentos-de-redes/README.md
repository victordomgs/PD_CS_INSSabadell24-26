<h1 align="center">3.1. Fundamentos de redes
<div align="center">

</div>

## Contenido:

[3.1.1. Diferentes tipos de redes](#3.1.1.-diferentes-tipos-de-redes)

[3.1.2. Importancia de los estándares en la construcción de redes](#3.1.1.-importancia-de-los-estándares-en-la-construcción-de-redes)

[3.1.3. Capas en la comunicación de red](#3.1.3.-capas-en-la-comunicación-de-red)

[3.1.4. Introducción a VPN](#3.1.4.-introducción-a-vpn)

[3.1.5. Uso de VPN](#3.1.4.-uso-de-vpn)

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
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%203.%20Redes.png" alt="Local Area Network" width="390" height="auto"/>
    <p><em>Figura 3: Local Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

Otro beneficio de formar una LAN es que, además de los periféricos, también se pueden compartir datos. Esto permite el intercambio de información entre clientes, eliminando la necesidad de enviar físicamente los datos mediante otros medios, como el intercambio de CD o memorias USB. Esto incrementa la flexibilidad y reduce la pérdida de tiempo.

La tecnología más común utilizada para construir LAN cableadas es un hub o un switch con cableado Ethernet. La Figura 4 muestra una LAN cableada compuesta por un servidor, tres clientes y una impresora conectada al servidor a través de un hub o un switch.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%204.%20Redes.png" alt="Local Area Network" width="290" height="auto"/>
    <p><em>Figura 4: Local Area Network. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>


### Red de Área Local Inalámbrica (WLAN)

Una WLAN conecta dos o más sistemas informáticos dentro de un área geográfica limitada, de forma similar a una LAN. La diferencia con una LAN es que los dispositivos de una WLAN están conectados mediante algún tipo de método de conexión inalámbrica. Esto permite que los usuarios tengan dispositivos móviles y portátiles conectados a la red y puedan desplazarse libremente.

Las WLAN tienen todos los beneficios de las LAN, además de la facilidad de la conexión inalámbrica, que permite el uso de dispositivos móviles en movimiento. Sin embargo, las WLAN pueden ser menos seguras que las LAN cableadas, ya que un posible intruso no necesita tener una conexión física con la red. Por ejemplo, un intruso podría intentar acceder a la WLAN de una escuela incluso desde fuera del recinto escolar si la señal de la red inalámbrica es lo suficientemente fuerte.

La tecnología más común utilizada para construir LAN inalámbricas es Wi-Fi, que permite el intercambio de datos entre sistemas informáticos utilizando ondas de radio. La Figura 5 muestra una LAN compuesta por un servidor, tres clientes y una impresora conectada al servidor. Dos de los clientes están conectados de manera inalámbrica a través de un hub o switch inalámbrico.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%205.%20Redes.png" alt="Local Area Network" width="290" height="auto"/>
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
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%206.%20Redes.png" alt="Virutal Local Area Network" width="350" height="auto"/>
    <p><em>Figura 6: Virtual Local Area Network con dos redes lógicas separadas. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>


## 3.1.2. Importancia de los estándares en la construcción de redes
## 3.1.3. Capas en la comunicación de red
## 3.1.4. Introducción a VPN
## 3.1.5. Uso de VPN
