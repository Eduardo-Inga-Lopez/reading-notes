# Mis Notas de Lectura:

# Introducción a Javascript

## 1. Tipos de Datos en JavaScript

En JavaScript, existen varios tipos de datos primitivos y complejos que permiten almacenar y manipular información. Los tipos principales incluyen:

- **String**: Representa texto. Se declara entre comillas simples (`' '`), dobles (`" "`), o backticks (`` ` ` ``). Ejemplo: `"Hola"` o `'JavaScript'`.
- **Number**: Incluye todos los números, tanto enteros como decimales. Ejemplo: `5`, `3.14`.
- **BigInt**: Para números enteros grandes que exceden el límite de `Number`. Ejemplo: `123n`.
- **Boolean**: Representa valores de verdad, `true` o `false`.
- **Undefined**: Un valor automático para variables no asignadas.
- **Null**: Representa un valor intencionalmente vacío.
- **Symbol**: Valor único, comúnmente usado como identificador único.
- **Object**: Un tipo complejo para almacenar colecciones de datos y entidades. Puede contener múltiples pares clave-valor, como `{ nombre: "Eduardo", edad: 51 }`.

## 2. Estructuras Condicionales `if` y `else`

Las estructuras condicionales `if` y `else` permiten ejecutar diferentes bloques de código según se cumpla o no una condición específica:

```javascript
let edad = 18;

if (edad >= 18) {
  console.log("Es mayor de edad.");
} else {
  console.log("Es menor de edad.");
}
```

## 3. Tipos de Operadores en JavaScript
JavaScript incluye varios tipos de operadores para realizar operaciones en las variables:

Aritméticos: Para operaciones matemáticas básicas. Ejemplos:

+ (suma): a + b
- (resta): a - b
* (multiplicación): a * b
/ (división): a / b
% (módulo): a % b (devuelve el residuo)
Asignación: Para asignar valores a las variables. Ejemplo: = o +=.

Comparación: Para comparar valores. Ejemplos: ==, !=, ===, !==, <, >.

Lógicos: Para operaciones lógicas, como && (AND), || (OR), y ! (NOT).

Tipo (typeof): Para verificar el tipo de datos. Ejemplo: typeof variable.

Los operadores aritméticos, como +, -, *, y /, son comunes para realizar cálculos matemáticos. Por ejemplo:

```javascript
let a = 5;
let b = 10;
let suma = a + b; // Resultado: 15
```
## 4. Declaración de Variables: var, let, y const
Las variables en JavaScript se declaran con var, let, o const, y cada uno tiene diferencias en cuanto a alcance y mutabilidad:

var: Tiene un alcance de función (no de bloque), y puede reasignarse y redeclararse. Ejemplo:

```javascript
var nombre = "Eduardo";
nombre = "Inga"; // Posible con `var`
```
let: Tiene un alcance de bloque (las {} en que se declara), puede reasignarse pero no redeclararse dentro del mismo bloque. Ejemplo:

```javascript
Copiar código
let edad = 51;
edad = 52; // Posible
```
const: También tiene un alcance de bloque, pero no puede ser reasignado ni redeclarado. Debe ser inicializado al declararse. Ideal para valores constantes:

```javascript
const PI = 3.1416;
```


