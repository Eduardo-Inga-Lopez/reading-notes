# Mis Notas de Lectura:

# Estructuras de Control y Datos en JavaScript

## 1. ¿Cuáles son los diferentes tipos de estructuras condicionales en JavaScript y en qué situaciones deberías usar cada una?

JavaScript ofrece varios tipos de estructuras condicionales, cada una adecuada para situaciones específicas:

1. **`if` / `else if` / `else`**  
   - **Uso**: Para evaluar una o varias condiciones de forma secuencial.  
   - **Ejemplo**:  
     ```javascript
     let age = 18;
     if (age < 18) {
         console.log("Menor de edad");
     } else if (age === 18) {
         console.log("Recién cumplidos");
     } else {
         console.log("Mayor de edad");
     }
     ```

2. **`switch`**  
   - **Uso**: Para comparar un valor contra múltiples opciones específicas. Es útil cuando se manejan muchos casos predefinidos.  
   - **Ejemplo**:  
     ```javascript
     let day = "Monday";
     switch (day) {
         case "Monday":
             console.log("Inicio de la semana");
             break;
         case "Friday":
             console.log("Fin de la semana");
             break;
         default:
             console.log("Día normal");
     }
     ```

3. **Operador Ternario (`condition ? expr1 : expr2`)**  
   - **Uso**: Para evaluaciones cortas donde solo se necesitan dos resultados.  
   - **Ejemplo**:  
     ```javascript
     let isMember = true;
     let fee = isMember ? "$10" : "$20";
     console.log(fee);
     ```

---

## 2. En el contexto de arreglos en JavaScript, ¿cuál es la diferencia entre los métodos  `push()`, `unshift()`, y `splice()`, y cuándo usarías cada uno? 

1. **`push()`**  
   - **Función**: Agrega uno o más elementos al final del arreglo.  
   - **Uso**: Cuando necesitas insertar elementos al final del arreglo.  
   - **Ejemplo**:  
     ```javascript
     let arr = [1, 2, 3];
     arr.push(4); // [1, 2, 3, 4]
     ```

2. **`unshift()`**  
   - **Función**: Agrega uno o más elementos al inicio del arreglo.  
   - **Uso**: Para insertar elementos al principio del arreglo.  
   - **Ejemplo**:  
     ```javascript
     let arr = [2, 3, 4];
     arr.unshift(1); // [1, 2, 3, 4]
     ```

3. **`splice()`**  
   - **Función**: Agrega, elimina o reemplaza elementos en una posición específica.  
   - **Uso**: Para modificaciones específicas dentro del arreglo.  
   - **Ejemplo**:  
     ```javascript
     let arr = [1, 2, 4];
     arr.splice(2, 0, 3); // [1, 2, 3, 4]
     ```

---

## 3. ¿Qué diferencias existen entre los Bucles `for`, `while` y `do...while`? Proporciona un ejemplo práctico de uso para cada uno.

1. **`for`**  
   - **Uso**: Para iteraciones con un número conocido de repeticiones.  
   - **Ejemplo**:  
     ```javascript
     for (let i = 0; i < 5; i++) {
         console.log(i);
     }
     ```

2. **`while`**  
   - **Uso**: Para iteraciones que dependen de una condición.  
   - **Ejemplo**:  
     ```javascript
     let i = 0;
     while (i < 5) {
         console.log(i);
         i++;
     }
     ```

3. **`do...while`**  
   - **Uso**: Cuando necesitas que el bloque se ejecute al menos una vez antes de evaluar la condición.  
   - **Ejemplo**:  
     ```javascript
     let i = 0;
     do {
         console.log(i);
         i++;
     } while (i < 5);
     ```

---

## 4. ¿Cómo se puede recorrer un arreglo en JavaScript utilizando diferentes tipos de bucles y cuál consideras más eficiente según el caso de uso?

1. **Usando `for`**  
   - **Ejemplo**:  
     ```javascript
     let arr = [1, 2, 3];
     for (let i = 0; i < arr.length; i++) {
         console.log(arr[i]);
     }
     ```

2. **Usando `for...of`**  
   - **Ejemplo**:  
     ```javascript
     for (let item of arr) {
         console.log(item);
     }
     ```

3. **Usando `forEach()`**  
   - **Ejemplo**:  
     ```javascript
     arr.forEach(item => console.log(item));
     ```

4. **Usando `while`**  
   - **Ejemplo**:  
     ```javascript
     let i = 0;
     while (i < arr.length) {
         console.log(arr[i]);
         i++;
     }
     ```

5. **Usando `do...while`**  
   - **Ejemplo**:  
     ```javascript
     let i = 0;
     do {
         console.log(arr[i]);
         i++;
     } while (i < arr.length);
     ```

### Elección Más Eficiente
- **`for`**: Ideal para iteraciones con control total sobre el índice.  
- **`for...of`**: Excelente para simplicidad y legibilidad.  
- **`forEach()`**: Más funcional, pero no permite `break` o `continue`.  


