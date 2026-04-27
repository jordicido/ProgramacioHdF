# Programación en Python

## **1. De pseudocódigo a Python: el cambio de “lenguaje”**

Antes de escribir código, es importante explicar que Python es un **lenguaje real**, mientras que el pseudocódigo era solo una forma de describir ideas.
Por eso en Python hay reglas **más estrictas**:

* Python usa **sangrías (indentación)** para saber qué instrucciones están dentro de un bloque.
* Python usa **dos puntos `:`** al iniciar bloques (`if`, `elif`, `else`, `while`, `for`, `def`…).
* El pseudocódigo usaba estructuras como `INICIO` y `FIN`, pero en Python **no existen**: el programa empieza desde la primera línea ejecutable.
* Ya no escribiremos:

  ```
  LEER nombre
  MOSTRAR nombre
  ```

  sino que usaremos funciones reales:

  * `input()` para pedir datos
  * `print()` para mostrar datos

---

## **2. Primer contacto con Python: `print()` y comentarios**

### `print()`

La función `print()` sirve para **mostrar texto o valores** en la pantalla.
Es la forma más básica de ver resultados.

```python
print("Hola, mundo")
print("Estamos aprendiendo Python")
print(3 + 7)
```

Hay varias formas de usar `print()`:
- Mostrar texto: `print("Texto aquí")`
- Mostrar variables: `print(variable)`
- Mostrar varios elementos separados por comas: `print("La edad es", edad)`

Por último, puedes usar una opción de la función print para combinar texto y variables de forma más avanzada:

```python
nombre = "Ana"
edad = 20
print(f"{nombre} tiene {edad} años.")
```

Se llama **f-strings** y es muy útil para crear mensajes dinámicos.

### Comentarios `#`

Sirven para añadir notas que el ordenador **no ejecuta**, pero ayudan a entender el programa.

```python
# Esto es un comentario
print("Ejemplo de comentario")
```

> Los comentarios ayudan a organizar y explicar el código.

---

## **3. Variables y tipos básicos**

En pseudocódigo se usaban variables sin declararlas.
En Python **aparecen cuando les asignas un valor**:

```python
edad = 17
nombre = "Laura"
precio = 19.95
```

Las variables en Python tienen **tipos de datos** que determinan qué tipo de valor almacenan, sin embargo, Python es un lenguaje de tipado dinámico, por lo que no necesitas declarar el tipo explícitamente e incluso puedes cambiar el tipo de una variable reasignándole un valor de otro tipo.

### Tipos básicos importantes:

| Tipo    | Ejemplo          | Explicación |
| ------- | ---------------- | ----------- |
| `int`   | `10`             | Enteros     |
| `float` | `3.14`           | Decimales   |
| `str`   | `"Hola"`         | Texto       |
| `bool`  | `True` / `False` | Lógico      |

### Conversión de tipos (porque input() genera texto)

Esto será clave más adelante:

```python
edad = int(input("Introduce tu edad: "))
precio = float(input("Precio: "))
nombre = input("Tu nombre: ")   # No necesita conversión
```

---

## **4. `input()` + conversión de tipos**

En pseudocódigo se usaba:

```
LEER edad
```

En Python:

```python
edad = input("Introduce tu edad: ")
```

El mensaje entre paréntesis se muestra al usuario, es una manera de hacer un MOSTRAR y un LEER en una sola línea.

Pero **si quieres números**, recuerda que `input()` siempre devuelve una **cadena de texto**, así que necesitas convertirla:

```python
edad = int(input("Introduce tu edad: "))
altura = float(input("Introduce tu altura: "))
```

> Si no conviertes los números, Python no te dejará sumarlos o compararlos correctamente.

---

## **5. Operadores: aritméticos, comparación y lógicos**

Aquí ya han visto la mayoría en pseudocódigo, pero toca formalizarlo.

### Operadores aritméticos

* `+` suma
* `-` resta
* `*` multiplicación
* `/` división decimal
* `//` división entera
* `%` resto
* `**` potencia

Ejemplos:

```python
print(10 / 3)   # 3.333...
print(10 // 3)  # 3
print(10 % 3)   # 1
print(2 ** 3)   # 8
```

## Ejemplos de práctica:

1. Calcula el área de un rectángulo pidiendo al usuario el ancho y el alto.
2. Pide dos números y muestra su suma, resta, multiplicación y división.
3. Convierte una cantidad en euros a dólares (1 euro = 1.1 dólares).
4. Calcula el resto de dividir dos números introducidos por el usuario.
5. Pide al usuario su nombre y edad, y muestra un mensaje personalizado usando f-strings.


### Operadores de comparación

