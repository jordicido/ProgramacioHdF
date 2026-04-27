# Ejercicios básicos de programación en Python

A continuación se presentan una serie de ejercicios básicos para practicar la sintaxis y las estructuras de control en Python. Estos ejercicios están diseñados para ayudarte a familiarizarte con el lenguaje y sus características fundamentales.

Para cada ejercicio, se debe escribir el código en un archivo `.py` y ejecutarlo en tu entorno de desarrollo. Para la entrega, comprime los archivos `.py` en un archivo ZIP y envíalo según las instrucciones del curso.

## Tabla de puntuación

| Ejercicios | Puntuación |
|------------|------------|
| 20         | 10         |
| 17         | 9          |
| 14         | 8          |
| 12         | 7          |
| 11         | 6          |
| 10         | 5          |
| <10        | 4, 3, 2, 1 |
|------------|------------|

## Ejercicios

### **1. Operaciones combinadas**

Pide tres números enteros y calcula:

* La suma de los dos primeros.
* El producto del segundo y el tercero.
* La diferencia entre el mayor y el menor de los tres.
  Muestra todos los resultados.

### **2. Calculadora simple**

Solicita dos números y una operación (+, -, *, /). Muestra el resultado según la operación indicada.

### **3. Par o impar**

Pide un número y determina si es par o impar utilizando `if`.

### **4. Clasificación según múltiplos (FizzBuzz básico)**

Pide un número entero y determina:

* Si es múltiplo de 3.
* Si es múltiplo de 5.
* Si es múltiplo de ambos.
  Usa operadores lógicos y condiciones compuestas.

### **5. Comparador de distancias**

Pide dos distancias en metros y analiza:

* Cuál es mayor.
* Si la diferencia supera los 10 metros.
* Si son prácticamente iguales (diferencia < 1 metro).

### **6. Mayor de tres números**

Introduce tres números y determina cuál es el mayor usando `if`, `elif`, `else`.

### **7. Calculadora de IMC**

Pide peso y altura, calcula el IMC y muestra la categoría: bajo peso, normal, sobrepeso u obesidad.

### **8. Año bisiesto**

Pide un año y determina si es bisiesto usando operadores lógicos:

```
(año % 4 == 0 and año % 100 != 0) or (año % 400 == 0)
```

### **9. Aprobado o suspenso**

Pide una nota y muestra si ha aprobado (>= 5) o suspendido.

### **10. Descuento en tienda**

Pide el precio inicial y aplica:

* 10% si supera 100€.
* 20% si supera 200€.
* Sin descuento en cualquier otro caso.

### **11. Comparación de cadenas**

Pide dos palabras y muestra si son iguales ignorando mayúsculas/minúsculas.

### **12. Validación de contraseña**

Comprueba si una contraseña:

* Tiene más de 8 caracteres.
* Contiene al menos un número.
  Usa operadores lógicos.

### **13. Clasificación de edad**

Según la edad introducida, muestra:

* Niño (<12)
* Adolescente (12–17)
* Adulto (18–64)
* Mayor (>=65)

### **14. Número dentro de un rango**

Pide un número y determina si está entre 1 y 100, ambos incluidos.

### **15. Divisibilidad**

Pide dos números y muestra si el primero es divisible por el segundo.

### **16. Comprobación de vocal**

Pide un carácter y determina si es una vocal usando:

```
if letra in "aeiouAEIOU":
```

### **17. Día de la semana**

Pide un número del 1 al 7 y muestra el día correspondiente. Si no es válido, muestra un mensaje de error.

### **18. Media de notas**

Pide 3 notas, calcula la media y clasifica:

* <5 → Suspenso
* 5–6.9 → Aprobado
* 7–8.9 → Notable
* 9–10 → Sobresaliente

### **19. Conversor de temperatura**

Pide una temperatura y el tipo de conversión (C→F o F→C). Calcula según la fórmula adecuada.

### **20. Validación de acceso**

Pide usuario y contraseña e indica si el acceso es permitido.
Usuario correcto: `"admin"`
Contraseña correcta: `"1234"`
Usa la condición `and`.
