# Programación en **Pseudocódigo**

## 1. ¿Qué es el pseudocódigo?

El pseudocódigo **no es un lenguaje de programación real**, sino una forma sencilla y estructurada de **explicar algoritmos** usando palabras cercanas al lenguaje humano.

Sirve para:

* Pensar soluciones antes de programar.
* Aprender lógica sin preocuparnos por la sintaxis exacta.
* Entender cómo funciona un programa paso a paso.

En pseudocódigo:

* No importa la sangría exacta, pero sí el orden.
* Se usan palabras clave como **INICIO**, **FIN**, **SI**, **MIENTRAS**, etc.
* El programa se ejecuta **de arriba hacia abajo**.

---

## 2. Entrada y salida de datos

### Mostrar información (SALIDA)

Para mostrar información por pantalla usamos la instrucción **MOSTRAR**.

**Ejemplos:**

```
MOSTRAR "Hola, mundo"
MOSTRAR "Estamos aprendiendo programación"
MOSTRAR 3 + 7
```

También podemos mostrar texto y valores juntos:

```
edad ← 18
MOSTRAR "La edad es ", edad
```

---

### Leer información (ENTRADA)

Para pedir datos al usuario usamos **LEER**.

**Ejemplo:**

```
LEER nombre
MOSTRAR nombre
```

Normalmente se combina mostrar un mensaje y leer el dato:

```
MOSTRAR "Introduce tu edad"
LEER edad
```

---

## 3. Comentarios

Los comentarios sirven para **explicar el algoritmo**, pero **no se ejecutan**.

Se suelen indicar con `//`.

**Ejemplo:**

```
// Esto es un comentario
MOSTRAR "Ejemplo de comentario"
```

Los comentarios ayudan a entender qué hace cada parte del algoritmo.

---

## 4. Variables y tipos básicos

Una **variable** es un espacio donde guardamos información que puede cambiar.

En pseudocódigo **no es necesario declarar el tipo**, solo asignar el valor.

**Ejemplos:**

```
edad ← 17
nombre ← "Laura"
precio ← 19.95
```

Tipos de datos más comunes:

| Tipo   | Ejemplo           | Uso                   |
| ------ | ----------------- | --------------------- |
| Entero | 10                | Números sin decimales |
| Real   | 3.14              | Números con decimales |
| Texto  | "Hola"            | Cadenas de texto      |
| Lógico | VERDADERO / FALSO | Condiciones           |

---

## 5. Operadores

### 5.1. Operadores aritméticos

| Operador | Significado          |
| -------- | -------------------- |
| +        | Suma                 |
| -        | Resta                |
| *        | Multiplicación       |
| /        | División             |
| MOD      | Resto de la división |
| ^        | Potencia             |

**Ejemplo:**

```
resultado ← 10 MOD 3
MOSTRAR resultado
```

---

### 5.2. Operadores de comparación

Sirven para comparar valores y devuelven **VERDADERO o FALSO**.

| Operador | Significado   |
| -------- | ------------- |
| =        | Igual         |
| ≠        | Distinto      |
| <        | Menor que     |
| ≤        | Menor o igual |
| >        | Mayor que     |
| ≥        | Mayor o igual |

**Ejemplo:**

```
edad ← 18
MOSTRAR edad ≥ 18
```

---

### 5.3. Operadores lógicos

Permiten combinar condiciones.

| Operador | Significado |
| -------- | ----------- |
| Y        | AND         |
| O        | OR          |
| NO       | NOT         |

**Ejemplos:**

```
edad ≥ 18 Y edad ≤ 65
edad < 0 O edad > 120
NO (edad < 0)
```

---

## 6. Condicionales

Las estructuras condicionales permiten **tomar decisiones**.

### 6.1. Condicional simple

```
SI condición ENTONCES
    instrucciones
SINO
    instrucciones
FIN_SI
```

**Ejemplo:**

```
MOSTRAR "Introduce tu edad"
LEER edad

SI edad ≥ 18 ENTONCES
    MOSTRAR "Eres mayor de edad"
SINO
    MOSTRAR "Eres menor de edad"
FIN_SI
```

---

### 6.2. Condicional con múltiples opciones

Se usa cuando hay **más de dos casos posibles**.

```
SI condición1 ENTONCES
    ...
SINO SI condición2 ENTONCES
    ...
SINO
    ...
FIN_SI
```