* `==` igual
* `!=` distinto
* `<`
* `<=`
* `>`
* `>=`

```python
edad = 18
print(edad >= 18)  # True
```

### Operadores lógicos

* `and`
* `or`
* `not`

```python
print(edad >= 18 and edad <= 65)
print(edad < 0 or edad > 120)
print(not (edad < 0))
```

---

## **6. Condicionales: `if`, `elif`, `else`**

Lo más importante del puente pseudocódigo → Python.

### Estructura básica:

#### Pseudocódigo:

```
SI condición ENTONCES
    ...
SINO
    ...
FIN_SI
```

#### Python:

```python
if condición:
    ...
else:
    ...
```

Ten en cuenta los dos puntos `:` y la indentación, sin los cuales el código no funcionará.

#### Ejemplo:

```python
edad = int(input("Edad: "))

if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

---

## **6.1. Múltiples condiciones: `elif`**

Explicas que `elif` = “sino si”, y que evita anidar muchos `if`:

```python
nota = float(input("Nota: "))

if nota < 5:
    print("Suspenso")
elif nota < 7:
    print("Aprobado")
elif nota < 9:
    print("Notable")
else:
    print("Sobresaliente")
```

Explicación clave:

> Python evalúa de arriba a abajo y ejecuta solo el primer bloque que se cumpla.

---

## **6.2. Condiciones compuestas**

Puedes combinar condiciones usando operadores lógicos:

```python
edad = int(input("Edad: "))
if edad >= 18 and edad <= 65:
    print("Eres adulto")
else:
    print("No eres adulto")
```

Es importante entender cómo funcionan los operadores lógicos para crear condiciones más complejas. 

---


## **7. Bucles (repeticiones): while y for**

En pseudocódigo ya se trabajaba la **repetición de instrucciones** mediante estructuras como *MIENTRAS*, *PARA* o *HASTA QUE*.
En Python estas estructuras existen, pero con su propia sintaxis y reglas.

La idea clave de un bucle es:

> **Repetir un bloque de instrucciones mientras se cumpla una condición o un número determinado de veces.**

---

### **7.1. Bucle `while` (mientras)**

El bucle `while` repite un bloque de código **mientras una condición sea verdadera**.

#### Pseudocódigo:

```
MIENTRAS condición HACER
    instrucciones
FIN_MIENTRAS
```

#### Python:

```python
while condición:
    instrucciones
```

⚠️ **Importante**:

* La condición se evalúa **antes** de cada repetición.
* Si la condición nunca deja de cumplirse, el programa entra en un **bucle infinito**.

#### Ejemplo básico:

```python
contador = 1

while contador <= 5:
    print(contador)
    contador = contador + 1
```

Salida:

```
1
2
3
4
5
```

Observa que **es obligatorio modificar la variable** que controla la condición.

---

### 7.2. Ejemplos prácticos con `while`

**Ejemplo 1: pedir un número hasta que sea positivo**

```python
numero = int(input("Introduce un número positivo: "))

while numero <= 0:
    numero = int(input("Error. Introduce un número positivo: "))

print("Número correcto:", numero)
```

**Ejemplo 2: contador regresivo**

```python
cuenta = 10

while cuenta > 0:
    print(cuenta)
    cuenta = cuenta - 1

print("¡Despegue!")
```

---

### **7.3. Bucle `for` (repeticiones controladas)**

El bucle `for` se utiliza cuando **sabemos cuántas veces** queremos repetir un bloque de instrucciones.

En Python, el `for` se usa normalmente junto con la función `range()`.

Es especialmente útil para:

* Contar números
* Recorrer rangos
* Tablas de multiplicar
* Repeticiones con inicio y fin claros

---

### **Estructura básica del `for`**

```python
for variable in range(inicio, fin):
    instrucciones
```

Aspectos importantes:

* `inicio` es el valor inicial (incluido)
* `fin` es el valor final (**no incluido**)
* La variable cambia automáticamente en cada repetición

---

### **7.4. Ejemplo básico de `for`**

Mostrar los números del 1 al 5:

```python
for i in range(1, 6):
    print(i)
```

Salida:

```
1
2
3
4
5
```

---

### **7.5. La función `range()`**

La función `range()` genera una secuencia de números.

Formas más comunes de usarla:

```python
range(5)        # 0, 1, 2, 3, 4
range(1, 6)     # 1, 2, 3, 4, 5
range(0, 10, 2) # 0, 2, 4, 6, 8
```

Ejemplo con salto:

```python
for i in range(0, 11, 2):
    print(i)
```

---

### **7.6. Ejemplo práctico: tabla de multiplicar con `for`**

```python
numero = int(input("Número: "))

for i in range(1, 11):
    print(f"{numero} x {i} = {numero * i}")
