
# **1. De pseudocódigo a Python: el cambio de “lenguaje”**

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

# 🖨️ **2. Primer contacto con Python: `print()` y comentarios**

## 👉 `print()`

La función `print()` sirve para **mostrar texto o valores** en la pantalla.
Es la forma más básica de ver resultados.

```python
print("Hola, mundo")
print("Estamos aprendiendo Python")
print(3 + 7)
```

## 👉 Comentarios `#`

Sirven para añadir notas que el ordenador **no ejecuta**, pero ayudan a entender el programa.

```python
# Esto es un comentario
print("Ejemplo de comentario")
```

**Mensaje clave:**

> Los comentarios ayudan a organizar y explicar el código.

---

# 🔤 **3. Variables y tipos básicos**

En pseudocódigo se usaban variables sin declararlas.
En Python **aparecen cuando les asignas un valor**:

```python
edad = 17
nombre = "Laura"
precio = 19.95
```

## Tipos básicos importantes:

| Tipo    | Ejemplo          | Explicación |
| ------- | ---------------- | ----------- |
| `int`   | `10`             | Enteros     |
| `float` | `3.14`           | Decimales   |
| `str`   | `"Hola"`         | Texto       |
| `bool`  | `True` / `False` | Lógico      |

## Conversión de tipos (porque input() genera texto)

Esto será clave más adelante:

```python
edad = int(input("Introduce tu edad: "))
precio = float(input("Precio: "))
nombre = input("Tu nombre: ")   # No necesita conversión
```

---

# ⌨️ **4. `input()` + conversión de tipos**

En pseudocódigo se usaba:

```
LEER edad
```

En Python:

```python
edad = input("Introduce tu edad: ")
```

Pero **si quieres números**, recuerda que `input()` siempre devuelve una **cadena de texto**, así que necesitas convertirla:

```python
edad = int(input("Introduce tu edad: "))
altura = float(input("Introduce tu altura: "))
```

**Explicación importante para el alumnado:**

> Si no conviertes los números, Python no te dejará sumarlos o compararlos correctamente.

---

# ➕ **5. Operadores: aritméticos, comparación y lógicos**

Aquí ya han visto la mayoría en pseudocódigo, pero toca formalizarlo.

## Operadores aritméticos

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

## Operadores de comparación

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

## Operadores lógicos

* `and`
* `or`
* `not`

```python
print(edad >= 18 and edad <= 65)
print(edad < 0 or edad > 120)
print(not (edad < 0))
```

---

# 🔀 **6. Condicionales: `if`, `elif`, `else`**

Lo más importante del puente pseudocódigo → Python.

## Estructura básica:

### Pseudocódigo:

```
SI condición ENTONCES
    ...
SINO
    ...
FIN_SI
```

### Python:

```python
if condición:
    ...
else:
    ...
```

### Ejemplo:

```python
edad = int(input("Edad: "))

if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

---

# 🔽 **6.1. Múltiples condiciones: `elif`**

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

# 🧪 **7. Mini ejercicios puente pseudocódigo → Python**

Aquí los alumnos conectan todo:

### Ejercicio 1: Par o impar

```python
n = int(input("Número: "))

if n % 2 == 0:
    print("Par")
else:
    print("Impar")
```

### Ejercicio 2: Clasificación por edad

```python
edad = int(input("Edad: "))

if edad < 13:
    print("Niño")
elif edad < 18:
    print("Adolescente")
else:
    print("Adulto")
```

### Ejercicio 3: Contraseña

```python
pw = input("Contraseña: ")

if pw == "python123":
    print("Acceso permitido")
else:
    print("Acceso denegado")
```

**Objetivo de estos ejercicios:**
Consolidar input, conversión, if/elif/else y operadores.

---
