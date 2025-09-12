<h1 align="center">4.1. Lenguaje procedimental
<div align="center">

</div>

## Contenido:

- [4.1.1. Procedimiento para la resolución de problemas](#411-procedimiento-para-la-resolución-de-problemas)
- [4.1.2. Orden de actividades y resultados](#412-orden-de-actividades-y-resultados)
- [4.1.3. Subprocesos en la resolución de problemas](#413-subprocesos-en-la-resolución-de-problemas)

---

## 4.1.1. Procedimiento para la resolución de problemas

Cuando se tiene que resolver un problema concreto, se debe identificar un **método o procedimiento eficaz**.
Este procedimiento reduce la solución a una serie de **pasos simples**.

Estos pasos deben seguirse en el orden correcto para obtener el resultado deseado.

Por ejemplo:

- Es imposible conducir una **motocicleta** si no sabes montar en **bicicleta**.
- Primero debes aprender a montar en bicicleta y, después, podrás conducir la motocicleta.

## 4.1.2. Orden de actividades y resultados

Una empresa desea desarrollar un nuevo **sistema de información**.
La fase de análisis será la que la empresa debe completar antes de pasar a las siguientes etapas del proyecto.

Si la empresa intenta implementar el nuevo sistema sin antes analizar el **dominio del problema**, entonces casi con total seguridad se producirá un **desperdicio total de dinero, esfuerzo y recursos**.

## 4.1.3. Subprocesos en la resolución de problemas

Un buen enfoque para enfrentar un **problema complejo** es desarrollar un método para **dividirlo en subproblemas más pequeños**.
Este método es muy eficaz y eficiente porque es mucho más sencillo abordar varios subproblemas que un único problema complejo.

Los subproblemas resultantes pueden dividirse aún más en otros más pequeños hasta que finalmente puedan ser tratados de manera **individual**.

Esta estrategia se denomina con frecuencia **diseño descendente (top–down design)** o **refinamiento paso a paso (stepwise refinement)**.

El mismo enfoque puede aplicarse al desarrollo de **programas informáticos complejos**.
Mediante el **diseño descendente de programas**, el problema complejo se descompone y para cada subproblema se desarrolla un **subprocedimiento adecuado**.

Un **subprocedimiento** contiene una serie de instrucciones que realizan una tarea.
Cuando un subprocedimiento es llamado, se ejecutan todas las sentencias incluidas en él.

Todos los subprocedimientos que representan diferentes partes de la solución del problema pueden usarse en el momento adecuado mediante sus **identificadores**.

De este modo, el procedimiento se divide en una serie de subprocedimientos; este proceso se conoce como **programación modular**.

Un **identificador** es el nombre que utiliza el programador para identificar de forma única una variable, un objeto, un subprocedimiento, etc.

Ejemplo: 

Supongamos un programa que calcula las soluciones de una **ecuación cuadrática**.
Un **subprocedimiento** llamado Discriminante podría usarse para calcular el discriminante **D**.

'''
Entrada: a, b, c
Llamar al subprocedimiento Discriminante que devuelve el valor D

Si D > 0 entonces
    Calcular x1 = (-b + √D) / (2a)
    Calcular x2 = (-b - √D) / (2a)
Sino, si D = 0 entonces
    Calcular x1 = -b / (2a)
    Calcular x2 = -b / (2a)
Sino
    Salida: "No hay soluciones reales"
Fin Si

Salida: x1, x2

--------------------------------------
Subprocedimiento Discriminante:
    Calcular D = b² - 4 * a * c
    Retornar D
'''