```

---

### **7.7. Contar hacia atrás con `for`**

```python
for i in range(10, 0, -1):
    print(i)

print("¡Despegue!")
```

---

### **7.8. `for` vs `while`**

| `for`                  | `while`                   |
| ---------------------- | ------------------------- |
| Repeticiones conocidas | Repeticiones desconocidas |
| Control automático     | Control manual            |
| Más sencillo           | Más flexible              |
| Evita bucles infinitos | Puede ser infinito        |

**Regla práctica para el alumnado**:

> Si sabes cuántas veces se repite → `for`
> Si no lo sabes → `while`

---

### **7.9. Bucles y condicionales combinados**

Dentro de un bucle `for` también se pueden usar condicionales.

**Ejemplo: contar números pares del 1 al 10**

```python
contador = 0

for i in range(1, 11):
    if i % 2 == 0:
        contador = contador + 1

print("Cantidad de números pares:", contador)
```

---

### **7.10. Errores comunes con `for`**

❌ Confundir el valor final del `range()`
❌ Pensar que el `range()` incluye el último número
❌ Modificar manualmente la variable del bucle
❌ Usar `for` cuando debería usarse `while`

Perfecto 👌
Te añado ahora el **apartado 8 – Listas en Python**, manteniendo exactamente el mismo estilo, nivel y progresión didáctica que llevas en los apuntes.

Puedes copiarlo tal cual a continuación del apartado 7.

---

# **8. Listas en Python**

Hasta ahora hemos trabajado con variables que almacenan **un solo valor**.
Pero muchas veces necesitamos guardar **varios valores juntos**.

Para eso usamos las **listas**.

---

## **8.1. ¿Qué es una lista?**

Una **lista** es una estructura de datos que permite almacenar **varios elementos en una sola variable**.

Se escribe usando **corchetes `[]`** y separando los elementos con comas.

```python
numeros = [1, 2, 3, 4, 5]
nombres = ["Ana", "Luis", "Marta"]
```

Una lista puede contener:

* Números
* Textos
* Valores lógicos
* Incluso mezclarlos (aunque no es lo más habitual)

```python
mezcla = [10, "Hola", True]
```

---

## **8.2. Acceder a los elementos (índices)**

Cada elemento de la lista tiene una **posición**, llamada **índice**.

⚠️ Muy importante:

> En Python, los índices empiezan en 0.

Ejemplo:

```python
nombres = ["Ana", "Luis", "Marta"]

print(nombres[0])  # Ana
print(nombres[1])  # Luis
print(nombres[2])  # Marta
```

---

## **8.3. Modificar un elemento**

Podemos cambiar un elemento accediendo a su posición:

```python
nombres = ["Ana", "Luis", "Marta"]
nombres[1] = "Carlos"

print(nombres)
```

Salida:

```
['Ana', 'Carlos', 'Marta']
```

---

## **8.4. Añadir elementos**

Para añadir un elemento al final de la lista usamos el método `.append()`:

```python
numeros = [1, 2, 3]
numeros.append(4)

print(numeros)
```

Salida:

```
[1, 2, 3, 4]
```

---

## **8.5. El tamaño de una lista**

Para saber cuántos elementos tiene una lista usamos `len()`:

```python
numeros = [10, 20, 30]
print(len(numeros))
```

Salida:

```
3
```

---

## **8.6. Recorrer una lista con `for`**

Una de las cosas más habituales es recorrer una lista con un bucle `for`.

```python
nombres = ["Ana", "Luis", "Marta"]

for nombre in nombres:
    print(nombre)
```

Aquí, `nombre` toma el valor de cada elemento en cada repetición.

---

## **8.7. Recorrer una lista usando índices**

También podemos recorrerla usando `range()` y posiciones:

```python
nombres = ["Ana", "Luis", "Marta"]

for i in range(len(nombres)):
    print(nombres[i])
```

---

## **8.8. Buscar un elemento**

Podemos comprobar si un elemento está dentro de una lista usando `in`:

```python
nombres = ["Ana", "Luis", "Marta"]

if "Ana" in nombres:
    print("Está en la lista")
```

---

## **8.9. Listas + acumuladores**

Las listas se combinan muy bien con bucles y acumuladores.

Ejemplo: sumar todos los números de una lista.

```python
numeros = [10, 20, 30, 40]
suma = 0

for numero in numeros:
    suma += numero

print("La suma es:", suma)
```

---

## **8.10. Errores comunes con listas**

❌ Olvidar que empiezan en índice 0
❌ Acceder a una posición que no existe
❌ Confundir `.append()` con `=`
❌ Modificar la lista mientras se recorre sin entender lo que ocurre

