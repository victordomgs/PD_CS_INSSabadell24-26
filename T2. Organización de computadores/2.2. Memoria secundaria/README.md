<h1 align="center">2.2. Memoria secundaria
<div align="center">

</div>

## Contenido:

- [2.2.1. Identifique la necesidad de contar con almacenamiento persistente](#221-identifique-la-necesidad-de-contar-con-almacenamiento-persistente)

---

<br>

## 2.2.1. Identifique la necesidad de contar con almacenamiento persistente

### Almacenamiento interno

#### Hard disk drive (HDD) y solid state drive (SSD)

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2011.%20Interior%20de%20una%20HDD%20y%20una%20SSD.png" alt="HDD y SSD" width="750" height="auto"/>
    <p><em>Figura 11: Interior de una HDD y una SSD. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Las **unidades de disco duro (HDD)** y las **unidades de estado sólido (SSD)** son las soluciones de almacenamiento más habituales en los ordenadores personales. Los HDD son una tecnología más antigua, pero todavía se utilizan con frecuencia, especialmente en dispositivos no portátiles, ya que resultan relativamente baratos en comparación con la capacidad de almacenamiento que ofrecen. Los HDD utilizan un disco magnético giratorio para leer y escribir datos. Son adecuados para almacenar grandes volúmenes de información, como archivos multimedia, copias de seguridad y documentos, en los que la velocidad no es un factor tan crítico.

Los SSD no tienen partes móviles. Utilizan memoria flash para almacenar datos, lo que proporciona un acceso de alta velocidad y mayor durabilidad. Esto los hace muy populares en dispositivos portátiles como portátiles y tabletas. Son ideales para sistemas operativos, aplicaciones de software y videojuegos debido a su alta velocidad de lectura y escritura, lo que mejora el rendimiento general del sistema.

| Característica       | HDD (disco duro)                                       | SSD (unidad de estado sólido)                  |
|-----------------------|-------------------------------------------------------|-----------------------------------------------|
| Tecnología de almacenamiento | Almacenamiento magnético con discos giratorios y cabezales de lectura/escritura | Memoria flash sin partes móviles               |
| Velocidad             | Velocidades de lectura/escritura más lentas (generalmente 50–150 MB/s) | Velocidades de lectura/escritura más rápidas (generalmente 200–500 MB/s) |
| Durabilidad           | Más propenso a daños físicos debido a las partes móviles | Más duradero; resistente a golpes físicos      |
| Ruido                 | Produce ruido debido a las partes móviles              | Funcionamiento silencioso                      |
| Consumo de energía    | Mayor consumo de energía debido a las partes mecánicas | Menor consumo de energía                       |
| Coste                 | Generalmente más barato por GB                         | Más caro por GB                                |
| Capacidad             | Disponible en mayores capacidades (hasta varios TB)   | Generalmente disponible en capacidades menores (hasta varios TB, pero a mayor coste) |
| Peso                  | Más pesado debido a los componentes mecánicos         | Más ligero                                     |
| Generación de calor   | Genera más calor debido a las partes móviles           | Genera menos calor                             |

Existe otra forma de unidad SSD que actualmente es muy popular y ofrece varias ventajas. Los SSD M.2 tienen el aspecto de una barra de chicle. Son muy pequeños y delgados, y ocupan mucho menos espacio que un SSD estándar. Los **SSD M.2 NVMe** también son más rápidos que los SSD SATA de 2,5” y se consideran más fáciles de instalar: simplemente se insertan en la placa base y se fijan con un solo tornillo.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2012.%20M2%20SSD.png" alt="M2 SSD" width="550" height="auto"/>
    <p><em>Figura 12: M.2 SSD. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

#### eMMC (Embedded MultiMediaCard)

En dispositivos de bajo coste, como teléfonos inteligentes de gama básica y portátiles económicos, donde no son esenciales todas las ventajas de los SSD, las eMMC son una opción popular. También son un tipo de almacenamiento flash que utiliza memoria flash NAND. Están soldadas directamente a la placa base del dispositivo. Aunque su capacidad y velocidad no igualan a las de un SSD estándar, su rendimiento es adecuado para las necesidades informáticas básicas y aplicaciones sencillas.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2013.%20eMMC.jpg" alt="M2 SSD" width="250" height="auto"/>
    <p><em>Figura 13: eMMC. Fuente: Kingston</em></p>
  </div>

### Almacenamiento externo

#### Hard disk drive (HDD) y solid state drive (SSD)

Como soluciones de almacenamiento externo, tanto los HDD como los SSD son opciones populares. Su rendimiento y comparación son idénticos a los de las versiones internas. El uso de uno u otro depende de los requisitos del usuario. Si necesitas transferencias rápidas de archivos, copias de seguridad y una solución portátil que sea menos propensa a sufrir daños al transportarse, los SSD son la mejor elección. Si lo que necesitas son copias de seguridad extensas, almacenar archivos multimedia o transportar archivos grandes, pero la velocidad no es tan crítica, puedes optar por un HDD como mejor alternativa.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2014.%20HDD%20externo.jpg" alt="HDD externo" width="350" height="auto"/>
    <p><em>Figura 14: HDD externo. Fuente: La Vanguardia</em></p>
  </div>

#### Discos ópticos y unidades ópticas

De izquierda a derecha: CD, DVD y Blu-Ray

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2015.%20CD%2C%20DVD%20y%20Blu-Ray.png" alt="Discos ópticos" width="550" height="auto"/>
    <p><em>Figura 15: De izquierda a derecha: CD, DVD y Blu-Ray. Fuente: Computer Science for the IB Diploma 2025 (Baumgarten P.)</em></p>
  </div>

Las unidades ópticas que leen/escriben discos ópticos, como los CD, DVD o Blu-Ray, están perdiendo popularidad, pero todavía se consideran una opción para el almacenamiento externo de datos. El coste de un disco óptico es bajo en comparación con un HDD o un SSD y, aunque sus velocidades de lectura/escritura pueden ser más lentas, son suficientes para el archivado de datos y la reproducción. Sin embargo, los discos son propensos a rayarse, especialmente si no se almacenan correctamente, y requieren una unidad óptica para leerlos o grabarlos, algo cada vez menos común en los dispositivos actuales.

#### Tarjetas de memoria

Las tarjetas de memoria son dispositivos de almacenamiento compactos que se utilizan con frecuencia en cámaras, teléfonos inteligentes y otros dispositivos portátiles. Son ideales para ampliar la capacidad de almacenamiento en dispositivos móviles y para guardar fotos y vídeos en cámaras, ya que utilizan memoria flash NAND. Existen en múltiples formatos, como SD, microSD y CompactFlash, adaptándose a diferentes dispositivos y necesidades de espacio. Se caracterizan por su durabilidad: son resistentes a golpes físicos, temperaturas extremas y al agua, lo que las hace perfectas para dispositivos portátiles. Sus tiempos de lectura/escritura suelen ser más lentos que los de los SSD, pero superan a los de los discos ópticos.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2016.%20Tarjetas%20de%20memoria.jpg" alt="HDD externo" width="350" height="auto"/>
    <p><em>Figura 16: Tarjetas de memoria. Fuente: JetComputer</em></p>
  </div>

#### Network Attached Storage (NAS)

El NAS es un sistema de almacenamiento de archivos dedicado, conectado a una red, que permite a múltiples usuarios acceder a los datos. Se utiliza a menudo en hogares o empresas para centralizar el almacenamiento de datos, el guardado de archivos y las copias de seguridad.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell25-27/blob/main/A1.%20Fundamentos%20de%20la%20inform%C3%A1tica/images/Figura%2017.%20NAS.jpg" alt="HDD externo" width="450" height="auto"/>
    <p><em>Figura 17: NAS. Fuente: MuyComputer</em></p>
  </div>

Un NAS normalmente está compuesto por múltiples HDD o SSD configurados en **RAID (Redundant Array of Independent Disks, Conjunto Redundante de Discos Independientes)**. Suele conectarse a la red mediante Ethernet y ejecuta un sistema operativo ligero diseñado para el almacenamiento, la gestión y el intercambio de archivos.

Al utilizar múltiples HDD o SSD, su capacidad suele ser alta, y es posible ampliar el sistema añadiendo más unidades.

> [!NOTE]  
> **RAID (Redundant Array of Independent Disks):** es una tecnología de almacenamiento de datos que combina múltiples discos físicos en una única unidad lógica para mejorar el rendimiento, proporcionar redundancia y garantizar la protección de los datos.
