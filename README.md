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

// Declaración de variables
| Declarar Ingredientes Masa | Tamaño Pizza | Ingredientes Especiales |
| -------------------------- | ------------- |------------------------|
| Harina | Individual | Pepperonni |
| Aceite | Pequeña | Hongos |
| Agua | Grande | Albahaca |
| Levadura | Familiar | Cebolla |
| Sal | #Slides | Jamón |
| Azúcar | - | Queso|
 
 - Crear clase pizza, está va a contener los ingredientes de la pizza, está va a heredar a las pizzas según su tamaño para que contengan la cantidad especifica de ingredientes para crear la masa y agregar ingredientes.
 
 // Ingreso de datos
 
Input int tamPizza: "Bienvenido a Pizza a su gusto. Favor ingrese el tamaño de la pizza que desea:" | Individual | Pequeña | Grande | Personalizado |
Input lista ingEspecial: "Por favor, seleccione los ingredientes que desea en su pizza:" | Pepperonni | Hongos | Albahaca | Cebolla | Jamón | Queso |
*** Hacer validación que la cantidad de ingredientes no sean excesivos para no ablandar la masa, sino enviar mensaje y solicitar nuevamente los Ingredientes Especiales ***
Input direccion = "Favor ingrese su dirección"

//Llamamiento funciones y proceso

- Iniciar precalentado horno y molde
- Iniciar masa = creacionMasa(tamPizza)
- Iniciar pizza = crearPizza(masa, tamPizza, ingEspecial)
- Iniciar pizza.getcortarSlides(tamPizza.getNumSlides)
- Print "Su pizza está en camino para entregar"+ pizza 
- Hacer delivery.pizza(pizza)

// Creación de funciones

//Mezclar ingredientes y formar bola de masa, se devuelve la masa estirada
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

creacionMasa(masa, infoPizza, ingredientesEsp){
 - Tomar la masa estirada
 - Vertir ingredientes especiales, iniciando por la salsa, el queso y luego el resto
 
}

