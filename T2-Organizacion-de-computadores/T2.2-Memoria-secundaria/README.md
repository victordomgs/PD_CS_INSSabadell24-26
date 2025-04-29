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

# 1. Introducción a la memoria

La memoria de yun sistema informático se define como el medio físico capaz de almacenar la información de forma temporal o permanente. Esta información puede ser leída o escrita segun las características de cada tipo de memoria. 

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
