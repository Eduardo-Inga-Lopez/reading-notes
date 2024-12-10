# Mis Notas de Lectura:

---

# Paradigmas de la programación 1

---

## 1. ¿Qué es la Programación Funcional y cuáles son sus principales características?

La **programación funcional** es un paradigma de programación que se centra en el uso de funciones puras y en evitar cambios en el estado y datos mutables. Se basa en el concepto de "declarar qué hacer" en lugar de "cómo hacerlo".

### Principales características:
1. **Funciones Puras**: No tienen efectos secundarios y siempre producen el mismo resultado para los mismos argumentos.
2. **Inmutabilidad**: Evita modificar datos existentes; en su lugar, crea nuevas copias con los cambios necesarios.
3. **Primacía de las Funciones**: Las funciones se tratan como ciudadanos de primera clase, es decir, pueden ser asignadas a variables, pasadas como argumentos y devueltas por otras funciones.
4. **Composición de Funciones**: Permite combinar funciones simples para crear funcionalidades complejas.
5. **Declaratividad**: Se enfoca en el *qué* hacer en lugar del *cómo* hacerlo.

---

## 2. ¿Cómo aplicarías el principio DRY en un proyecto de JavaScript?

El **principio DRY (Don't Repeat Yourself)** busca evitar la duplicación de código al abstraer la lógica repetitiva en funciones reutilizables.

### Ejemplo práctico:

#### Antes de aplicar DRY:
```javascript
let calculateAreaRectangle = (length, width) => length * width;
console.log("Área del rectángulo:", calculateAreaRectangle(10, 5));

let calculateAreaTriangle = (base, height) => 0.5 * base * height;
console.log("Área del triángulo:", calculateAreaTriangle(10, 5));
```

```javascript
let calculateArea = (type, a, b) => {
    return type === "rectangle" ? a * b : 0.5 * a * b;
};
console.log("Área del rectángulo:", calculateArea("rectangle", 10, 5));
console.log("Área del triángulo:", calculateArea("triangle", 10, 5));
```

## 3. ¿Cuáles son las ventajas de utilizar métodos funcionales como map(), filter() y reduce()?

### Ventajas de Métodos Funcionales como `map()`, `filter()` y `reduce()`

1. **Legibilidad**: El código es más fácil de leer y entender, ya que describe la intención en lugar de los detalles.
2. **Concisión**: Se pueden realizar operaciones complejas en pocas líneas.
3. **Inmutabilidad**: Estos métodos no mutan el arreglo original; crean nuevos arreglos o valores.
4. **Composición**: Son ideales para combinar funciones y realizar transformaciones en pasos.

---

### Ejemplo:

#### Con un bucle tradicional:
```javascript
let numbers = [1, 2, 3, 4, 5];
let doubled = [];
for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % 2 === 0) {
        doubled.push(numbers[i] * 2);
    }
}
console.log(doubled); // [4, 8]
```

Usando filter() y map():

```javascript
let numbers = [1, 2, 3, 4, 5];
let doubled = numbers.filter(num => num % 2 === 0).map(num => num * 2);
console.log(doubled); // [4, 8]
```

## 4. ¿De qué manera el principio DRY y la programación funcional se complementan entre sí?

1. **Reutilización de Código**:  
   La programación funcional favorece la creación de funciones puras reutilizables, lo que reduce la duplicación de código (principio DRY).

2. **Modularidad**:  
   Al dividir la lógica en funciones pequeñas y específicas, el código es más fácil de mantener y escalar.

3. **Legibilidad y Escalabilidad**:  
   Ambos enfoques promueven un código más limpio, declarativo y fácil de entender, lo que facilita trabajar en proyectos grandes.

4. **Menor Propensión a Errores**:  
   Al evitar la duplicación y modificar datos de forma segura, disminuyen los errores en la lógica de negocio.

---

### Ejemplo combinando DRY y programación funcional:

```javascript
let calculate = (arr, condition, transform) => {
    return arr.filter(condition).map(transform);
};

let numbers = [1, 2, 3, 4, 5];
let result = calculate(numbers, num => num % 2 === 0, num => num * 2);
console.log(result); // [4, 8]
```



