# 3a Hackathon IES Hort de Feliu

En esta dinámica os propongo 5 problemas de diferente nivel (de menor a mayor) para que vayáis resolviendo durante la sesión de hoy en parejas. Cuantos más problemas solventéis, más nota tendréis en la prueba.

No se puede avanzar un nivel superior hasta que no pase a revisar la solución del problema. Si no sabéis justificar alguna parte del código o detecto que ha sido consultado a una IA, ese nivel queda anulado y no podéis optar a nota en ese nivel.

Nivel 1 (1 punto)
Nivel 2 (2 puntos)
Nivel 3 (2 puntos)
Nivel 4 (3 puntos)
Nivel 5 (2 puntos)

## Nivel 1 (1 punto)

La profesora de música del IES Hort de Feliu necesita un programa para guardar los nombres de los alumnos de su clase. El programa debe pedir el nombre de 5 alumnos, guardarlos en una lista y mostrar la lista completa al final usando un bucle.

Ejemplo de resultado:

```
Nombre alumno 1: Ana
Nombre alumno 2: Luis
Nombre alumno 3: Marta
Nombre alumno 4: Carlos
Nombre alumno 5: Elena
Alumnos de música:
- Ana
- Luis
- Marta
- Carlos
- Elena
```

## Nivel 2 (2 puntos)

El profesor de matemáticas del IES Hort de Feliu necesita calcular estadísticas de las notas de su clase. El programa debe pedir el número de alumnos y luego la nota de cada uno. Al final debe mostrar la nota más alta, la nota más baja y la nota media de la clase.

No se puede usar `max()`, `min()` ni `sum()` directamente. Hay que calcularlos recorriendo la lista con un bucle.

Ejemplo de resultado:

```
Número de alumnos: 4
Nota alumno 1: 7
Nota alumno 2: 5
Nota alumno 3: 9
Nota alumno 4: 6
Nota más alta: 9.0
Nota más baja: 5.0
Nota media: 6.75
```

## Nivel 3 (2 puntos)

El departamento de orientación del IES Hort de Feliu quiere separar a los alumnos aprobados de los suspendidos. El programa debe pedir el número de alumnos y la nota de cada uno. Al final debe mostrar dos listas separadas: una con las notas de los aprobados (nota >= 5) y otra con las notas de los suspendidos.

Ejemplo de resultado:

```
Número de alumnos: 5
Nota alumno 1: 7
Nota alumno 2: 3
Nota alumno 3: 9
Nota alumno 4: 4
Nota alumno 5: 6
Aprobados (3 alumnos): [7.0, 9.0, 6.0]
Suspendidos (2 alumnos): [3.0, 4.0]
```

## Nivel 4 (3 puntos)

El profesor de educación física quiere registrar los tiempos de los alumnos en una carrera de 100 metros. El programa debe pedir el nombre y el tiempo en segundos de cada alumno. Al final debe mostrar el nombre del alumno más rápido y el del más lento.

No se puede usar `max()` ni `min()` directamente. Hay que encontrar los valores recorriendo las listas con un bucle.

Ejemplo de resultado:

```
Número de alumnos: 3
Nombre alumno 1: Ana
Tiempo de Ana (segundos): 14.5
Nombre alumno 2: Luis
Tiempo de Luis (segundos): 12.3
Nombre alumno 3: Marta
Tiempo de Marta (segundos): 13.8
El alumno más rápido es Luis con 12.3 segundos.
El alumno más lento es Ana con 14.5 segundos.
```

## Nivel 5 (2 puntos)

Los alumnos de 1º de Bachillerato van a votar el destino del viaje de fin de curso. El programa debe tener una lista fija con 4 destinos posibles. Luego debe pedir el número de alumnos y el voto de cada uno. Si un alumno introduce un destino que no está en la lista, el programa debe avisarle y pedirle que vote de nuevo. Al final, debe mostrar el recuento de votos de cada destino y el destino ganador.

Ejemplo de resultado:

```
Destinos disponibles: ['París', 'Roma', 'Londres', 'Berlín']
Número de alumnos: 4
Voto alumno 1: París
Voto alumno 2: Madrid
Destino no válido. Vuelve a votar.
Voto alumno 2: Roma
Voto alumno 3: París
Voto alumno 4: Londres
Resultados:
- París: 2 votos
- Roma: 1 voto
- Londres: 1 voto
- Berlín: 0 votos
El destino ganador es París con 2 votos.
```
