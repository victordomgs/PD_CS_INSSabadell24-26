# Actividad 6: División Binaria

## Pasos para la División Binaria

1. Escribe el dividendo y el divisor en binario.
2. Comienza dividiendo las cifras de mayor valor, de izquierda a derecha, comprobando si el divisor cabe en esa parte del dividendo.
3. Si el divisor "cabe", escribe un 1 en el cociente y resta el divisor de esa sección del dividendo.
4. Si el divisor "no cabe", escribe un 0 en el cociente y baja la siguiente cifra.
5. Repite el proceso hasta completar la división, identificando el cociente y el residuo final.

## Ejemplo

Dividir el número binario **1101** entre **10**.

  1101 ÷ 10
  	    110
	--------
 	10 | 1101
	     - 10
	--------
 	      100
 	     - 10      	
	--------
 	       01

**Explicación paso a paso**:

1. Tomamos los dos primeros dígitos de **1101** (11), como 11 es mayor o igual a 10, dividimos:
   - **11 ÷ 10** da un cociente de **1** y un residuo de **1**.
2. Bajamos el siguiente dígito del dividendo para formar **100**.
3. **100 ÷ 10** da un cociente de **1** y un residuo de **0**.
4. Bajamos el último dígito, obteniendo **01**, que es menor que 10, así que este es el residuo final.

## Ejercicios

Realiza las siguientes divisiones en binario, indicando el cociente y el residuo:

1. 1011 ÷ 10
2. 1110 ÷ 11
3. 11001 ÷ 101
4. 10010 ÷ 110
5. 11101 ÷ 100
6. 101101 ÷ 111
7. 110111 ÷ 101
8. 100111 ÷ 11
9. 111111 ÷ 110
10. 1010 ÷ 10
