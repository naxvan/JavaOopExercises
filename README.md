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



# Maestro de Objetos: Parte 2

Al club le gustó mucho su trabajo y le han pedido desarrollar un poco más las opciones del personaje. Quieren agregar las clases de Ninja, Wizard y Samurai pero también quieren que cualquier modificación hecha en la clase Human se extienda a estas.

Adicional a esto, cada clase tendrá algunas características únicas:

## Clase Wizard
- Valor predeterminado de salud: 50.
- Valor predeterminado de inteligencia: 8.
- Método `heal(Human)`: Permite curar al otro Human en una cantidad igual a la inteligencia del Wizard.
- Método `fireBall(Human)`: Disminuye la salud del otro Human en 3 veces la inteligencia del Wizard.

## Clase Ninja
- Valor predeterminado de sigilo: 10.
- Método `steal(Human)`: Roba la salud del otro Human igual al nivel de sigilo del Ninja.
- Método `runAway()`: Reduce la salud del Ninja en 10.

## Clase Samurai
- Valor predeterminado de salud: 200.
- Método `deathBlow(Human)`: Ataca al otro Human y reduce su salud a 0, también reduce la salud del Samurai a la mitad.
- Método `meditate()`: Cura al Samurai en la mitad de su salud actual.
- Método `howMany()`: Devuelve el número actual de Samurais.

## Objetivos
- Implementar paquetes para el espacio de trabajo de su proyecto.
- Implementar herencia.

## Actividades
- Crear las clases `Wizard`, `Ninja` y `Samurai`, todas extendiendo de la clase `Human`.
- Wizard: Establecer un valor predeterminado de health en 50.
- Wizard: Establecer un valor predeterminado de intelligence en 8.
- Wizard: Agregar un método heal(Human) que aumentará la salud del otro Human en los puntos de intelligence que tenga el Wizard.
- Wizard: Agregar un método fireBall(Human) que disminuye la salud del otro Human en los puntos de intelligence * 3 que tenga el Wizard.
- Ninja: Establecer un valor predeterminado de stealth en 10.
- Ninja: Agregar un método steal(Human) que roba la cantidad de puntos que tenga el Ninja en stealth de la salud del otro Human y los agrega a la health del Ninja.
- Ninja: Agregar un método runAway() que reduce su salud en 10.
- Samurai: Establecer un valor predeterminado de health en 200.
- Samurai: Agregar un método deathBlow(Human) que asesina al otro Human y reduce la health del Samurai a la mitad.
- Samurai: Agregar un método meditate() que curará al Samurai en la mitad de puntos que tenga de health.
- Samurai: Agregar un método howMany() que devuelve el número actual del Samurai.

# Cuenta de Banco

Vamos a crear la clase `BankAccount`. Esta clase recreará algunas de las transacciones más comunes que normalmente ocurren en una cuenta de banco como mostrar su número de cuenta, monto en cuenta corriente y de ahorros, monto total. Por supuesto, hay métodos que invocar, tanto como depositar un cheque, verificar saldo, retirar dinero.

## Objetivos

- Practicar variables principales.
- Practicar métodos de instancia, getters y setters.
- Implementar variables y métodos estáticos.

## Actividades

1. Crear una clase `BankAccount`.
2. La clase debe tener los siguientes atributos: `(string) número de cuenta`, `(double) saldo cuenta corriente`, `(double) saldo cuenta de ahorros`.
3. Crear una variable `(static)` que contenga el número de cuentas creadas hasta el momento.
4. Crear una variable `(static)` que rastree la cantidad de dinero almacenado en cada cuenta creada.
5. Crear un método privado que retorne un número de 10 dígitos aleatorios para el número de cuenta.
6. En el constructor, llamar al método privado anterior, así cada usuario tendrá un número de cuenta de 10 dígitos aleatorios.
7. En el constructor, asegurarse de incrementar el contador de cuentas creadas.
8. Crear un método getter para el saldo de la cuenta corriente del usuario.
9. Crear un método getter para el saldo de la cuenta de ahorros del usuario.
10. Crear un método que permita al usuario depositar dinero en su cuenta corriente o cuenta de ahorros, asegúrese de aumentar el total de dinero almacenado.
11. Crear un método para retirar dinero de una cuenta. No permita que retire dinero si tiene fondos insuficientes.
12. Crear un método para ver el total de dinero en la cuenta corriente y en la cuenta de ahorros.
13. Los usuarios no deberían poder configurar ningún atributo de la clase.

# En esta actividad, crearemos una Pokedex que nos dé información acerca de los Pokemon.

## Objetivos

- Practicar con variables y métodos estáticos.
- Definir clases abstractas.
- Definir interfaces.
- Implementar clases que utilicen clases abstractas e interfaces.

## Actividades

- Crear una clase `Pokemon` con:
  - `name`, `health` y `type` como variables principales.
  - `void attackPokemon(Pokemon pokemon)` Este método reduce la salud del Pokemon atacado en 10 puntos.
  - Una variable estática `count` para mantener el número de Pokemones creados en el programa.
  - Getter y Setter para cada variable principal.
  - Un constructor para establecer `name`, `health` y `type` en la creación de la instancia.
 



# Teléfonos

En esta actividad vamos a utilizar clases `Abstract` e `Interface` para crear 2 tipos de teléfonos: iPhone y Galaxy.

## Objetivos

- Definir clases.
- Definir Interfaces.
- Implementar clases que utilicen clases abstractas e interfaces.

## Actividades

- Crear una clase abstracta `Phone`.

- Crear una interfaz `Ringable` que contenga los siguientes métodos:
  - `ring()`: Este método retorna un String.
  - `unlock()`: Este método retorna un String.

- Crear las clases `IPhone` y `Galaxy`.
  - Ambas clases deben extender/heredar de la clase abstracta `Phone` e implementar de la interfaz `Ringable`.

- Implementar los métodos (`ring`, `unlock`, `displayInfo`) de las clases `IPhone` y `Galaxy`.

### Ejemplo de Implementación Esperada:
## Consola:

Galaxy S9 From Verizon
Galaxy Says: Ring ring ring
Unlocking via finger print
-----------------------------------------------------------
Iphone: x From AT&T
Iphone says: Zing
Unloking via facial recognition



