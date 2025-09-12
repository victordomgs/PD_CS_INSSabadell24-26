<h1 align="center">4.1. Pensamiento lógico
<div align="center">

</div>

## Contenido:

- [4.1.4. Toma de decisiones](#414-toma-de-decisiones)
- [4.1.5. Decisión requerida para problema concreto](#415-decisión-requerida-para-problema-conreto)
- [4.1.6. Condición asociada a una decisión concreta a un problema](#416-condición-asociada-a-una-decisión-concreta-a-un-problema)
- [4.1.7. Relación entre decisión y condición](#417-relación-entre-decisión-y-condición)
- [4.1.8. Reglas lógicas para decisiones reales](#418-reglas-lógicas-para-decisiones-reales)

---

## 4.1.4. Toma de decisiones

### Suma simple

El proceso de suma no requiere tomar ninguna decisión. El algoritmo es directo:

```
Entrada: A
Entrada: B
C = A + B
Salida: C
```

### Problema decisional

Algunos problemas requieren decisiones.

Imagina un cruce peatonal con semáforo:

- Si la luz está **verde**, entonces **es seguro cruzar** → el peatón **cruza**.
- Si la luz está **roja**, entonces el peatón debe **detenerse y esperar**.

```
If Light is green
Then
Set pedestrian = PASS
Else
Set pedestrian = WAIT
End If
```

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2020.%20Redes.png" alt="Conditional operation" width="550" height="auto"/>
    <p><em>Figura 20: Operación condicional. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

## 4.1.5. Decisión requerida para problema concreto

En la vida cotidiana, las personas están constantemente **identificando las decisiones necesarias** y las diferentes **acciones relevantes** para un problema o una situación.

Es evidente que **tomamos diferentes acciones según las condiciones que prevalezcan**.

### Ejemplo: Ir a un partido de fútbol

Un estudiante puede ir al partido de fútbol **si se cumplen las dos condiciones**:

- Haber hecho los deberes (**Homework done**)
- Que el clima sea bueno (**Weather is good**)

| Homework done | Weather is good | Allowed |
|---------------|-----------------|---------|
| TRUE          | TRUE            | TRUE    |
| TRUE          | FALSE           | FALSE   |
| FALSE         | TRUE            | FALSE   |
| FALSE         | FALSE           | FALSE   |

```
Boolean Homework_done
Boolean Weather_is_good
Boolean Allowed

Input Homework_done
Input Weather_is_good

If Homework_done AND Weather_is_good Then
    Allowed = True
Else
    Allowed = False
End If
```


## 4.1.6. Condición asociada a una decisión concreta a un problema

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2021.%20Redes.png" alt="The loop while" width="550" height="auto"/>
    <p><em>Figura 21: The loop while. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

> [!TIP]
> **WHILE loop:** Ejecuta las instrucciones mientras la condición sea verdadera. En cuanto la condición se evalúa como falsa, el bucle termina y no se ejecuta el cuerpo.
> **FROM/TO loop (también conocido como FOR loop):** Ejecuta las instrucciones un número determinado de veces, según los valores inicial y final. El bucle termina cuando la condición se evalúa como falsa, es decir, cuando se alcanza o supera el límite indicado.

La **iteración** es el proceso de repetir una serie de instrucciones. Es extremadamente útil en la programación y se utiliza para repetir una sentencia o un bloque de sentencias dentro de un algoritmo.

La iteración se expresa usando las sentencias “**from to loop**” y “**while loop**”.

La notación aprobada por el **IB** para desarrollar pseudocódigo incluye los siguientes diagramas de flujo y pseudocódigo para representar estas sentencias.

La figura en forma de **rombo** realiza una prueba booleana, evalúa una expresión y devuelve un valor booleano (**true o false**).

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2022.%20Redes.png" alt="The from to loop" width="550" height="auto"/>
    <p><em>Figura 22: The from to loop (IB notation). Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

La notación aprobada por el **IB** para desarrollar pseudocódigo no incluye el siguiente **símbolo de diagrama de flujo**, aunque está ampliamente aceptado.

  <div style="text-align: center;">
    <img src="https://github.com/victordomgs/PD_CS_INSSabadell24-26/blob/main/images/Figura%2023.%20Redes.png" alt="The from to loop" width="550" height="auto"/>
    <p><em>Figura 23: The from to loop. Fuente: Core Computer Science (Kostas Dimitriou & Markos Hatzitaskos)</em></p>
  </div>

#### Ejemplo: loop while
```
//use of while loop
//to print a message
//user selects the number of times
I = O
X = input("How many times do you want to see the message")
loop while I < x
I=I+1
output ("it will be printed (number entered) times")
end while
```

#### Ejemplo: loop from to
```
//use of from to loop
//to print a message
//user selects the number of times
I = 0
X = input-.("How many times do you want to see the message")
loop I from 1 to X
output ("it will be printed (number entered) times")
and loop
```

## 4.1.7. Relación entre decisión y condición

## 4.1.8. Reglas lógicas para decisiones reales



