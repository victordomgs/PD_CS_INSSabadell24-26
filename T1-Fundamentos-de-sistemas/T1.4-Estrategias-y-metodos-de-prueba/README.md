<h1 align="center">Estrategias y métodos de prueba
<div align="center">

<a href="https://github.com/victordomgs/Teoria-de-sistemas-i-computacion/blob/main/LICENSE"><img src="https://img.shields.io/github/license/abhisheknaiidu/awesome-github-profile-readme?color=2b9348" alt="License Badge"/></a>
<a href="https://agora.xtec.cat/ies-sabadell/"><img src="https://img.shields.io/badge/Institut%20Sabadell-Centre-%23FFD700" alt="Enllaç a Institut Sabadell"/></a>
</a>



</div>

## Contenido:
[1. Importancia de las pruebas](#1-los-sistemas-de-información)  
  - [1.1. Beneficios de las pruebas](#11-beneficios-de-las-pruebas)
  - [1.2. Pruebas en todas las fases del ciclo de vida](#12-pruebas-en-todas-las-fases-del-ciclo-de-vida)
  - [1.3. Distintos tipos de pruebas de Software](#13-distintos-tipos-de-pruebas-de-software)


<br>

## 1. Importancia de las pruebas
Las pruebas son una fase esencial en cualquier proceso de desarrollo e implementación de sistemas. Su objetivo principal es garantizar que el sistema cumple con los requisitos funcionales y no funcionales, así como detectar y corregir errores antes de que el producto final llegue al usuario. Sin un enfoque adecuado en las pruebas, la calidad del sistema puede verse comprometida, lo que afecta negativamente a la experiencia del usuario y a la productividad de la organización.

### 1.1. Beneficios de las pruebas
1. **Garantía de calidad:**
   - Validan que el sistema funciona según lo esperado.
   - Detecta errores tempranamente, reduciendo costes y tiempos en correcciones posteriores.
2. **Satisfacción del usuario final:**
   - Los usuarios perciben un sistema confiable, funcional y fácil de usar.
   - Un sistema probado reduce incidecias que puedan generar frustración.
3. **Minimización de riesgos:**
   - Evitan fallos críticos en producción que podrían causar interrupciones o pérdidas de datos.
   - Aseguran que el sistema cumple con estándares de seguridad y rendimiento.
4. **Cumplimiento de requisitos:**
   - Verifican que el software implementa correctamente los requisitos definidos por el cliente o la organización.

### 1.2. Pruebas en todas las fases del ciclo de vida
Las pruebas no deben limitarse a una etapa final del desarrollo, sino que deben integrarse en todas las fases del ciclo de vida del sistema. Cada etapa tiene objetivos específicos de pruebas:
1. **Durante el diseño:**
   - Validar que los requerimientos están correctamente especificados.
   - Asegurar que las especificaciones son viables y alineadas con las expectativas del cliente.
2. **Durante el desarrollo:**
   - Identificar y corregir errores en el código (pruebas unitarias).
   - Evaluar la integración entre compoentes (pruebas de integración).
3. **Antes del lanzamiento:**
   - Realizar pruebas funcionales y no funcionales.
   - Simular escenarios reales con usuarios (pruebas beta).
4. **Durante la operación:**
   - Continuar con pruebas de mantenimiento y regresión para garantizar que actualizaciones o cambios no introduzcan errores.

### 1.3. Distintos tipos de pruebas de Software
Hay muchos tipos de técnicas de pruebas de software que puedes utilizar para asegurarte de que los cambios en el código funcionen según lo esperado. Sin embargo, no todas las pruebas son iguales.

#### Pruebas unitarias
Las pruebas unitarias son pruebas de bajo nivel que se enfocan en validar el correcto funcionamiento de métodos, funciones o bloques específicos dentro de las clases, componentes o módulos del software. Estas pruebas se realizan muy cerca de la lógica fuente de la aplicación, asegurando que cada unidad de código cumpla con su propósito de manera independiente.

En términos generales, las pruebas unitarias son económicas de automatizar y se ejecutan rápidamente, lo que las hace ideales para integrarlas en un servidor de integración continua. Esto permite detectar y corregir errores en etapas tempranas del desarrollo, mejorando la eficiencia del proceso.

#### Pruebas de integración
Las pruebas de integración tienen como objetivo verificar que los diferentes módulos o servicios de una aplicación interactúan correctamente entre sí. Por ejemplo, estas pruebas pueden validar que la aplicación se comunica adecuadamente con la base de datos o que los microservicios colaboran de manera efectiva y cumplen con las expectativas del sistema.

A diferencia de las pruebas unitarias, las pruebas de integración suelen ser más costosas de realizar, ya que requieren que múltiples componentes de la aplicación estén operativos al mismo tiempo. Esto implica una mayor preparación del entorno de pruebas y un tiempo de ejecución más prolongado.

#### Pruebas funcionales
Las pruebas funcionales están diseñadas para validar que una aplicación cumple con los requisitos empresariales definidos. Estas pruebas se centran exclusivamente en los resultados de las acciones realizadas, sin analizar los estados intermedios del sistema durante su ejecución.

#### Pruebas de rendimiento
Las pruebas de rendimiento evalúan el rendimiento de un sistema con una carga de trabajo determinada. Ayudan a medir la fiabilidad, la velocidad, la escalabilidad y la capacidad de respuesta de una aplicación. Por ejemplo, una prueba de rendimiento puede analizar los tiempos de respuesta al ejecutar un gran número de solicitudes, o cómo se comporta el sistema con una cantidad significativa de datos.

#### Pruebas beta
Las pruebas beta, del inglés beta testing, son las pruebas de software que se realizan cuando el sistema está teóricamente correcto y pasa a ejecutarse en un entorno real. No importa cuán bueno que sea nuestro proceso de desarrollo, siempre habrá fallos que no han sido descubiertos por los desarrolladores ni por el equipo de pruebas.

---

> [!IMPORTANT]  
> Existen múltiples programas y herramientas diseñados específicamente para realizar pruebas automatizadas sobre otros programas, lo que simplifica el proceso de prueba, reduce errores humanos y disminuye significativamente los costes asociados con la validación y el mantenimiento de software. Estas herramientas permiten ejecutar pruebas repetitivas y detalladas de manera más eficiente que las pruebas manuales.
