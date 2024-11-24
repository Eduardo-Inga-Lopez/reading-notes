# Mis Notas de Lectura:

# HTML5 y CSS

## Porque es importante HTML5 y CSS?

Este tema es importante porque cubre los fundamentos esenciales del desarrollo web moderno, como el uso de HTML semántico, CSS para diseño responsivo y accesible, y las mejores prácticas en optimización para motores de búsqueda (SEO). Estos conceptos son cruciales para crear sitios web eficientes, bien estructurados y accesibles para una audiencia diversa, lo cual es clave en el mundo actual, donde la presencia en línea es esencial para cualquier negocio o proyecto.

En relación con mis estudios, estos conocimientos complementan y refuerzan las habilidades que estoy adquiriendo en el desarrollo de sistemas y aplicaciones web. Aprender a estructurar correctamente una página web, aplicar diseño responsivo, y optimizar para accesibilidad y SEO, me permitirá crear soluciones más efectivas y competitivas, mejorando la experiencia del usuario y asegurando que mis proyectos sean más visibles y funcionales en diversas plataformas y dispositivos.

---

### 1. Ventajas del uso de HTML semántico en comparación con el uso de etiquetas genéricas como `<div>`:
El uso de HTML semántico ofrece varias ventajas en comparación con las etiquetas genéricas como `<div>`:

- **Accesibilidad**: El HTML semántico mejora la accesibilidad web, ya que los navegadores y las tecnologías de asistencia (como lectores de pantalla) pueden interpretar mejor el contenido, lo que facilita la navegación para usuarios con discapacidades.

- **SEO (Optimización en motores de búsqueda)**: Las etiquetas semánticas ayudan a los motores de búsqueda a entender mejor la estructura del contenido, lo que puede mejorar la clasificación en los resultados de búsqueda.

- **Mantenibilidad**: Al utilizar etiquetas semánticas, el código es más fácil de leer y mantener, ya que las etiquetas proporcionan una idea clara sobre el propósito del contenido dentro de la página.

- **Mejor estructura y organización**: Las etiquetas semánticas permiten una organización clara del contenido, como encabezados, secciones y artículos, lo que facilita la comprensión del documento tanto para los desarrolladores como para los usuarios.

---

### 2. Etiquetas semánticas esenciales para estructurar correctamente una página web y su función:
Las siguientes etiquetas semánticas son esenciales para estructurar una página web correctamente:

- **`<header>`**: Define la cabecera de un documento o sección, generalmente incluye el logo, el título y la navegación principal.
  
- **`<nav>`**: Especifica un conjunto de enlaces de navegación dentro de un documento.
  
- **`<main>`**: Representa el contenido principal de un documento, excluyendo elementos repetitivos como encabezados, pies de página y barras laterales.
  
- **`<article>`**: Define un contenido autónomo e independiente que puede ser distribuido o reutilizado, como un blog o una entrada de noticias.
  
- **`<section>`**: Define una sección dentro de un documento, por lo general, tiene un encabezado y agrupa contenido relacionado.
  
- **`<footer>`**: Define el pie de página de un documento o sección, normalmente contiene información de contacto, derechos de autor o enlaces adicionales.

Estas etiquetas semánticas mejoran la accesibilidad, el SEO y la organización del contenido.

---

### 3. Función principal de las media queries en CSS y su contribución al diseño responsivo:
Las **media queries** en CSS permiten aplicar estilos CSS diferentes en función de las características del dispositivo, como el tamaño de la pantalla, la orientación (vertical u horizontal) o la resolución.

- **Contribución al diseño responsivo**: Las media queries permiten crear diseños que se adaptan a diferentes dispositivos, como teléfonos móviles, tabletas y pantallas de escritorio. Esto asegura que la página web se vea bien en cualquier tamaño de pantalla sin necesidad de reescribir completamente el diseño para cada dispositivo.

**Ejemplo básico de media query**:

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

---

### 4. Diferencias clave entre unidades absolutas y relativas en CSS y situaciones de uso:

- **Unidades absolutas**: Son unidades fijas que no cambian con respecto al contexto o tamaño de la pantalla. Las más comunes son:

  - **px (píxeles)**: Una unidad fija que define un tamaño exacto en píxeles.
  - **pt (puntos)**: Usado principalmente para impresión, donde 1 punto es igual a 1/72 de pulgada.
  - **in (pulgadas)**: Define tamaños basados en pulgadas.

  **Cuándo usar**: Las unidades absolutas son útiles cuando se necesita un tamaño específico e inmutable, como en la impresión o en casos donde no se requiere un diseño adaptable.

---

- **Unidades relativas**: Dependen de otro valor, como el tamaño de la fuente o el tamaño del contenedor padre. Las más comunes son:

  - **em**: Relativo al tamaño de la fuente del elemento padre. 1em es igual al tamaño de la fuente del elemento contenedor.
  - **rem**: Relativo al tamaño de la fuente raíz (generalmente el `html`).
  - **% (porcentaje)**: Relativo al tamaño del elemento contenedor.
  - **vw/vh (viewport width/height)**: Relativo al tamaño de la ventana de visualización (viewport).

  **Cuándo usar**: Las unidades relativas son ideales para diseño responsivo y adaptativo, ya que permiten que el diseño se ajuste dinámicamente al tamaño de la pantalla o al tamaño de la fuente.

---

## Cosas de las que quiero saber más

- Conceptos de **Diseño UX/UI**.
  

