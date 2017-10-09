﻿# CIFRADO CESAR
### Pseudocodigo


##### Algoritmo Cipher

	Definir num,output,input1,j,k Como Entero
	Definir input Como Caracter
	Escribir 'Ingrese una frase:'
	Leer input
	Mientras (input=='') Hacer
		Escribir 'Ingrese una frase:'
		Leer input
		Para j<-0 Hasta Longitud(input)Hacer
			Mientras input[j]=== num Hacer
				Escribir 'Ingrese una frase sin n�meros:'
			FinMientras
			Leer output
		FinPara
	FinMientras
	Leer output
	input1 <-  Mayusculas[input]
	Para k <-0 Hasta Longitud(input1) Hacer
		Si  input1[k] === ' '
			Entonces output = ' '
		SiNo
			Entonces output = String.fromCharCode((input1.charCodeAt(k) - 65 + 33) % 26 + 65)
		Fin Si Entonces
	FinPara
	Mostrar en pantalla output
  FinAlgoritmo
##### Algoritmo Decipher

	Definir output1,i Como Entero
	Definir input2 Como Caracter
	Escribir 'Ingrese la frase que desea decifrar'
	Leer input2
	Para i<-0 Hasta Longitud(input2)Hacer
		Si input2[i] === ' '
		Entonces output1 = ' '
		Si No
		Entonces output1 += String.fromCharCode((input2.charCodeAt(i) - 65 + 19) % 26 + 65)
		Fin Si Entonces
	FinPara
	Mostrar en pantalla output1
  FinAlgoritmo
