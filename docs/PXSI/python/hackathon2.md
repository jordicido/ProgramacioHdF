# 2a Hackathon IES Hort de Feliu

En esta dinámica os propongo 5 problemas de diferente nivel (de menor a mayor) para que vayáis resolviendo durante la sesión de hoy en parejas. Cuantos más problemas solventéis, más nota tendréis en la prueba.

No se puede avanzar un nivel superior hasta que no pase a revisar la solución del problema. Si no sabéis justificar alguna parte del código o detecto que ha sido consultado a una IA, ese nivel queda anulado y no podéis optar a nota en ese nivel.

Nivel 1 (1 punto)
Nivel 2 (2 puntos)
Nivel 3 (2 puntos)
Nivel 4 (3 puntos)
Nivel 5 (2 puntos)

## Nivel 1 (1 punto)

Haz un programa que muestre la cuenta atrás de un despegue de un cohete desde 10 hasta 1, y luego muestre "¡Despegue!" al final.

## Nivel 2 (2 puntos)

Haz un programa que muestre los números del 1 al 30, pero cumpliendo estas reglas:

* Si el número es par, muestra "Par"
* Si el número es impar, muestra "Impar"
* Si el número es múltiplo de 10, muestra "Diez"

Si un número cumple varias condiciones, solo muestra el texto correspondiente a la más importante (por ejemplo, el múltiplo de 10).

```
1: Impar
2: Par
3: Impar
...
10: Diez
11: Impar
12: Par
...
30: Diez
```

## Nivel 3 (2 puntos)

Haz un programa que pida al usuario palabras y calcule cuántas de ellas son la palabra "python" (sin importar mayúsculas o minúsculas). El programa debe seguir pidiendo palabras hasta que el usuario introduzca la palabra "salir". Al final, muestra el número total de veces que se ha introducido la palabra "python", la cantidad total de palabras introducidas (excluyendo "salir") y el porcentaje que representa. 

```
Palabra: Java
Palabra: python
Palabra: C++
Palabra: PYTHON
Palabra: salir
La palabra "python" se ha introducido 2 veces.
Se han introducido un total de 4 palabras.
El porcentaje de veces que se ha introducido "python" es: 50.0%
```

Recuerda que queremos que el programa ignore las mayúsculas y minúsculas al comparar las palabras, para ello podemos usar el método `.lower()` o `.upper()` de las cadenas de texto.

## Nivel 4 (3 puntos)

Haz un programa que pida al usuario un número entero positivo y calcule si es un número primo o no. Un número primo es aquel que solo es divisible por 1 y por sí mismo. Por ejemplo, el 7 es un número primo porque solo es divisible por 1 y por 7, mientras que el 8 no es un número primo porque es divisible por 1, 2, 4 y 8.

```
Número entero positivo: 7
El número 7 es un número primo.
```

## Nivel 5 (2 puntos)

Haz un programa que pida un número al usuario y luego dibuje un triángulo rectángulo de asteriscos con la altura indicada por el número introducido, pero con forma invertida. Por ejemplo, si el usuario introduce el número 5, el programa debe mostrar:

```
*****
****
***
**
*
```