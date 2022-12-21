# core-code-from-scratch-readme-week5

## TIME CONVERTER

Funcion res <- convt(num)

	Definir res Como Caracter
	Definir seg, min, hor, dias Como Entero
	seg = num % 60
	min = Trunc(num/60) % 60
	hor = Trunc(num/3600) % 24
	dias = Trunc(num/86400)
	res = Concatenar(ConvertirATexto(dias), " dias ")
	res = Concatenar(res, ConvertirATexto(hor))
	res = Concatenar(res, " horas ")
	res = Concatenar(res, ConvertirATexto(min))
	res = Concatenar(res, " minutos y ")
	res = Concatenar(res, ConvertirATexto(seg))
	res = Concatenar(res, " segundos")
	
FinFuncion

Algoritmo convertidor

	Escribir convt(150000)
  
FinAlgoritmo

## COMPARE DISTANCES

Funcion res <- compareDistances ()

	Definir res Como Logico
	Definir pos, neg Como Real
	neg = 0
	pos = 0
	Para i=1 Hasta 5 Con Paso 1 Hacer
		Escribir "Ingrese un numero: "
		Leer num
		Si num > 0 Entonces
			pos = pos + num
		SiNo
			neg = neg + num
		Fin Si
		res = pos > abs(neg)
	Fin Para
	
FinFuncion

Algoritmo Compare

	Escribir compareDistances()
	
FinAlgoritmo

## SUM OF PAIRS

Funcion res <- sumOfPairs()

	Definir res Como Entero
	sum = 0
	Repetir
		Escribir "Ingrese un numbero entre 1 y 100"
		Leer num
		Si num % 2 = 0 Entonces
			sum = sum + num
		Fin Si
	Mientras Que num > 0 & num < 100
	res = sum
	
FinFuncion

Algoritmo exampleSumOfPairs
	
	Escribir sumOfPairs()
	
FinAlgoritmo

## MID POINT

Funcion res <- midPoint (num1, num2)
	
	res = (num1 + num2)/2
	
FinFuncion

Algoritmo Mid

	Escribir midPoint(-40,-80)
	Escribir midPoint(40,-80)
	Escribir midPoint(50,50)
	Escribir midPoint(-50,50)
	
FinAlgoritmo