**Ejemplo:**

```
MOSTRAR "Introduce la nota"
LEER nota

SI nota < 5 ENTONCES
    MOSTRAR "Suspenso"
SINO SI nota < 7 ENTONCES
    MOSTRAR "Aprobado"
SINO SI nota < 9 ENTONCES
    MOSTRAR "Notable"
SINO
    MOSTRAR "Sobresaliente"
FIN_SI
```

👉 El programa evalúa **de arriba a abajo** y solo ejecuta el **primer bloque verdadero**.

---

### 6.3. Condiciones compuestas

Se pueden combinar varias condiciones usando operadores lógicos.

**Ejemplo:**

```
LEER edad

SI edad ≥ 18 Y edad ≤ 65 ENTONCES
    MOSTRAR "Eres adulto"
SINO
    MOSTRAR "No eres adulto"
FIN_SI
```

---

## 7. Bucles (repeticiones)

Los bucles permiten **repetir instrucciones** varias veces sin escribirlas de nuevo.

---

### 7.1. Bucle MIENTRAS

Se repite **mientras una condición sea verdadera**.

```
MIENTRAS condición HACER
    instrucciones
FIN_MIENTRAS
```

⚠️ La condición se evalúa **antes de cada repetición**.

**Ejemplo:**

```
contador ← 1

MIENTRAS contador ≤ 5 HACER
    MOSTRAR contador
    contador ← contador + 1
FIN_MIENTRAS
```

---

### 7.2. Ejemplos con MIENTRAS

**Ejemplo 1: pedir un número positivo**

```
LEER numero

MIENTRAS numero ≤ 0 HACER
    MOSTRAR "Error. Introduce un número positivo"
    LEER numero
FIN_MIENTRAS

MOSTRAR "Número correcto"
```

**Ejemplo 2: cuenta atrás**

```
cuenta ← 10

MIENTRAS cuenta > 0 HACER
    MOSTRAR cuenta
    cuenta ← cuenta - 1
FIN_MIENTRAS

MOSTRAR "¡Despegue!"
```
---

### 7.3. Bucle PARA

El bucle **PARA** se utiliza cuando sabemos **cuántas veces** queremos repetir un conjunto de instrucciones.

Es especialmente útil para:

* Contar números
* Recorrer rangos
* Tablas de multiplicar
* Repeticiones controladas

#### Estructura básica

```
PARA variable DESDE inicio HASTA fin HACER
    instrucciones
FIN_PARA
```

La variable:

* Comienza en el valor **inicio**
* Aumenta automáticamente de uno en uno
* El bucle termina cuando llega al valor **fin**

---

### 7.4. Ejemplo básico de PARA

Mostrar los números del 1 al 5:

```
PARA i DESDE 1 HASTA 5 HACER
    MOSTRAR i
FIN_PARA
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

### 7.5. Ejemplo práctico: tabla de multiplicar

```
MOSTRAR "Introduce un número"
LEER numero

PARA i DESDE 1 HASTA 10 HACER
    MOSTRAR numero, " x ", i, " = ", numero * i
FIN_PARA
```

---

### 7.6. Contar hacia atrás con PARA

```
PARA i DESDE 10 HASTA 1 HACER
    MOSTRAR i
FIN_PARA
```

---

### 7.7. PARA y MIENTRAS: ¿cuál usar?

| PARA                   | MIENTRAS                  |
| ---------------------- | ------------------------- |
| Repeticiones conocidas | Repeticiones desconocidas |
| Control automático     | Control manual            |
| Más sencillo           | Más flexible              |
| Evita bucles infinitos | Puede ser infinito        |

**Regla práctica para el alumnado:**

> Si sabes cuántas veces se repite → **PARA**
> Si no lo sabes → **MIENTRAS**

---

### 7.8. Bucles y condicionales combinados

Dentro de un bucle se pueden usar condicionales.

**Ejemplo: contar números pares del 1 al 10**

```
contador ← 0

PARA i DESDE 1 HASTA 10 HACER
    SI i MOD 2 = 0 ENTONCES
        contador ← contador + 1
    FIN_SI
FIN_PARA

MOSTRAR contador
```

---

### 7.9. Errores comunes con PARA

❌ Modificar manualmente la variable del bucle
❌ Confundir el valor inicial y final
❌ No entender cuántas veces se ejecuta
❌ Usar PARA cuando debería usarse MIENTRAS
