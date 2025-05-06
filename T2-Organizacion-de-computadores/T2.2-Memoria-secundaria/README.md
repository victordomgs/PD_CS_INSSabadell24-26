<h1 align="center">Memoria secundaria
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>

</div>

## Contenido:

[1. Introducción a la memoria](#1-introducción-a-la-memoria)  

[2. Memoria: especificaciones físicas](#2-memoria-especificaciones-físicas)  
  - [2.1. Características principales](#21-características-principales)
  - [2.2. Tipos de memorias](#22-tipos-de-memorias)  
    - [2.2.1. Memorias volátiles (RAM - Random Access Memory)](#221-memorias-volátiles-ram---random-access-memory)  
    - [2.2.2. Memorias no volátiles](#222-memorias-no-volátiles)  
    - [2.2.3. Memoria Caché](#223-memoria-caché)  
    - [2.2.4. Memoria Virtual](#224-memoria-virtual)

[3. Memoria secundaria](#3-memoria-secundaria)  
  - [3.1. Características principales](#31-características-principales)  
  - [3.2. Tipos de memoria secundaria](#32-tipos-de-memoria-secundaria)  
  - [3.3. Importancia en los sistemas informáticos](#33-importancia-en-los-sistemas-informáticos)  
  - [3.4. Evolución tecnológica](#34-evolución-tecnológica)  
  - [3.5. Comparación entre tipos de almacenamiento](#35-comparación-entre-tipos-de-almacenamiento)  

# 1. Introducción a la memoria

La memoria de un sistema informático se define como el medio físico capaz de almacenar la información de forma temporal o permanente. Esta información puede ser leída o escrita segun las características de cada tipo de memoria. 

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/T2-Organizacion-de-computadores/T2.2-Memoria-secundaria/images/cpumemoria.png" alt="Relación CPU i memoria" width="600" height="auto"/>
    <p><em>Figura 1: Relación CPU i memoria. Fuente: Abacus</em></p>
  </div>
  
# 2. Memoria: especificaciones físicas

## 2.1. Características principales
Las características principales de la memoria estan determinadas por los siguientes factores: 

#### Duración de la información

- **Memorias volátiles:** la información se mantiene solo mientras hay subministramiento eléctrico (por ejemplo, la RAM).
- **Memorias no volátiles:** la información persiste después de apagar el equipo (por ejemplo, la ROM o las memorias flash).
- **Memorias permanentes:** no pueden ser modificadas una vez grabadas (por ejemplo, algunas ROM de fábrica).
- **Memorias con refresco:** necesitan una operación periódica para evitar la pérdida de datos (por ejemplo, DRAM).

#### Capacidad de almacenamiento

Determinada por el número de posiciones de almacenamiento y la canditat de bits por posición. 

Expresada en bytes (B), kilbytes (KB), megabytes (MB), gigabytes (GB), etc. 

| Amplada       | Nom              |
|---------------|------------------|
| 1 bit         | (b)              |
| 4 bits        | nibble           |
| 8 bits        | byte (B)         |
| 16 bits       | paraula          |
| 32 bits       | doble paraula    |

| Unitat | Equivalència                         |
|--------|--------------------------------------|
| 1K     | Kilo = 2¹⁰ = 1024                    |
| 1M     | Mega = 2²⁰ = 1024 K                  |
| 1G     | Giga = 2³⁰ = 1024 M                  |
| 1T     | Tera = 2⁴⁰ = 1024 G                  |
| 1P     | Peta = 2⁵⁰ = 1024 T                  |

#### Velocidad

- **Tiempo de acceso (TA)**: Tiempo necesario para leer o escribir un dato en una posición determinada.
- **Tiempo de ciclo (TC)**: Tiempo mínimo entre dos operaciones sucesivas sobre la memoria.
- **Frecuencia de acceso (FA)**: Número de lecturas/escrituras que se pueden realizar por unidad de tiempo.

#### Unidad de transferencia

- **Acceso por palabra**: Se transfiere una única palabra de memoria por operación.
- **Acceso por bloque**: Se transfiere un conjunto de palabras de memoria.

#### Modo de acceso

- **Acceso aleatorio**: Se puede acceder directamente a cualquier posición de memoria (por ejemplo, la RAM).
- **Acceso secuencial**: Es necesario recorrer la memoria en orden hasta llegar a la posición deseada (por ejemplo, cintas magnéticas).
- **Acceso directo**: Primero se localiza el bloque de datos y luego se busca dentro del bloque (por ejemplo, discos duros).
- **Acceso asociativo**: Se busca la información por contenido y no por dirección (por ejemplo, memorias caché tipo CAM).

## 2.2. Tipos de memorias

Según su tecnología y funcionamiento, podemos clasificar las memorias de la siguiente manera:

### 2.2.1. Memorias volátiles (RAM - Random Access Memory)

Las memorias RAM son de lectura y escritura y se utilizan como memoria principal de los ordenadores. Hay dos tipos principales:

- **DRAM (Dynamic RAM)**: Necesita refresco periódico para mantener la información.
- **SRAM (Static RAM)**: No necesita refresco, es más rápida pero más cara y con menor capacidad.

### 2.2.2. Memorias no volátiles

Estas memorias conservan la información sin necesidad de suministro eléctrico. Ejemplos:

- **ROM (Read Only Memory)**: Solo se puede leer. Incluye subtipos como PROM, EPROM y EEPROM.
- **Memoria Flash**: Variante de la EEPROM, más rápida y duradera.
- **NVRAM (Non-Volatile RAM)**: Combinación de SRAM con EEPROM.

### 2.2.3. Memoria Caché

Es una memoria SRAM de alta velocidad situada entre la CPU y la RAM para reducir los tiempos de acceso a los datos más utilizados.

### 2.2.4. Memoria Virtual

Es una técnica que permite simular más memoria RAM utilizando espacio en disco, gestionada por el sistema operativo.

## 3. Memoria secundaria

La memoria secundaria, también conocida como almacenamiento masivo, cumple una función vital en los sistemas informáticos: el almacenamiento permanente de datos. A diferencia de la memoria principal (RAM), los datos no se pierden cuando el sistema se apaga. Esta memoria es más lenta, pero ofrece una gran capacidad de almacenamiento a un coste relativamente bajo.

### 3.1. Características principales

- **Capacidad**: Las memorias secundarias pueden alcanzar capacidades de varios terabytes (TB), lo que las hace adecuadas para almacenar grandes volúmenes de datos como bases de datos, vídeos, copias de seguridad, etc.
- **Persistencia**: Una de sus principales ventajas es la retención de datos sin necesidad de energía eléctrica. Esto es fundamental para la integridad y conservación de la información.
- **Velocidad**: Aunque son más lentas que la memoria RAM, las tecnologías actuales como las SSD han reducido esta brecha significativamente.
- **Costo**: Su precio por gigabyte es considerablemente más bajo que el de la memoria principal, lo que las hace idóneas para almacenamiento a largo plazo.

### 3.2. Tipos de memoria secundaria

- **Discos duros (HDD)**: Utilizan platos magnéticos giratorios y cabezales de lectura/escritura. Son ideales para almacenamiento masivo a bajo costo. Sin embargo, presentan mayor latencia debido a las partes mecánicas.
- **Unidades de estado sólido (SSD)**: Basadas en memoria flash, ofrecen velocidades de lectura y escritura muy superiores a los HDD. No tienen partes móviles, lo que reduce su desgaste y mejora su resistencia a impactos.
- **Memorias USB (pendrives)**: Utilizadas habitualmente para transferencias rápidas de datos entre dispositivos. Aunque su velocidad puede ser limitada, destacan por su portabilidad y facilidad de uso.
- **Tarjetas de memoria**: Comunes en cámaras digitales, teléfonos y dispositivos portátiles. Utilizan también tecnología flash y presentan diversas capacidades y velocidades.
- **Cintas magnéticas**: Aunque han caído en desuso en el ámbito doméstico, siguen siendo una solución viable para almacenamiento masivo a largo plazo en entornos empresariales, especialmente para copias de seguridad.

### 3.3. Importancia en los sistemas informáticos

La memoria secundaria es esencial en múltiples aspectos del funcionamiento de un sistema informático:

- Almacena el sistema operativo, que se carga en la memoria principal al arrancar.
- Guarda las aplicaciones y los archivos del usuario.
- Permite realizar copias de seguridad para evitar la pérdida de información crítica.
- Facilita la gestión de grandes volúmenes de datos de forma estructurada (por ejemplo, en servidores y bases de datos).

### 3.4. Evolución tecnológica

La evolución de la memoria secundaria ha sido constante, con mejoras notables en capacidad, velocidad y fiabilidad:

- De los antiguos disquetes a los actuales discos duros y SSD.
- Disminución del tamaño físico con aumento de capacidad (por ejemplo, microSD de 1 TB).
- Avances como NVMe y PCIe han incrementado significativamente la velocidad de acceso en los SSD modernos.
- Aparición del almacenamiento en la nube como forma de memoria secundaria accesible remotamente.

### 3.5. Comparación entre tipos de almacenamiento

| Tipo             | Capacidad típica | Velocidad      | Precio por GB | Durabilidad | Portabilidad |
|------------------|------------------|----------------|---------------|-------------|--------------|
| HDD              | 500 GB – 16 TB   | Media          | Bajo          | Moderada    | Baja         |
| SSD (SATA/NVMe)  | 120 GB – 8 TB    | Alta           | Medio         | Alta        | Media        |
| USB              | 8 GB – 2 TB      | Variable       | Medio         | Alta        | Alta         |
| Tarjeta de memoria | 4 GB – 1 TB     | Variable       | Medio         | Alta        | Alta         |
| Cinta magnética  | Hasta 30 TB      | Muy baja       | Muy bajo      | Alta        | Baja         |

Cada tipo de memoria secundaria tiene su contexto de uso ideal, por lo que es habitual encontrar varios tipos coexistiendo en un mismo entorno informático.
