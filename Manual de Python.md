# **Lenguaje de programacion Python** #

## Estructuras repetitivas ##

## *La sentencia for* ##

La sentencia for en Python difiere un poco de lo que uno puede estar acostumbrado en lenguajes como
C o Pascal. En lugar de siempre iterar sobre una progresión aritmética de números (como en Pascal) o
darle al usuario la posibilidad de definir tanto el paso de la iteración como la condición de fin (como en C),
la sentencia for de Python itera sobre los ítems de cualquier secuencia (una lista o una cadena de
texto), en el orden que aparecen en la secuencia. En cada iteración, el elemento siguiente del iterable se asigna al nombre de variable especificado:

    lista = ["a", "b", "c"]
    for i in lista: # Iteramos sobre una lista, que es iterable
    	print i
    
    a
    b
    c
    
	cadena = "abcdef"
    for i in cadena:  Iteramos sobre una cadena, que también es iterable
		print i,   //añadiendo una coma al final hacemos que no introduzca un salto de línea, sino un espacio
    
    a b c d e f

