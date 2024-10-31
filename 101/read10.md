## 1 **¿Qué es “Control Flow” (Control de Flujo)?**
  - El *Control de Flujo* en programación se refiere al orden en que se ejecutan las instrucciones de un programa. En JavaScript, el control de flujo se maneja a través de declaraciones como condiciones (`if`, `else`, `switch`), bucles (`for`, `while`), y otros bloques de control que determinan cómo y cuándo se ejecutan ciertas partes del código.

## 2 **¿Qué es una “function” (Función) de JavaScript?**
  - Una *función* en JavaScript es un bloque de código reutilizable que realiza una tarea específica o calcula un valor. Las funciones permiten organizar el código y evitar redundancias. Se definen con la palabra clave `function`, seguidas por un nombre, paréntesis y un bloque de instrucciones. Por ejemplo:
  
    ```javascript
    function greet(name) {
        return `Hello, ${name}!`;
    }
    ```

## 3 **¿Cuántas veces se ejecutará un bucle “while”?**
  - Un bucle `while` se ejecutará indefinidamente mientras la condición especificada sea verdadera. Si la condición inicial es falsa, el bucle no se ejecutará. Es importante asegurarse de que haya una manera de hacer que la condición se vuelva falsa en algún momento para evitar un *bucle infinito*.

## 4 **¿Qué método usarías para agregar un elemento al final de un array y cómo se utiliza?**
  - El método `push()` se utiliza para agregar un elemento al final de un array en JavaScript. Su uso es muy simple:
  
    ```javascript
    const fruits = ["apple", "banana"];
    fruits.push("orange");
    console.log(fruits); // ["apple", "banana", "orange"]
    ```
