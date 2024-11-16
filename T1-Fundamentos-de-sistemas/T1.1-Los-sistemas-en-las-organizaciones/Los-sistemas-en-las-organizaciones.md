<h1 align="center">Los sistemas en las organizaciones 
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
<a href="https://www.linkedin.com/in/v%C3%ADctor-garc%C3%ADa-saiz-/"><img src="https://img.shields.io/badge/LinkedIn-Perfil-%230077B5" alt="Perfil de LinkedIn"/></a>
</a>



</div>

### Contenido:
[1.1. Los sistemas en las organizaciones](#11-los-sistemas-en-las-organizaciones)
  - [1.1.1. Planificación e instalación de sistemas](#111-planificación-e-instalación-de-sistemas)
    - [1.1.1.1. Identificación del contexto para la planificación de un nuevo sistema](#1111-identificación-del-contexto-para-la-planificación-de-un-nuevo-sistema)
    - [1.1.1.2. La necesidad de la gestión de cambios](#1112-la-necesidad-de-la-gestión-de-cambios)
    - [1.1.1.3. Problemas de compatibilidad en sistemas heredados y fusiones de negocios](#1113-problemas-de-compatibilidad-en-sistemas-heredados-y-fusiones-de-negocios)
    - [1.1.1.4. Comparación entre hardware cliente y alojamiento remoto](#1114-comparación-entre-hardware-cliente-y-alojamiento-remoto)
    - [1.1.1.5. Evaluación de procesos alternativos de instalación](#1115-evaluación-de-procesos-alternativos-de-instalación)
  - [1.1.2. Migración de datos](#12-migración-de-datos)
    - [1.1.2.1. Problemas comunes en la migración de datos](#121-problemas-comunes-en-la-migración-de-datos)
  - [1.1.3. Pruebas de sistemas](#13-pruebas-de-sistemas)
    - [1.1.3.1. Importancia de las pruebas en la implementación](#131-importancia-de-las-pruebas-en-la-implementación)
    - [1.1.3.2. Tipos de pruebas](#132-tipos-de-pruebas)
      - [1.1.3.2.1. Validación de datos introducidos por el usuario](#1321-validación-de-datos-introducidos-por-el-usuario)
      - [1.1.3.2.2. Depuración](#1322-depuración)
      - [1.1.3.2.3. Pruebas beta](#1323-pruebas-beta)
  - [1.1.4. Pensar en el usuario](#14-pensar-en-el-usuario)
    - [1.1.4.1. Importancia de la documentación para el usuario](#141-importancia-de-la-documentación-para-el-usuario)
    - [1.1.4.2. Métodos para ofrecer documentación](#142-métodos-para-ofrecer-documentación)
    - [1.1.4.3. Métodos para ofrecer capacitación](#143-métodos-para-ofrecer-capacitación)
  - [1.1.5. Copia de seguridad del sistema](#15-copia-de-seguridad-del-sistema)
    - [1.1.5.1. Causas de pérdida de datos](#151-causas-de-pérdida-de-datos)
    - [1.1.5.2. Consecuencias de la pérdida de datos en contextos específicos](#152-consecuencias-de-la-pérdida-de-datos-en-contextos-específicos)
    - [1.1.5.3. Métodos para prevenir la pérdida de datos](#153-métodos-para-prevenir-la-pérdida-de-datos)
  - [1.1.6. Implementación de software](#16-implementación-de-software)
    - [1.1.6.1. Estrategias para la gestión de versiones y actualizaciones](#161-estrategias-para-la-gestión-de-versiones-y-actualizaciones)

<br>

### 1.1.1. Planificación e instalación de sistemas

La planificación e instalación de sistemas es una etapa fundamental para garantizar que un sistema informático cumpla con las necesidades de una organización. Esta sección aborda los pasos necesarios para planificar adecuadamente y los desafíos asociados con la instalación de sistemas en diferentes contextos organizacionales.

#### 1.1.1.1. Identificación del contexto para la planificación de un nuevo sistema
La planificación de un nuevo sistema de información es un proceso crítico que requiere un análisis exhaustivo del contexto organizacional. Este análisis debe considerar diversos factores que aseguren la alineación del sistema con los objetivos y necesidades de la organización. A continuación, se detallan los aspectos clave a evaluar:

<ins>**Alcance y limitaciones del sistema**</ins>

Es esencial determinar qué procesos y funciones cubrirá el nuevo sistema. Esto implica identificar las áreas operativas que se beneficiarán del sistema y establecer los límites de su aplicación. Una definición clara del alcance ayuda a evitar desviaciones y garantiza que el sistema cumpla con las expectativas establecidas.

Reconocer las restricciones técnicas, financieras y temporales que puedan afectar la implementación del sistema. Estas limitaciones pueden influir en la selección de tecnologías, en la escala del proyecto y en los plazos de entrega.

Se puede decir que la gestió del alcance del proyecto cumple co ua serie de pasos necesarios: 
1. Determinar los **objetivos del proyecto**.
2. Definir **metas concretas** para alcanzar estos objetivos.
3. Planificar las **fases** que necesitamos para ir alcanzando esas metas.
4. Identificar las **actividades** que necesitamos en cada fase.
5. Relacionar las actividades en la **planificación**, creando dependencias entre ellas. Por ejemplo, no podemos empezar una actividad hasta que no termine otra.

> [!NOTE]
> **Nombre del proyecto:** Prototipo de librería electrónica.
> 
> **Definición del proyecto:**
> 
> - **Objetivo:** El objetivo del proyecto es realizar un prototipo de un sistema de venta de libros electrónicos vía Internet que pueda ser utilizado a través de cualquier navegador web, utilizando la metodología orientada a objetos.
> 
> - **Alcance:** El proyecto va a incluir desde la planificación y programación del proyecto pasando por las diferentes etapas del proceso de desarrollo, ya sea elicitación y especificación de requerimientos, así como el análisis y diseñoi hasta la creación de un prototipo finalizando con el desarrollo de un modelo de pruebas, un plan de implantación y la prueba del mismo.
> 
> - **Límites:** El proyecto no incluirá el desarrollo exhaustivo del producto. Tampoco se incluirá la documentación que da respaldo a desarrollo del producto, como por ejemplo los manuales de usuario.

<ins>**Roles de usuarios**</ins>

Comprender las necesidades y expectativas de los diferentes usuarios dentro de la organización es fundamental. Esto incluye identificar quiénes interactuarán con el sistema, sus competencias tecnológicas y cómo el sistema impactará en sus tareas diarias.

**Clasificación de roles**

Los usuarios pueden clasificarse en diversas categorías, tales como:

- **Usuarios finales:** Empleados que utilizarán el sistema para realizar sus funciones diarias.
- **Administradores del sistema:** Responsables de la configuración, mantenimiento y seguridad del sistema.
- **Desarrolladores y técnicos de soporte:** Encargados de la implementación, actualización y resolución de problemas técnicos.

**Gestión del cambio**

Es vital considerar cómo la introducción del nuevo sistema afectará a los usuarios y planificar estrategias de capacitación y soporte para facilitar la transición.

  <div style="text-align: center;">
  <img src="https://www.iberdrola.com/documents/20125/40504/gestion_ESP.jpg" alt="XT color" width="497" height="586"/>
  <p><em>Figura 1: La gestión del cambio en una organización.. Fuente: <a href="https://www.iberdrola.com/talento/que-es-gestion-del-cambio">Iberdrola</a></em></p>
  </div>

#### 1.1.1.2. La necesidad de la gestión de cambios
La introducción de un nuevo sistema inevitablemente implica cambios que deben gestionarse cuidadosamente. Los puntos clave incluyen:

- **Factores clave del cambio:** Identificar qué aspectos del sistema o de los flujos de trabajo se verán afectados.
- **Gestión del impacto:** Mitigar los efectos negativos sobre los empleados, asegurando una transición fluida.
- **Comunicación:** Informar a todos los stakeholders sobre el propósito, los beneficios y el impacto del nuevo sistema.
- **Capacitación:** Asegurar que los usuarios finales tengan el conocimiento necesario para usar el sistema de manera efectiva.

#### 1.1.1.3. Problemas de compatibilidad en sistemas heredados y fusiones de negocios
Las organizaciones que integran sistemas existentes o realizan fusiones enfrentan problemas de compatibilidad que pueden incluir:

- **Compatibilidad de software:** Sistemas que no pueden interactuar debido a diferencias en versiones, formatos de datos o estándares.
- **Diferencias culturales y de idioma:** En fusiones internacionales, las diferencias idiomáticas y culturales pueden complicar la integración de sistemas.
- **Costos de actualización:** Migrar o adaptar sistemas heredados puede ser costoso en términos de tiempo y recursos.

#### 1.1.1.4. Comparación entre hardware cliente y alojamiento remoto
Al decidir cómo implementar un sistema, las organizaciones deben elegir entre usar hardware cliente o un alojamiento remoto. Las diferencias clave incluyen:

- **Hardware cliente:**
  - Mayor control sobre los datos y el sistema.
  - Costos iniciales altos debido a la compra e instalación del hardware.
  - Mantenimiento interno y actualización de equipos.
- **Alojamiento remoto:**
  - Uso de soluciones basadas en la nube, como SaaS (Software como servicio).
  - Reducción de costos iniciales, pero mayor dependencia de proveedores externos.
  - Problemas potenciales de latencia y diferencias de zona horaria.

#### 1.1.1.5. Evaluación de procesos alternativos de instalación
Existen diferentes métodos para instalar un nuevo sistema, cada uno con sus ventajas e inconvenientes. Estos métodos incluyen:

- **Ejecución en paralelo:** Operar el sistema antiguo y el nuevo simultáneamente hasta que se confirme el éxito del nuevo sistema.
  - **Ventaja:** Minimiza riesgos.
  - **Desventaja:** Costos más altos debido a la operación dual.
- **Ejecución de prueba:** Implementar el sistema en un entorno controlado antes de lanzarlo por completo.
  - **Ventaja:** Identificación temprana de problemas.
  - **Desventaja:** Puede no replicar todas las condiciones del entorno real.
- **Cambio directo:** Reemplazar el sistema antiguo por el nuevo de manera inmediata.
  - **Ventaja:** Más rápido y menos costoso.
  - **Desventaja:** Mayor riesgo en caso de fallos.
- **Conversión en fases:** Implementar el sistema por etapas o departamentos.
  - **Ventaja:** Permite ajustar problemas a medida que avanza la instalación.
  - **Desventaja:** Puede generar inconsistencias temporales en la operación.
