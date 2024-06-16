## Proyecto Class

Una empresaria le ha pedido crear una clase que ella pueda utilizar para crear proyectos fácilmente. Ella pide que cada proyecto tenga un nombre y una descripción. Ella necesita poder crear proyectos vacíos a los que pueda agregar nombre y descripción más adelante, proyectos solo con nombre y también proyectos con ambos parámetros. Todos los proyectos deberían tener getters y setters, ambos métodos. También necesita que cada proyecto pueda Imprimir una breve descripción y devolver nombre y descripción separados por dos puntos ( : ).

Por supuesto, usted necesitará demostrarle sus capacidades a ella, así que cree la clase `ProjectTest` para hacer esto.

### Objetivos

- Practicar sobrecarga tanto de métodos como de constructores.
- Implementar getters y setters.

### Actividades

1. Crear una clase `Project` que tenga los campos `nombre` y `descripcion`.
2. Crear una instancia de método que se llame `elevatorPitch` que devolverá `nombre` y `descripcion` separados por dos puntos ( : ).
3. Sobrecargar el método constructor en tres diferentes formas:
    - `public Project() { }`
    - `public Project(String name) { }`
    - `public Project(String name, String description) { }`
4. Crear getter y setter para cada campo.
5. Crear el archivo `ProjectTest` que hará las pruebas a toda la funcionalidad.

### Desafíos Opcionales

- Agregar una variable `initialCost` de tipo `double` y tenga su propio getter y setter.
- Agregar esto en el paréntesis de `elevatorPitch` después del nombre, ejemplo `nombre (cost): descripcion`.
- Crear una clase `Portfolio` que tendrá un `ArrayList` de `Project` en el campo `projects`. Utilizar Generics para asegurarse que esos son objetos de tipo `Project`.
- Agregar los métodos apropiados de getter y setter y el constructor para que funcione.
- Agregar el método `getPortfolioCost` para calcular y devolver el costo total del portafolio completo.
- Agregar el método `showPortfolio` que mostrará en pantalla todos los proyectos en formato `elevatorPitch`, seguido del costo total.





# Guardia del Zoológico: Parte 1

Una guardia de zoológico le ha pedido ayuda para crear una manera de realizar un seguimiento a los niveles de energía de sus animales. En particular, ella tiene dificultades haciendo un seguimiento a los mamíferos. Cada mamífero debe tener un nivel de energía (predeterminado de 100). Todos deben poder mostrar su nivel de energía cuando se les pregunte a través del método `displayEnergy`, que debe mostrarlo en pantalla y devolver el valor del nivel de energía.

Una vez hecho esto, ella ha pedido que también se cree una clase `Gorilla` a parte, que puede tirar cosas a las personas `throwSomething()` pero perderá energía (-5) cada que lo hace. El `Gorilla` también puede comer bananos `eatBananas()` y recuperará energía (+10). El `Gorilla` también puede trepar a la cima `climb()` y perderá energía (-10).

Ella ha pedido que le demuestre que la clase funciona como se espera haciendo que el `Gorilla` lance algo tres veces, coma bananos dos veces y trepe a la cima una vez, luego debe Imprimir la energía del `Gorilla`.

## Objetivos

- Implementar paquetes para el espacio de trabajo de su proyecto.
- Implementar herencia.

## Actividades

1. Crear una clase `Mammal` que tenga un `energyLevel` y un método `displayEnergy()`. El método `displayEnergy()` debe imprimir el nivel de energía del animal y devolverlo.
2. Crear una clase a parte `Gorilla` que puede `throwSomething()`, `eatBananas()` y `climb()`.
3. Para el método `throwSomething()`, hacer que imprima un mensaje en pantalla indicando que el gorila ha lanzado algo, al mismo tiempo que disminuye su nivel de energía en 5.
4. Para el método `eatBananas()`, hacer que imprima un mensaje en pantalla indicando la satisfacción del gorila e incrementar su nivel de energía en 10.
5. Para el método `climb()`, hacer que muestre un mensaje en pantalla indicando que el gorila ha trepado a la cima de un árbol y disminuir su nivel de energía en 10.

Crear una clase `GorillaTest`, para instanciar al gorila y hacer que lance algo tres veces, coma bananos dos veces y trepe a un árbol una vez.



# Guardia del Zoológico: Parte 2

La guardia del zoológico estaba feliz con el trabajo que usted hizo y ahora quiere algo más de ayuda, ellos han capturado un raro espécimen. Su valor de energía predeterminado es mucho más alto que el de la mayoría de los mamíferos, su nivel de energía es de 300. También puede hacer más que escalar, puede volar. Además, este espécimen no come bananos, come humanos… y no lanza cosas, pero ataca la ciudad. La guardia del zoológico ha capturado un murciélago gigante y quiere su ayuda para realizar un seguimiento a sus niveles de energía.

## Objetivos

- Implementar paquetes para el espacio de trabajo de su proyecto.
- Implementar herencia.

## Actividades

- Crear una clase `Bat` que tenga un método `fly()`, `eatHumans()` y `attackTown()` y que tenga un nivel predeterminado de energía de 300.
- Para el método `fly()`, mostrar el sonido que hace el Bat al despegar y disminuir su nivel de energía en 50.
- Para el método `eatHumans()`, imprimir “bueno, no importa” e incrementar su nivel de energía en 25.
- Para el método `attackTown()`, mostrar en pantalla el sonido de la ciudad en llamas y disminuir su nivel de energía en 100.

Crear la clase `BatTest` para instanciar a `Bat` y hacer que ataque la ciudad tres veces, coma dos humanos y vuele dos veces.



# Maestro de Objetos: Parte 1

Un club local de D&D le ha pedido que les ayude creando unos objetos que ellos podrían utilizar con un simple programa de Java para hacer seguimiento a sus jugadores. Para empezar, a ellos les gustaría tener solo Human en esta campaña en particular. Los Human pueden seleccionar varias clases (Wizard, Ninja, Samurai).

Ellos quieren que los Human tengan 4 propiedades: `strength`, `intelligence`, `stealth` y `health`. El valor predeterminado para cada una de las propiedades debe ser 3, excepto para `health`, que debe ser 100. Cada Human debe tener la habilidad de `attack`, en donde se disminuirá la salud de cualquiera que sea atacado en la cantidad de puntos de `strength` que tenga el atacante.

También quieren ver si usted puede crear una clase que puedan usar antes de cualquier cosa, entonces solo hay que implementar la clase `Human`.

## Objetivos

- Implementar paquetes para el espacio de trabajo de su proyecto.
- Implementar herencia.

## Actividades

- Crear una clase `Human`.
- Agregar los atributos de `strength`, `stealth` e `intelligence` con un valor predeterminado de 3.
- Agregar el atributo `health` con un valor predeterminado de 100.
- Agregar el método `attack(Human)` y reducir el atributo `health` del humano atacado por los puntos de `strength` del humano atacante.

Crear la clase `HumanTest` para probar estos métodos.


