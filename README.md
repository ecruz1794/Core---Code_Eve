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
 
 - Crear clase pizza, está va a contener los ingredientes de la pizza, está va a heredar 
 a las pizzas según su tamaño para que contengan
 
 // Ingreso de datos
 
Input int tamPizza: "Bienvenido a Pizza a su gusto. Favor ingrese el tamaño de la pizza que desea:" | Individual | Pequeña | Grande | Personalizado |
Input lista ingEspecial: "Por favor, seleccione los ingredientes que desea en su pizza:" | Pepperonni | Hongos | Albahaca | Cebolla | Jamón | Queso |
Input direccion = "Favor ingrese su dirección"

//Llamamiento funciones y proceso

- Iniciar precalentado horno y molde
- Iniciar masa = creacionMasa(tamPizza)
- Iniciar pizza = crearPizza(masa, tamPizza, ingEspecial)
- Iniciar pizza.getcortarSlides(tamPizza.getNumSlides)
- Print "Su pizza está en camino para entregar"+ pizza 
- Hacer delivery.pizza(pizza)

// Creación de funciones
creacionMasa(infoPizza){
 - Colocar taza
 - Poner ingredientes basados
}

