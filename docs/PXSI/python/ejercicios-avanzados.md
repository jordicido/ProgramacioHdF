# **Ejercicio: Cálculo de cambio en billetes y monedas**

## **Enunciado**

Vas a programar un sistema que ayude a calcular el **cambio correcto** que debe devolverse a un cliente tras realizar una compra.

El programa debe pedir al usuario:

1. **El precio del producto** (en euros, puede tener decimales).
2. **La cantidad entregada por el cliente** (en euros).

---

## **Requisitos del programa**

### ** Validaciones iniciales**

* Si el precio o la cantidad entregada son **negativos**, el programa debe mostrar:

  > “Cantidad no válida”
* Si la cantidad entregada es **menor que el precio**, el programa debe mostrar:

  > “Dinero insuficiente”

---

### ** Cálculo del cambio**

* Si la cantidad entregada es **igual** al precio:

  > “No hay cambio”
* Si la cantidad entregada es **mayor**, se debe calcular el **cambio total** a devolver.

---

### ** Desglose del cambio**

El programa debe descomponer el cambio en el **menor número posible** de billetes y monedas.

Se deben utilizar las siguientes unidades:

**Billetes:**

* 50 €, 20 €, 10 €, 5 €

**Monedas:**

* 2 €, 1 €, 0,50 €, 0,20 €, 0,10 €, 0,05 €, 0,02 €, 0,01 €

---

### ** Condiciones de salida**

* Solo se deben mostrar los billetes o monedas que se utilizan.
* El resultado debe mostrarse de forma clara y ordenada, indicando cuántas unidades de cada tipo se devuelven.

---

## **Ejemplo de ejecución**

```
Introduce el precio del producto: 13.37
Introduce el dinero entregado: 20

Cambio a devolver: 6.63 €

Billetes:
5 € → 1

Monedas:
1 € → 1
0.50 € → 1
0.10 € → 1
0.02 € → 1
0.01 € → 1
```

---

## **Indicaciones importantes**

* No se permite el uso de listas ni bucles (solo variables y condicionales).
* Se debe evitar mostrar valores con errores de decimales.
* El programa debe ser legible y bien estructurado.

