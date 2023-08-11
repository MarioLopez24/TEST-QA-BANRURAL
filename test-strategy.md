En este documento se listan todos los fallos encontrados en las pruebas QA realizadas.

Línea 35 - elemento Input recibe parámetros de tipo carácter y no numéricos como se solicito
solución: modificar input type="text" a input type="number".

Línea 35 - comando Input no especifica el rango de números (1-100) aceptados por el juego
Solución: añadir al elemento input que contiene con la class guessField el atributo para el valor mínimo de 1 y el valor máximo de 100.

Línea 44 - el cálculo para el numero aleatorio es generado de 0 a 10, y no de 1 a 100
Solución: añadir a la formula el metodo math.floor para que aproxime el número y retorne un numero entero, así como modificar el valor de 10 a 100 y sumarle 1 para que se tome el rango correcto.

Línea 46 - límite de intentos es menor a 10
Solución: modificar el valor de la constante ATTEMPTS de 5 a 10.

Línea 58 - los números ingresado no deben de ir con décimas, esto complicaría el adivinar el numero entero
Solución: utilizar la función parseInt para convertir el argumento (cadena) y a un entero.

Línea 78 - condicionante if adicional
Solución: eleminiar la condicionante if con la condicion ya que no es necesaria para el proceso

Línea 87 - la sintaxis del evento está mal escrita
Solución: modificar guessSubmit.addeventListener a guessSubmit.addEventListener

funcion checkGuess() - no tiene las condicionales como se especifica en el caso de uso
Solución: organizar correctamente las condiciones de victoria, derrota e intento fallido

Línea 50 - la clase lowOrHi no se selecciona correctamente
Solución: agregar un punto antes de lowOrHi ( const lowOrHi = document.querySelector('.lowOrHi');)

Línea 97 - la sintaxis del evento está mal escrita
Solución: modificar guessSubmit.addeventListener a guessSubmit.addEventListener

Línea 114 - el cálculo para el numero aleatorio no tiene un valor maximo como limite
Solución: añadir a la formula el producto de Math.random() * 100.