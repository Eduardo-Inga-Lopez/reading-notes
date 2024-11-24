# Mis Notas de Lectura:

# Introducción a la Web Moderna

## 1. ¿Qué roles desempeñan los clientes y los servidores en el funcionamiento de la web?

### **Clientes**
- Son dispositivos (computadoras, teléfonos, tablets) que envían solicitudes para acceder a información o servicios en la web.
- Los navegadores web (como Chrome, Firefox o Safari) actúan como intermediarios para enviar estas solicitudes y mostrar la información recibida.
- **Ejemplo**: Al escribir una URL en el navegador, el cliente solicita los datos de esa dirección al servidor.

### **Servidores**
- Son computadoras remotas que almacenan y procesan la información solicitada por los clientes.
- Responden a las solicitudes del cliente enviando los recursos necesarios (páginas HTML, imágenes, videos, datos en JSON, etc.).
- **Ejemplo**: Un servidor web como Apache o Nginx entrega el contenido de un sitio web al cliente.

---

## 2. ¿Cómo se realiza la comunicación entre un navegador y un servidor al acceder a un sitio web?

### **El cliente inicia la solicitud**
1. El usuario ingresa una URL en el navegador.
2. El navegador traduce la URL en una dirección IP mediante el **DNS (Domain Name System)**.

### **Establecimiento de conexión**
- El navegador y el servidor establecen una conexión mediante el protocolo **TCP/IP**.
- Si el sitio usa HTTPS, se realiza un **handshake SSL/TLS** para establecer una conexión segura.

### **Envío de la solicitud HTTP/HTTPS**
- El navegador envía una solicitud HTTP (GET, POST, etc.) al servidor, especificando qué recurso necesita (p. ej., `index.html`).

### **Respuesta del servidor**
- El servidor procesa la solicitud y devuelve una respuesta HTTP con los recursos solicitados (HTML, CSS, JS, etc.).

### **Renderización en el navegador**
- El navegador interpreta el contenido recibido y renderiza la página web para el usuario.

---

## 3. ¿Cuáles son las principales ventajas de utilizar un IDE en la nube en comparación con un IDE local?

### **Accesibilidad desde cualquier lugar**
- Los IDE en la nube permiten trabajar en proyectos desde cualquier dispositivo con conexión a internet, eliminando la dependencia de una máquina específica.

### **Colaboración en tiempo real**
- Facilitan el trabajo en equipo mediante la colaboración simultánea en el mismo proyecto.

### **Configuración sencilla**
- No requieren instalación ni configuración compleja. Las herramientas están preconfiguradas y actualizadas en el entorno.

### **Escalabilidad**
- Pueden manejar proyectos de gran tamaño con menos impacto en los recursos del dispositivo del usuario.

### **Respaldo automático**
- Los proyectos suelen estar alojados en la nube, lo que garantiza copias de seguridad constantes.

---

## 4. ¿Qué funciones automatizadas comunes se encuentran en la mayoría de los IDE, y por qué son importantes para los desarrolladores?

### **Autocompletado de código**
- Sugiere y completa automáticamente fragmentos de código. Esto mejora la velocidad de escritura y reduce errores sintácticos.

### **Depuración integrada**
- Permite identificar y solucionar errores ejecutando el código paso a paso.

### **Resaltado de sintaxis**
- Destaca palabras clave, funciones y errores en el código para facilitar su lectura.

### **Refactorización**
- Ayuda a reorganizar y mejorar el código sin cambiar su funcionalidad, haciendo que sea más limpio y eficiente.

### **Control de versiones**
- Integración con herramientas como Git para gestionar cambios en el código de manera eficiente.

### **Compilación y ejecución automática**
- Compilan y ejecutan programas con un solo clic, ahorrando tiempo en tareas manuales.

### **Plantillas y snippets**
- Ofrecen estructuras predefinidas de código para tareas repetitivas.

