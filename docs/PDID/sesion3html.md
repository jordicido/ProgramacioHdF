# Práctica 3 - Imágenes y tablas

## Objetivo

- Aprender a insertar imágenes en una página web.
- Aprender a crear tablas para organizar información.

## Teoría mínima

Las imágenes en HTML se insertan con la etiqueta `<img>`. El atributo `src` se utiliza para especificar la URL de la imagen, y el atributo `alt` proporciona un texto alternativo que se muestra si la imagen no se carga. Por ejemplo:

```html
<img src="https://www.ejemplo.com/imagen.jpg" alt="Descripción de la imagen">
```

Se puede referenciar una imagen local usando una ruta relativa, por ejemplo:

```html
<img src="imagenes/foto.jpg" alt="Foto local">
```

Las tablas en HTML se crean con la etiqueta `<table>`. Dentro de una tabla, se utilizan `<tr>` para definir filas, `<th>` para definir celdas de encabezado y `<td>` para definir celdas de datos. Por ejemplo:

```html
<table>
    <tr>
        <th>Nombre</th>
        <th>Edad</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>25</td>
    </tr>
    <tr>
        <td>Luis</td>
        <td>30</td>
    </tr>
</table>
```

## Tarea 1

Añade a tu web:

- una imagen relacionada contigo o tus intereses
- atributo alt descriptivo

Condiciones:

- La imagen debe tener sentido con el contenido
- El texto alternativo debe explicar la imagen

Reto:

- Ajusta el tamaño de la imagen
- Colócala debajo de un título

## Tarea 2

Añade una tabla con al menos:

- 3 filas
- 3 columnas

Ideas:

- horario
- videojuegos
- deportes
- series

Condiciones:

- Debe incluir encabezados `<th>`
- Debe ser clara y legible
