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
