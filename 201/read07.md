### 1. ¿Qué es la abstracción en programación y cómo se implementa utilizando objetos en JavaScript? Proporciona un ejemplo práctico.

La **abstracción** en programación es el proceso de ocultar los detalles complejos de un sistema y mostrar solo las funcionalidades esenciales. En otras palabras, permite que los usuarios interactúen con un sistema sin necesidad de comprender todos los detalles internos. En JavaScript, la abstracción se puede lograr utilizando objetos y métodos que encapsulan detalles internos.

**Ejemplo práctico:**

```javascript
class Coche {
  constructor(marca, modelo) {
    this.marca = marca;
    this.modelo = modelo;
  }

  arrancar() {
    console.log(`El coche ${this.marca} ${this.modelo} ha arrancado.`);
  }

  detener() {
    console.log(`El coche ${this.marca} ${this.modelo} se ha detenido.`);
  }
}

// Aquí estamos abstraiendo el funcionamiento interno del coche
const miCoche = new Coche("Toyota", "Corolla");
miCoche.arrancar();  // No es necesario saber cómo funciona internamente
miCoche.detener();   // Solo interactuamos con los métodos públicos
```

