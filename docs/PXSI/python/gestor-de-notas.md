# Gestor de notas

En esta práctica que desarrollaremos en varias sesiones, vamos a crear un programa un poco diferente a los que hemos hecho hasta ahora. El programa deberá ejecutarse indefinidamente hasta que el usuario decida salir, y nos permitirá gestionar las notas de los alumnos de una clase.

El programa deberá mostrar un menú con las siguientes opciones:

1. Calcular media del alumno
2. Generar informe de notas
3. Generar nota aleatoria
4. Salir

Vamos a ir desarrollando el programa poco a poco, añadiendo funcionalidades en cada sesión.

## Sesión 1: Construir el menú y la opción de salir del programa

En esta primera sesión, vamos a construir el menú y la opción de salir del programa. Para ello, podemos usar un bucle `while` que se ejecute indefinidamente hasta que el usuario decida salir. Dentro del bucle, mostraremos el menú y pediremos al usuario que introduzca una opción. Si el usuario introduce la opción 4, saldremos del programa.

Como ya hemos visto en la teoría el bucle while se ejecuta indefinidamente mientras se cumpla una condición. En este caso, la condición será que el usuario no haya introducido la opción de salir.

Para completar esta sesión, Tenéis que:

1. Crear un bucle `while` que se ejecute indefinidamente.
2. Mostrar el menú con las opciones.
3. Pedir al usuario que introduzca una opción.
4. Si el usuario introduce cualquiera de las opciones 1, 2 o 3, mostrar un mensaje indicando que esa opción aún no está implementada.
5. Si el usuario introduce la opción 4, salir del programa.
6. Si el usuario introduce una opción no válida, mostrar un mensaje de error y volver a mostrar el menú.

# Sesión 2: Implementar la opción de calcular la media del alumno

En esta sesión, vamos a implementar la opción de calcular la media del alumno. Para ello, pediremos al usuario que introduzca el nombre del alumno y sus notas. Luego, calcularemos la media de las notas y la mostraremos al usuario.

Para completar esta sesión, Tenéis que:

1. Pedir al usuario que introduzca el nombre del alumno.
2. Pedir al usuario que introduzca las notas del alumno, de una en una, como números decimales. El usuario deberá introducir un número negativo para indicar que ha terminado de introducir las notas.
3. Calcular la media de las notas introducidas.
4. Mostrar la media al usuario.

# Sesión 3: Implementar la opción de generar informe de notas

En esta sesión, vamos a implementar la opción de generar informe de notas. Como sabéis en el boletín de notas aparece la nota numérica y la nota cualitativa (sobresaliente, notable, bien, suficiente o insuficiente). Para generar el informe de notas, pediremos al usuario que introduzca el nombre del alumno y sus notas. Luego, calcularemos la media de las notas y la nota cualitativa correspondiente, y las mostraremos al usuario.

Para completar esta sesión, Tenéis que:

1. Pedir al usuario que introduzca el nombre del alumno.
2. Pedir al usuario que introduzca las notas del alumno, de una en una, como números decimales. El usuario deberá introducir un número negativo para indicar que ha terminado de introducir las notas.
3. Calcular la media de las notas introducidas.
4. Determinar la nota cualitativa correspondiente a la media, según la tabla de abajo.
5. Mostrar la media y la nota cualitativa al usuario.

| Media | Nota cualitativa |
|------|------------------|
| 9.0 - 10.0 | Sobresaliente |
| 7.0 - 8.9 | Notable |
| 6.0 - 6.9 | Bien |
| 5.0 - 5.9 | Suficiente |
| 0.0 - 4.9 | Insuficiente |

# Sesión 4: Implementar la opción de generar nota aleatoria

En esta sesión, vamos a implementar la opción de generar notas aleatoria. Como los alumnos estan usando la IA para todo, hemos pensado que tampoco importará si el profesor genera notas aleatorias a los trabajos de los alumnos. Para ello, pediremos al usuario que introduzca el nombre del alumno y el número de notas que desea generar. Luego, generaremos las notas aleatorias, calcularemos la media y la nota cualitativa correspondiente, y las mostraremos al usuario.

Para calcular la nota aleatoria, podemos usar la función `random.uniform(a, b)` del módulo `random`, que devuelve un número decimal aleatorio entre `a` y `b`. En este caso, podemos usar `a = 0.0` y `b = 10.0` para generar notas entre 0 y 10. Para usar el módulo `random`, primero debemos importarlo al principio de nuestro programa con la línea `import random`.

Para completar esta sesión, Tenéis que:
1. Pedir al usuario que introduzca el nombre del alumno.
2. Pedir al usuario que introduzca el número de notas que desea generar, como un número entero positivo.
3. Generar las notas aleatorias usando la función `random.uniform(0.0, 10.0)`.
4. Calcular la media de las notas generadas.
5. Determinar la nota cualitativa correspondiente a la media, según la tabla de la sesión anterior.
6. Mostrar las notas generadas, la media y la nota cualitativa al usuario.