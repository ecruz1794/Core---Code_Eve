# Core-Code_Eve
Core - Code Bootcamp | Eve Workspace

<h1>CONTENIDO </h1>

<h2>Week 01</h2>

1. Pizza
-
-
-

----------------------------------------------

<h3>Pizza</h3>

// Declaración de variables//
| Declarar Ingredientes Masa | Tamaño Pizza | Ingredientes Especiales |
| -------------------------- | ------------- |------------------------|
| Harina | Individual | Pepperonni |
| Aceite | Pequeña | Hongos |
| Agua | Grande | Albahaca |
| Levadura | Familiar | Cebolla |
| Sal | #Slides | Jamón |
| Azúcar | - | Queso|
 
 *** Crear clase pizza, está va a contener los ingredientes de la pizza, está va a heredar a las pizzas según su tamaño para que contengan la cantidad especifica de ingredientes para crear la masa y agregar ingredientes ***
 
 // Ingreso de datos //
 
*** Si el tamaño de la pizza es personalizado se va a válidar, se va a crear la clase pizza ajustandose a la personalización, no lo agregue porque se extendería ***

Input int tamPizza: "Bienvenido a Pizza a su gusto. Favor ingrese el tamaño de la pizza que desea:" | Individual | Pequeña | Grande | Personalizado |
Input lista ingEspecial: "Por favor, seleccione los ingredientes que desea en su pizza:" | Pepperonni | Hongos | Albahaca | Cebolla | Jamón | Queso |
*** Hacer validación que la cantidad de ingredientes no sean excesivos para no ablandar la masa, sino enviar mensaje y solicitar nuevamente los Ingredientes Especiales ***

Input direccion = "Favor ingrese su dirección"

//Llamamiento funciones y proceso//

- Iniciar precalentado horno y molde
- Iniciar masa = creacionMasa(tamPizza)
- Iniciar pizza = crearPizza(masa, tamPizza, ingEspecial)
- Inciar pizzaHorneada = HornearPizza(pizza, tamPizza)
- Iniciar pizzaLista = cortarSlides (pizzaHorneada, tamPizza.getNumSlides())
- Print "Su pizza está en camino para entregar" + pizza + " en la dirección " + direccion 
- Hacer entrega = delivery.pizza(pizza, direccion)
- Sí entrega es igual a 1 imprimir "Entrega exitosa! Gracias por su compra, provecho!", sino imprimir "Falló entrega, favor comuniquese con el proveedor". 

// Creación de funciones//

//Mezclar ingredientes y formar bola de masa, se devuelve la masa estirada//

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

//Crear la pizza agregando los ingredientes especiales, desde las salsas, queso, hongos etc según el usuario haya solicitado, ingredientesEspeciales es un array/lista //

crearPizza(masa, infoPizza, ingredientesEsp){
 - Tomar la masa estirada
 - Vertir ingredientes especiales, iniciando por la salsa, el queso (En caso que el usuario no solicitara alguno se omiten)
 - Agregar el resto de ingredientes especiales solicitados por el usuario según la lista
 -  Regresar la pizza
 - 
}

//Se va a hornear la pizza conforme la duración y temperatura según su clase dependiendo su tamaño, no va a ser el mismo tiempo de cocción para una pizza individual que para una pizza grande//

HornearPizza (pizza, tamPizza){
- Colocar la pizza en el horno precalentado
- Hornear pizza durante pizza.DuracionHorno(tamPizza) a la temperatura de pizza.Temperatura(tamPizza)
- Devolver pizza
}

// Se va a cortar la pizza según el número de slides del tamaño de la pizza//

cortarSlides( pizza, numSlides){
- Cortar pizza en numSlides proporcionado
- Devolver pizza

}

// Entrega de la pizza usando la dirección//

delivery.pizza(pizza, dir){
- Llevar la pizza a la dirección entregada en dir
- Tocar el timbre
- Devolver true si la pizza es recibida, sino false
-
}
