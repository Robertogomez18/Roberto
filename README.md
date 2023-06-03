# Roberto
Proyecto III
Algoritmo Calculadora
	
    Dimension matriz1[5, 5]
    Dimension matriz2[5, 5]
    Definir n, m Como Entero
    Definir opcion Como Entero
	
    Limpiar Pantalla
    Escribir "* CALCULADORA DE MATRICES *"
    Repetir
        Escribir "1. Suma"
        Escribir "2. Resta"
        Escribir "3. Multiplicación"
        Escribir "4. División"
        Escribir "5. Sumar todos los valores de la matriz"
        Escribir "6. Restar todos los valores de la matriz"
        Escribir "7. Suma de matrices"
        Escribir "8. Resta de matrices"
        Escribir "9. Triángulo con números"
        Escribir "10. Rectángulo con asteriscos"
        Escribir "11. Salir"
        Escribir "Seleccione una opción -> "
        Leer opcion
		
        Segun opcion Hacer
            1, 2, 3, 4:
                Escribir "Ingrese el primer número:"
                Leer num1
                Escribir "Ingrese el segundo número:"
                Leer num2
				
                Segun opcion Hacer
                    1: resultado <- num1 + num2
                    2: resultado <- num1 - num2
                    3: resultado <- num1 * num2
                    4: resultado <- num1 / num2
                FinSegun
				
                Escribir "El resultado es:", resultado
                Esperar Tecla
				
            5:
                Escribir "Ingrese el tamaño de la matriz:"
                Leer n
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta n Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "]:"
                        Leer matriz1[i, j]
                    FinPara
                FinPara
				
                suma <- 0
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta n Hacer
                        suma <- suma + matriz1[i, j]
                    FinPara
                FinPara
				
                Escribir "La suma de los valores de la matriz es:", suma
                Esperar Tecla
				
            6:
                Escribir "Ingrese el tamaño de la matriz:"
                Leer n
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta n Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "]:"
                        Leer matriz1[i, j]
                    FinPara
                FinPara
				
                resta <- 0
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta n Hacer
                        resta <- resta - matriz1[i, j]
                    FinPara
                FinPara
				
                Escribir "La resta de los valores de la matriz es:", resta
                Esperar Tecla
				
            7:
                Escribir "Ingrese el tamaño de la matriz 1:"
                Leer n
                Escribir "Ingrese el tamaño de la matriz 2:"
                Leer m
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "] de la matriz 1:"
                        Leer matriz1[i, j]
                    FinPara
                FinPara
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "] de la matriz 2:"
                        Leer matriz2[i, j]
                    FinPara
                FinPara
				
                Dimension matrizResultado[10, 10]
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        matrizResultado[i, j] <- matriz1[i, j] + matriz2[i, j]
                    FinPara
                FinPara
				
                Escribir "La suma de las matrices es:"
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir matrizResultado[i, j]
                    FinPara
                    Escribir ()
                FinPara
				
                Esperar Tecla
				
            8:
                Escribir "Ingrese el tamaño de la matriz 1:"
                Leer n
                Escribir "Ingrese el tamaño de la matriz 2:"
                Leer m
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "] de la matriz 1:"
                        Leer matriz1[i, j]
                    FinPara
                FinPara
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir "Ingrese el valor para la posición [", i, ",", j, "] de la matriz 2:"
                        Leer matriz2[i, j]
                    FinPara
                FinPara
				
                Dimension matrizResultado[10, 10]
				
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        matrizResultado[i, j] <- matriz1[i, j] - matriz2[i, j]
                    FinPara
                FinPara
				
                Escribir "La resta de las matrices es:"
                Para i <- 1 Hasta n Hacer
                    Para j <- 1 Hasta m Hacer
                        Escribir matrizResultado[i, j]
                    FinPara
                    Escribir ()
                FinPara
				
                Esperar Tecla
				
            9:
                Repetir
                    Escribir "1: Imprimir números"
                    Escribir "2: Leer número"
                    Escribir "3: Salir"
                    Escribir ""
                    Escribir "Ingrese una opción: "
                    Leer opcion
					
                    Segun opcion Hacer
                        1:
                            Escribir "Escribe un número"
                            Leer X
                            Para j <- 1 Hasta X Hacer
                                Para i <- 1 Hasta j Hacer
                                    Escribir i Sin Saltar
                                Fin Para
                                Escribir ""
                            Fin Para
							
                        10:
							Escribir ""
							n <- 0
							Mientras n < 3 o n > 20 Hacer
								Escribir "Ingrese un número entre 3 y 20: "
								Leer n
							Fin Mientras
							
							Para i <- 1 Hasta n Hacer
								Para j <- 1 Hasta n Hacer
									Si i = 1 o i = n o j = 1 o j = n Entonces
										Escribir Sin Saltar "* "
									Sino
										Escribir Sin Saltar "  "
									Fin Si
								Fin Para
								Escribir ""
							Fin Para
							
							
                        11:
                            Escribir "Saliendo del programa..."
							
                        De Otro Modo:
                            Escribir "Opción inválida. Intente nuevamente."
                            Esperar Tecla
                    Fin Segun
					
                    Escribir ""
					
                Hasta Que opcion = 11
        FinSegun
    Hasta Que opcion = 11
FinAlgoritmo
