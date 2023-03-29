# Barreras_python

### Francisco Ogando (2021-0160)
[Link explicación del código]()

*Esta es mi documentación sobre el bloque de código que usted dejó Lizandro acerca de las barreras en python, primero se importa el módulo de hilos de Python y la función sleep del módulo de tiempo. Además, se define un objeto mutex (bloqueo mutuo) que se usa para sincronizar el acceso a una variable compartida.*

*La clase Hilo se define como una subclase de threading.Thread, lo que significa que cada objeto Hilo es un subproceso que se puede ejecutar simultáneamente con otros subprocesos. Cada objeto Hilo tiene una propiedad "id" que se establece en la creación del objeto.*

*La función "run" se define para cada objeto Hilo y se ejecuta cuando se llama al método "start" del objeto. El método "acquire" del objeto mutex se llama al principio de la función "run" para bloquear el acceso a la variable compartida "d". Luego, el hilo llama a la función sleep con un valor que depende del valor de su propiedad "id". Finalmente, el hilo imprime un mensaje que muestra su propiedad "id" y el valor actual de "d".*

*Fuera de la definición de la clase Hilo, se define la variable "d" con un valor de 1 y se crea una lista de tres objetos Hilo con diferentes valores de "id". Luego, se inicia cada hilo en la lista con el método "start", lo que hace que cada hilo ejecute su función "run" en paralelo con los otros hilos.*

*En resumen, este bloque de código crea tres subprocesos que acceden a una variable compartida "d" y se sincronizan mediante un objeto mutex para evitar conflictos de acceso. Cada hilo espera un tiempo diferente antes de imprimir su propiedad "id" y el valor actual de "d".*
