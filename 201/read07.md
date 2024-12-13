# Mis Notas de Lectura:

---

# Paradigmas de la programación 2

---

## 1. ¿Qué es la abstracción en programación y cómo se implementa utilizando objetos en JavaScript? Proporciona un ejemplo práctico.

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

---

## 2. ¿Cuáles son los cuatro pilares de la Programación Orientada a Objetos y cómo se aplican en JavaScript?

Los cuatro pilares de la **Programación Orientada a Objetos** (POO) son:

- **Abstracción:** Ocultar los detalles internos y mostrar solo lo esencial. En JavaScript, se logra mediante objetos y clases.
- **Encapsulamiento:** Agrupar datos y comportamientos que operan sobre esos datos dentro de una misma unidad, como una clase, y controlar el acceso a esos datos mediante métodos. Se puede aplicar usando propiedades privadas o protegidas y métodos públicos.
- **Herencia:** Permite que una clase herede características (propiedades y métodos) de otra clase. En JavaScript, se puede implementar mediante la palabra clave `extends` en clases.
- **Polimorfismo:** Permite que un objeto de una clase se comporte de diferentes maneras dependiendo del contexto. Se logra mediante la redefinición de métodos en clases derivadas.

## Ejemplo de cada pilar:

```javascript
class Animal {   // Clase base
  constructor(nombre) {
    this.nombre = nombre;
  }

  hablar() {
    console.log(`${this.nombre} hace un sonido.`);
  }
}

class Perro extends Animal {   // Herencia
  constructor(nombre) {
    super(nombre);  // Llamada al constructor de la clase padre
  }

  hablar() {
    console.log(`${this.nombre} ladra.`);
  }
}

class Gato extends Animal {   // Herencia
  constructor(nombre) {
    super(nombre);  // Llamada al constructor de la clase padre
  }

  hablar() {  // Polimorfismo
    console.log(`${this.nombre} maúlla.`);
  }
}

const perro = new Perro("Max");
perro.hablar();  // "Max ladra."

const gato = new Gato("Felix");
gato.hablar();  // "Felix maúlla."
```

---

## 3. ¿Cuál es la diferencia entre un objeto literal y una clase en JavaScript? ¿Cuándo deberías usar cada uno?

### Objeto literal:
Es una forma de crear objetos sin necesidad de usar clases. Es útil para definir un solo objeto con propiedades y métodos. Ideal para casos simples y cuando no se necesita reutilizar o extender el objeto.

## Ejemplo:

```javascript
const coche = {
  marca: "Toyota",
  modelo: "Corolla",
  arrancar() {
    console.log("El coche ha arrancado.");
  }
};

coche.arrancar();  // "El coche ha arrancado."
```

## Clase:
Es una plantilla para crear múltiples objetos con las mismas propiedades y métodos. Las clases son más útiles cuando necesitas crear varios objetos con la misma estructura y comportamientos, o cuando planeas extender funcionalidad con herencia.

## Ejemplo:

```javascript
class Coche {
  constructor(marca, modelo) {
    this.marca = marca;
    this.modelo = modelo;
  }

  arrancar() {
    console.log(`El coche ${this.marca} ${this.modelo} ha arrancado.`);
  }
}

const miCoche = new Coche("Toyota", "Corolla");
miCoche.arrancar();  // "El coche Toyota Corolla ha arrancado."
```

---

## 4. ¿Cómo implementarías la herencia en JavaScript utilizando clases? Proporciona un ejemplo que demuestre la relación padre-hijo entre dos clases.

En JavaScript, la herencia se implementa utilizando la palabra clave `extends`. Una clase hija puede heredar métodos y propiedades de una clase padre utilizando `super()` para llamar al constructor de la clase padre.

**Ejemplo de herencia:**

```javascript
class Animal {  // Clase padre
  constructor(nombre) {
    this.nombre = nombre;
  }

  comer() {
    console.log(`${this.nombre} está comiendo.`);
  }
}

class Perro extends Animal {  // Clase hija
  constructor(nombre, raza) {
    super(nombre);  // Llamada al constructor de la clase padre
    this.raza = raza;
  }

  ladrar() {
    console.log(`${this.nombre} está ladrando.`);
  }
}

const miPerro = new Perro("Rex", "Pastor Alemán");
miPerro.comer();  // "Rex está comiendo." (heredado de la clase Animal)
miPerro.ladrar();  // "Rex está ladrando." (propio de la clase Perro)
```






