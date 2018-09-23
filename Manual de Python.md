# **Lenguaje de programacion Python** #

## Estructuras repetitivas ##

## *La sentencia while* ##

El bucle while evalúa una condición y, si es verdadera, ejecuta el bloque de código interno. Continúa evaluando y ejecutando mientras la condición sea verdadera. Se define con la palabra clave while seguida de la condición, y a continuación el bloque de código interno:

    >>> numero = 0
    >>> while numero < 10:
    ...     print numero,
    ...     numero += 1  #un buen programador modificará las variables de control al finalizar el ciclo while
    ...
    0 1 2 3 4 5 6 7 8 9
