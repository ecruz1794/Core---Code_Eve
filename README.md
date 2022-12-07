# Core-Code_Eve
Core - Code Bootcamp | Eve Workspace

<h1>CONTENIDO </h1>

<h2>Week 01</h2>

[1. Pizza](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#pizza)

[2. Hot N Cold](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#hot-n-cold)

[3. Some Geometry](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#some-geometry)

[4. Numbers](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#numbers)

[5. Date of Birth](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#date-of-birth)

[6. Treasures](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#treasure)

----------------------------------------------

<h2>Week 02</h2>

[1. Logic problem](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#logic-problem)

[2. Cereal vs Milk](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#que-va-primero-el-cereal-o-la-leche)

[3. Print my name](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#print-my-name)

[4. Print my name & age](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#print-my-name--age)

[5. Algorithm game](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#algorithm-game)

[6. Mod](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#mod)

[7. Register form](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#register-form)

[8. Truth Tables](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#truth-tables)

[9. Boolean results](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#boolean-results)

[10. Identify odd and even numbers](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#identify-odd-and-even-numbers)

-------------------------------------------------

<h2>Week 03</h2>

[1. Simple Calculator](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#simple-calculator)

[2. Special Number](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#special-number)

[3. Simple calculator with Switch](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#calculator-switch)

[4. Multi Option](https://github.com/ecruz1794/Core-Code_Eve/blob/main/README.md#multi-option-program)

[5. algo]()

----------------------------------------------

<h1>Semana 01</h1>

----------------------------------------------

<h3>Pizza</h3>

>// Declaración de variables//


| Declarar Ingredientes Masa | Tamaño Pizza | Ingredientes Especiales |
| -------------------------- | ------------- |------------------------|
| Harina | Individual | Pepperonni |
| Aceite | Pequeña | Hongos |
| Agua | Grande | Albahaca |
| Levadura | Familiar | Cebolla |
| Sal | #Slides | Jamón |
| Azúcar | - | Queso|
 
>*** Crear clase pizza, está va a contener los ingredientes de la pizza, está va a heredar a las pizzas según su tamaño para que contengan la cantidad especifica de ingredientes para crear la masa y agregar ingredientes ***
 
>// Ingreso de datos //
 
>*** Si el tamaño de la pizza es personalizado se va a válidar, se va a crear la clase pizza ajustandose a la personalización, no lo agregue porque se extendería ***

Input int tamPizza: "Bienvenido a Pizza a su gusto. Favor ingrese el tamaño de la pizza que desea:" | Individual | Pequeña | Grande | Personalizado |

Input lista ingEspecial: "Por favor, seleccione los ingredientes que desea en su pizza:" | Pepperonni | Hongos | Albahaca | Cebolla | Jamón | Queso |

>*** Hacer validación que la cantidad de ingredientes no sean excesivos para no ablandar la masa, sino enviar mensaje y solicitar nuevamente los Ingredientes Especiales ***

Input direccion = "Favor ingrese su dirección"

>//Llamamiento funciones y proceso//

- Iniciar precalentado horno y molde
- Iniciar masa = creacionMasa(tamPizza)
- Iniciar pizza = crearPizza(masa, tamPizza, ingEspecial)
- Inciar pizzaHorneada = HornearPizza(pizza, tamPizza)
- Iniciar pizzaLista = cortarSlides (pizzaHorneada, tamPizza.getNumSlides())
- Print "Su pizza está en camino para entregar" + pizza + " en la dirección " + direccion 
- Hacer entrega = delivery.pizza(pizza, direccion)
- Sí entrega es igual a 1 imprimir "Entrega exitosa! Gracias por su compra, provecho!", sino imprimir "Falló entrega, favor comuniquese con el proveedor". 

>// Creación de funciones//
>//Mezclar ingredientes y formar bola de masa, se devuelve la masa estirada//

creacionMasa(infoPizza){
 - Colocar taza
 - Poner ingredientes (Estos toman la cantidad según su tamaño a partir de la clase heredada, harina, agua, aceite, levadura etc.)
 - Mezclar ingredientes
 - Amasar la masa
 - Hacer bola de masa y estirar
 - Cepillar la masa con el aceite
 - Agregar harina espolvoreada en la masa estirada
 - Dejar reposar la masa
 - Devolver masa estirada
 
}

>//Crear la pizza agregando los ingredientes especiales, desde las salsas, queso, hongos etc según el usuario haya solicitado, ingredientesEspeciales es un array/lista //

crearPizza(masa, infoPizza, ingredientesEsp){
 - Tomar la masa estirada
 - Vertir ingredientes especiales, iniciando por la salsa, el queso (En caso que el usuario no solicitara alguno se omiten)
 - Agregar el resto de ingredientes especiales solicitados por el usuario según la lista
 -  Regresar la pizza
 
}

>//Se va a hornear la pizza conforme la duración y temperatura según su clase dependiendo su tamaño, no va a ser el mismo tiempo de cocción para una pizza individual que para una pizza grande//

HornearPizza (pizza, tamPizza){
- Colocar la pizza en el horno precalentado
- Hornear pizza durante pizza.DuracionHorno(tamPizza) a la temperatura de pizza.Temperatura(tamPizza)
- Devolver pizza

}

>// Se va a cortar la pizza según el número de slides del tamaño de la pizza//

cortarSlides( pizza, numSlides){
- Cortar pizza en numSlides proporcionado
- Devolver pizza

}

>// Entrega de la pizza usando la dirección//

delivery.pizza(pizza, dir){
- Llevar la pizza a la dirección entregada en dir
- Tocar el timbre
- Devolver true si la pizza es recibida, sino false

}

-------------------------------------------------------------------

<h3>Hot N Cold</h3>

- Input opc = Buenas! Que tipo de conversión desea realizar:
	1. Celcius a Fahrenheit
	2. Fahrenheit a Celcius
- Válidar que la opción ingresada sea correcta sino volver a solicitarlo
- Input numTemp = Ingrese el valor a convertir.
- resultado = convertirValor( opc, numTemp )
- Print "El valor " + numTemp + " convertido es de: " + resultado. 

>//Función para conversión del valor//

convertirValor( numOpc, numTemp){

int temperatura = 0

If numOpc = 1 entonces {

-	temperatura = 	( numTemp * 9/5 ) + 32

else
-	temperatura = ( numTemp − 32) × 5/9 
	
return temperatura

}

-------------------------------------------------------------

<h3>Some Geometry</h3>

1. Solicitar el tipo de geometría que se desea calcular su volumen
	A. Cubo 
	B. Pirámide 
	C. Esfera
	
2. Válidar los datos ingresados sean válidos

4. Si la geometría es un cubo solicitar tamaño de los lados y devolver lado elevado a la 3

6. Si la geometría es una Pirámide se solicita su altura, longitud de base, ancho de base y se devuelve 1/3 * longitudBase × anchoBase × altura

8. Si la geometría es una esfera se solicitan el radio y se devuelve (4/3)π * radio elevado a la 3

-------------------------------------------------------------------

<h3>Numbers</h3>

>// Diseñar algoritmo que identifique si el número ingresado es par o impar

Input int num = "Ingrese el valor del número que desea evaluar"

string parImpar = evaluarNum(num)

Print "El número dado es" + parImpar

>// Funcion para evaluar el número en par o impar //
evaluarNum(numEvaluar){

If ( numEvaluar/2 == 0 ){
-	return "Par"

else
-	return "Impar"

}

--------------------------------------------------------------------------------------

<h3>Date Of Birth</h3> 

1. dataBirth = "Ingrese el año de su nacimiento"
2. dataYear = "Ingrese el año al cual quiere averigüar su edad"
3. edad = dataYear - dataBirth
4. Print "La edad que va a tener en el año " + dataYear + " es: " + edad
5. Fin

------------------------------------------------------------------------------------------

<h3>Treasure</h3> 

Estamos en una habitación con tres cofres. Sabemos que al menos uno tiene un tesoro en él. Cada cofre tiene un mensaje, pero todos los mensajes son mentiras.

- Cofre izquierdo: El cofre del medio tiene un tesoro.
- Cofre medio: Todos estos cofres tienen tesoros en ellos
- Cofre derecho: Solo uno de estos cofres tiene tesoros.

¿Qué cofres tienen tesoros?

R/ Hay tesoro en el cofre izquierdo y el derecho, porque el enunciado del primero da a conocer que hay un tesoro en el medio, pero este es mentira por la premisa. El cofre derecho que solo uno tiene un tesoro, al ser mentira podemos concluir que dos pueden tener tesoro y sabemos que al menos uno debe tener. Por lo tanto, solo el del medio no tiene tesoro.

-------------------------------------------------------------

<h1>Semana 02</h1>

<h3>Logic Problem</h3> 

> The teacher asks his 5 students if they studied mathematics yesterday.
> 
> Alice: "Nobody studied math yesterday".  
> Bob: "1 person studied math yesterday".  
> Charlie: "2 people studied math yesterday".  
> Dan: "3 people studied mathematics yesterday".  
> Eva: "4 people studied mathematics yesterday".
> 
> The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

Solución: Bob es quién esta diciendo la verdad, porque si alguno de los otros dice la verdad produce contradicción en las premisas y lo que cada uno esta diciendo.

<h3>Que va primero, El Cereal o la Leche?</h3>

** Solución Pseudocódigo **
```
- Inicio programa
- crear bowl
- Int firstAction = "Favor ingrese que desea primero. 1. Cereal  2. Leche"
	If( firAction == 1) {
   		1. Agregar Cereal al bowl;
		2. Agregar Leche al bowl;
	}else{
		if(firstAction == 2){
			1. Agregar leche al bowl;
			2. Agregar cereal al bowl;
		}else{
			Print "Ingreso de datos incorrecto"
			Volver a iniciar programa;
		}
	}
	return bowl;	
- Finalizar 
```
** Solución Diagrama de Flujo **
![_Diagrama de flujo](https://user-images.githubusercontent.com/2061113/204888985-12099344-5758-4a64-9b69-61dbd1e6f0d8.png)

--------------------------------------------------------------

<h3>Print my name</h3>

![myName](https://user-images.githubusercontent.com/2061113/204913686-87a7804e-09fd-4e1d-a800-2d8e63fd5bde.JPG)

-----------------------------------------------------------------

<h3>Print my name & age</h3>

![image](https://user-images.githubusercontent.com/2061113/204913871-75611b05-6a5f-4e26-a736-41805117eca7.png)

-----------------------------------------------------------------

<h3>Algorithm game</h3>

![image](https://user-images.githubusercontent.com/2061113/204917754-a8d82399-22fe-4458-ae75-e3271272226c.png)

-----------------------------------------

<h3>Mod</h3>

![image](https://user-images.githubusercontent.com/2061113/204920562-0153e370-4592-4438-972b-72a4c42fa574.png)

----------------------------------------

<h3>Register form</h3>

![image](https://user-images.githubusercontent.com/2061113/204922846-040ac328-830c-4453-ab07-07fcfde32694.png)

-----------------------------------------

<h3>Truth tables</h3>

- Remember that AND can be represented by & 
- Remember that OR can be represented by | 
- Remember that NOT can be represented by ~| 

1. T & T = T ✅
2. T & F = F ✅
3. F & T = T ❌
4. F & F = F ✅
5. T | T = T ✅
6. T | F = F ❌
7. F | T = T ✅
8. F | F = F ✅
9. ~T = T ❌
10. ~F = T ✅
11. (T & F) | (~F) = T ✅
12. (T | F ) & (F | F) = T ❌
13. ~((T | F ) & (F | F)) & F = T ✅
14. ~((T | F ) & (F | F)) & T = F ✅

-----------------------------------------

<h3>Boolean results</h3>

```
Algoritmo boolean
	a <- 5 == 3		// output: False | Compara si '5' es igual a '3'
	b <- 4 <> 3		// output: True | Compara si '4' es diferente a '3'
	c <- 7 > 7		// output: False | Compara si '7' es mayor a '7'
	d <- 4 < 4		// output: False | Compara si '4' es menor a '4'
	e <- 100 <= 90		// output: False | Compara si '100' es menor o igual a '90'
	f <- 40 >= 40		// output: True | Compara si '40' es mayor o igual a '40'
FinAlgoritmo
```
-----------------------------------------

<h3>Identify odd and even numbers</h3>

```
Proceso IdentParImpar
	Definir num Como Entero
	Definir residuo Como Entero
	Imprimir "Bienvenido, Digite el valor a verificar:"
	Leer num
	Si num%2 == 0 Entonces
		Imprimir "El número ",num," es Par."
	SiNo
		Imprimir "El número ",num, " es Impar."
	Fin Si
FinProceso
```

-----------------------------------------

<h3>Simple Calculator</h3>

```
Proceso calculadoraSimple
	Definir a Como Entero
	Definir b Como Entero
	Definir op Como Caracter
	Definir res Como Entero
	Imprimir "*************	 	Calculadora 	*************"
	Imprimir "Ingrese el primer número: "
	Leer a
	Imprimir "Ingrese el segundo número: "
	Leer b
	Imprimir "Ingrese el tipo de operación a realizar +,-,*,/: "
	Leer op
	Si op == "+" Entonces
		res<-a+b
	SiNo
		Si op == "-" Entonces
			res<-a-b
		SiNo
			Si op == "*" Entonces
				res<-a*b
			SiNo
				Si op == "/" Entonces
					res<-a*b
				SiNo
					Imprimir "Operación Inválida"
				Fin Si
			Fin Si
		Fin Si
	Fin Si
	Imprimir "El resultado de la operación es: " res
FinProceso
```

-----------------------------------------

<h3>Special Number</h3>

```
Proceso specialNumber
	Definir n  Como Entero
	Imprimir "Please put the number to evaluate: "
	Leer n
	Si n == 100 Entonces
		Imprimir "This is a special number"
	SiNo
		Si (n < 1000) & (n % 10 == 0) Entonces
			Imprimir "Almost special number"
		SiNo
			Imprimir "Just a regular number"
		Fin Si
	Fin Si
FinProceso
```

-------------------------------------

<h3>Calculator Switch</h3>

```
Proceso CalculadoraSwitch
	Definir a Como Entero
	Definir b Como Entero
	Definir op Como Caracter
	Imprimir "--------- Calculator ----------"
	Imprimir "Ingrese un número"
	Leer a
	Imprimir "Ingrese el segundo número"
	Leer b
	Imprimir "Ingrese el tipo de operación a realizar +,-,*,/: "
	Leer op
	Segun op Hacer
		"+":
			Imprimir "El resultado es " a+b
		"-":
			Imprimir "El resultado es " a-b
		"*":
			Imprimir "El resultado es " a*b
		"/":
			Imprimir "El resultado es " a/b
		De Otro Modo:
			Imprimir "Operación inválida"
	Fin Segun
FinProceso
```

-------------------------------------

<h3>Multi Option Program</h3>
