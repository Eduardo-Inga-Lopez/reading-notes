# Mis Notas de Lectura:

# Introducción al DOM

## 1. ¿Qué es el DOM?

El DOM (Document Object Model) es una representación estructurada de un documento HTML o XML, organizada en una jerarquía de nodos que incluye elementos, atributos y texto. A través del DOM, los desarrolladores pueden acceder y manipular el contenido, estructura y estilo de una página web de manera dinámica.

## 2. Describe brevemente la relación entre el DOM y JavaScript.

JavaScript interactúa con el DOM para modificar de forma dinámica los elementos de una página web. Con JavaScript, podemos acceder a los nodos del DOM, cambiar su contenido, estilo o estructura, y responder a eventos del usuario (como clics o movimientos del ratón). Esta relación permite que una página web sea interactiva y pueda actualizarse sin necesidad de recargar la página.

## 3. ¿Qué método usarías para seleccionar un elemento del DOM por su ID y cómo se utiliza?

Para seleccionar un elemento por su ID, se usa el método `document.getElementById()`. Este método toma como argumento el ID del elemento que se desea seleccionar y devuelve una referencia a ese elemento.

**Ejemplo:**

```javascript
const elemento = document.getElementById("miElemento");

```

## 4. ¿Qué método utilizarías para cambiar el color de fondo de un elemento en el DOM y cómo se implementaría?
Para cambiar el color de fondo de un elemento, se utiliza la propiedad style.backgroundColor en JavaScript.

**Ejemplo:**

```javascript
const elemento = document.getElementById("miElemento");
elemento.style.backgroundColor = "blue";
```

En este ejemplo, el color de fondo del elemento con el ID miElemento cambiará a azul.
