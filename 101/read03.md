## 1. ¿Cuál es el propósito de CSS?

**El propósito de CSS es**:  
Dar estilo, separar contenidos y presentación, mejorar la experiencia de usuario, y facilitar el mantenimiento sin modificar el HTML.

---

## 2. ¿Qué analogía NO técnica usarías para explicar la responsabilidad de HTML vs. CSS?

El **HTML** es como la estructura de una casa, como las paredes, los cimientos y las habitaciones.  
En cambio, **CSS** es como la decoración y el diseño de interiores, incluyendo los colores de las paredes, los muebles y la iluminación, entre otros detalles.

---

## 3. ¿Cuáles son las tres formas de insertar CSS en tu proyecto?

Existen 3 formas:

**A. CSS en línea (Inline CSS)**, donde se agrega directamente en la etiqueta HTML utilizando el atributo `style`.

**B. CSS Interno (Internal CSS)**, donde se agrega dentro de la etiqueta `<head>` del documento HTML utilizando la etiqueta `<style>`.

**C. CSS Externo (External CSS)**, donde se crea un archivo separado con extensión `.css`, y este se enlaza al documento HTML mediante la etiqueta `<link>`. La etiqueta `<link>` va dentro de la etiqueta `<head></head>`.

Se recomienda utilizar **CSS Externo** ya que mejora la organización y mantenimiento, y facilita la reutilización de estilos en múltiples páginas.

---

## 4. Escribe un ejemplo de una regla CSS que daría texto rojo a todos los elementos `<p>`.

```css
p {
  color: red;
}
