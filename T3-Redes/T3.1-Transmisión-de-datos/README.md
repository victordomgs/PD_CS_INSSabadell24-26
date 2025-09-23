<h1 align="center">3.1. Transmisión de datos
<div align="center">

</div>

## Contenido:

- [3.1.6. Protocolo y paquete de datos](#316-protocolo-y-paquete-de-datos)
- [3.1.7. Necesidad de los protocolos](#317-necesidad-de-los-protocolos)
- [3.1.8. Velocidad de transmisión de datos en red](#318-velocidad-de-transmisión-de-datos-en-red)
- [3.1.9. Compresión de datos](#319-compresión-de-datos)
- [3.1.10. Características según el tipo de transmisión](#3110-características-según-el-tipo-de-transmisión)
- [3.1.11. Conmutación de paquetes](#3111-conmutación-de-paquetes)

---

## 3.1.6. Protocolo y paquete de datos

### Packet (paquete)

Grupo de bits. Puede incluir señales de control, bits de error, información codificada, así como el destino de los datos.

### Protocol (protocolo)

Reglas internacionales que garantizan la transferencia de datos entre sistemas. Un protocolo reconocido como estándar para un tipo específico de transferencia se llama protocolo estándar. Ejemplo: TCP/IP es un protocolo estándar.

## 3.1.7. Necesidad de los protocolos

### Protocolos de comunicación

Sin **reglas predefinidas**, la comunicación sería imposible. Estas reglas se llaman **protocolos**. Pueden entenderse como **normas estrictas y predefinidas**.

Algunos de los elementos que deben cumplirse para que la comunicación tenga lugar incluyen:

1. La presencia de un **emisor identificado**.
2. La presencia de un **receptor identificado**.
3. La existencia de un **método de comunicación acordado** (correo electrónico, mensajería instantánea, smartphone, gestos, conversación cara a cara, teléfono, fax, carta, fotografía, etc.).
4. El uso de un **lenguaje común**.
5. La presencia de una **gramática común**.
6. El acuerdo sobre la **velocidad y el tiempo de entrega** (ejemplo: “¡Hablas demasiado rápido, baja el ritmo!”).
7. La existencia de **mecanismos de confirmación o acuse de recibo** (ejemplo: “¿Tiene sentido lo que digo?” – “No, por favor explícalo de nuevo”).

### Qué proporcionan los protocolos de red

Los **protocolos de red** también proporcionan:

- Reglas sobre el **formato de los mensajes**.
- Reglas sobre cómo los **dispositivos intermedios** deben facilitar la comunicación.
- Reglas sobre la **iniciación y finalización** de una sesión de comunicación.
- Reglas sobre el **tipo de verificación de errores** a utilizar.
- Reglas sobre los **métodos y algoritmos de compresión de datos** (si se utiliza compresión).
- Reglas sobre mecanismos de **detección y corrección de errores**.
- Reglas sobre la **recuperación y reenvío de datos**.

### Garantías que ofrecen los protocolos de red

- **Integridad de datos:** Asegura que la información **no ha sido alterada o corrompida** (de manera intencional o accidental) durante la transmisión, desde el origen hasta el destino. Los mecanismos de **checksum** ayudan a garantizar esta integridad.
- **Integridad del origen:** Verifica la identidad del remitente. Las **firmas digitales** prueban la autenticidad del emisor.
- **Control de flujo:** Las infraestructuras de red tienen memoria y ancho de banda limitados. La **capa de transporte** ajusta la velocidad de transmisión cuando se produce sobrecarga de recursos. Puede solicitar a una aplicación emisora que reduzca su ritmo de envío de datos.
- **Gestión de la congestión:** La congestión ocurre cuando la **demanda de recursos de red supera la capacidad disponible**.
- **Prevención de interbloqueos (deadlock):** Un **deadlock** ocurre cuando dos o más procesos esperan que el otro finalice, y ninguno lo hace. Se **utilizan temporizadores de persistencia** para resolver la situación.
- **Verificación de errores:** Proceso de detección de errores en la transmisión.
- **Corrección de errores:** Capacidad de **reparar** los errores detectados.

## 3.1.8. Velocidad de transmisión de datos en red

Es importante mencionar que diferentes **medios de transmisión** soportan distintas velocidades. La unidad principal utilizada para medir la transferencia de datos es **bps (bits por segundo)**.

Hoy en día, gracias a las mejoras en las tecnologías de red, se usan unidades mayores como:

- **kbps (kilobits por segundo)**
- **Mbps (megabits por segundo, millones de bits por segundo)**

El **ancho de banda** es la **velocidad teórica máxima** de transferencia de datos en un medio, y depende de:

- La técnica de señalización utilizada.
- Las propiedades físicas del medio.

La **tasa de transferencia real** se llama **throughput**, y está afectada por factores como interferencias, tráfico, número de dispositivos conectados y errores.

En una red con varios segmentos, el **segmento más lento genera un cuello de botella**, limitando la velocidad final. En este caso, el **throughput** solo será tan rápido como el **enlace más lento** en la ruta entre el origen y el destino.

El término **goodput** se refiere a la **tasa de transferencia de datos útiles** (sin contar cabeceras, retransmisiones, etc.).

### Factores que afectan la velocidad de transmisión de datos

- Ancho de banda de la red.
- Velocidad de transferencia de los dispositivos de almacenamiento.
- Interferencias.
- Software malicioso.
- Número de dispositivos conectados.
- Número de usuarios y la demanda en un momento dado (tráfico).
- Pérdida de paquetes y retransmisiones.
- Velocidad de lectura de dispositivos de almacenamiento.
- Segmento más lento en la red.
- Velocidad, tecnología y capacidad del servidor de red.
- Tiempo requerido para la autenticación del usuario y verificaciones de seguridad.
- Tipo de archivos enviados.
- Tipo de medio de transmisión.
- Velocidad de la CPU del PC del usuario.
- RAM / caché de disco del PC del usuario.
- Rendimiento de los subsistemas del PC del usuario.

## 3.1.9. Compresión de datos

Todas las redes tienen un **ancho de banda limitado**. La **compresión de datos** reduce el tamaño de los archivos transmitidos a través de la red.

- Un archivo comprimido **ocupa menos ancho de banda**.
- Al reducir su tamaño, también se reduce el **tiempo necesario para enviarlo**.

La **compresión de datos** (también llamada reducción de tasa de bits) consiste en **reducir la cantidad de bits** mediante la codificación de los datos con menos bits que la representación original.

La compresión de archivos es muy usada al **enviar un archivo de un ordenador a otro**, ya que:

- Hace que el archivo sea más pequeño.
- Permite transferencias más rápidas.
- No implica pérdida de datos.

> [!IMPORTANT]  
> El receptor debe contar con un programa que **descomprima el archivo**.

### Tipos de compresión de datos

- **Compresión con pérdida (Lossy):** Se acepta cierta pérdida de información. No es posible recuperar el archivo original. Ejemplos: JPEG, MPEG-2.
- **Compresión sin pérdida (Lossless):** Reduce el número de bits eliminando redundancias estadísticas. No se pierde información en el proceso. Ejemplos: programas de compresión–descompresión (ZIP, RAR, 7z).

## 3.1.10. Características según el tipo de transmisión

### Comunicación cableada

**Cable de cobre (conductores metálicos):** Es el tipo de cableado más común en redes de computadoras.Tipos principales:

**- Cable coaxial:** Consiste en dos conductores de cobre. Se utilizó en redes de computadoras y también para señales de TV. **Ventajas:** bajo coste de instalación.

**- Cable de par trenzado no blindado (UTP):** Muy popular en LANs. Fácil de instalar. **Inconvenientes:** susceptible a interferencias eléctricas. **Ventajas:** bajo coste, seguro, adecuado para distancias cortas entre repetidores, utilizado en redes telefónicas.

**- Cable de par trenzado blindado (STP):** Más difícil de instalar que UTP. **Ventaja:** reduce las interferencias.

**- Fibra óptica:** Transmite datos mediante un haz de luz. **Ventajas:** altísimas velocidades, necesita menos repetidores, extremadamente segura. **Inconvenientes:** muy cara. **Usos:** transmisión de datos y líneas telefónicas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2019.%20Redes.jpg" width="450" height="auto"/>
    <p><em>Figura 19: Cable coaxial. Fuente: El cajón del electrónico</em></p>
  </div>

### Comunicación inalámbrica

**- Radio de microondas:** Usado ampliamente en redes de telefonía móvil y LANs. Transmite la información a través del aire. **Ventajas:** alto ancho de banda (pero menor que los cables). **Inconvenientes:** requiere línea de visión (sin edificios u obstáculos), afectado por el clima, menos seguro que la comunicación cableada, difícil garantizar fiabilidad.

**- Satélites:** Usan señales de microondas para transmisión a grandes distancias.

**- Infrarrojos (IR):** Uso limitado a **distancias muy cortas**. No atraviesa objetos, requiere **línea de visión**. **Ventaja:** ofrece seguridad avanzada.

**- RFID (Identificación por radiofrecuencia):** Usa diversas tecnologías de radio. **RFID activo:** necesita fuente de energía interna. **RFID pasivo:** no requiere energía interna.

**- Bluetooth:** Usa radio de microondas para intercambiar datos. Transmite con **muy baja potencia**. Cambia frecuencias regularmente (para mejorar seguridad y fiabilidad).

**- Óptica de espacio libre (FSO):** Usa **láseres** para la comunicación inalámbrica entre computadoras.

### Comparación de medios de transmisión  
(Escala: 1 = peor, 3 = mejor)

| Medio de transmisión | Velocidad | Fiabilidad | Costo | Seguridad |
|-----------------------|-----------|------------|-------|-----------|
| Conductor metálico    | 2         | 2          | 2     | 2         |
| Fibra óptica          | 3         | 3          | 3     | 3         |
| Inalámbrico           | 1         | 1          | 1     | 1         |


## 3.1.11. Conmutación de paquetes

Un **paquete de datos** es una unidad de información en una forma adecuada para viajar entre computadoras. En una **red de conmutación de paquetes**, el **datagrama** es la unidad básica de transferencia y, en ocasiones, se utiliza en lugar del término paquete de datos (un análisis detallado de las diferencias entre ambos queda fuera del alcance de este texto).

La **conmutación de paquetes** es un método de comunicación usado en redes digitales de computadoras, en el cual los datos se agrupan en **paquetes**.

- El archivo original se divide en paquetes antes de la transmisión.
- Cada paquete puede seguir un camino distinto hacia el destino.
- Cada paquete se envía de manera individual y puede llegar a través de rutas diferentes.

Este método permite que el canal de comunicación se use de forma más eficiente y que se **minimicen los retrasos**.

#### Tipos de conmutación de paquetes:

**- Conmutación de paquetes por datagramas:** Cada paquete contiene la dirección del receptor. Los datagramas entre la misma fuente y destino pueden seguir caminos distintos.
**- Conmutación de paquetes por circuito virtual:** Se establece una ruta entre origen y destino antes de que tenga lugar la transmisión.
