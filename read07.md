# Control de Versiones..
<br>
<div style="text-align: justify;">
•  ¿Qué es el control de versiones?

El control de versiones es un sistema que permite gestionar y registrar los cambios realizados en un proyecto a lo largo del tiempo. Facilita el seguimiento de las modificaciones, la colaboración entre varios desarrolladores, y la capacidad de volver a versiones anteriores en caso de errores. Los sistemas de control de versiones más comunes son Git, Subversion y Mercurial.
</div>
<br>
<div style="text-align: justify;">
•  ¿Qué es “clone” en Git?
El comando git clone en Git se utiliza para crear una copia local de un repositorio remoto. Cuando ejecutas este comando, descargas todos los archivos, el historial de commits, y las ramas de un repositorio desde un servidor (como GitHub, GitLab, etc.) a tu máquina local, permitiéndote trabajar en el proyecto.
</div>
<br>
<div style="text-align: justify;">
•  ¿Cuál es el comando para agregar los archivos modificados a la zona de preparación?
El comando para agregar archivos modificados a la zona de preparación (staging area) es:
git add <nombre_del_archivo>
Si deseas agregar todos los archivos modificados, puedes usar:
git add .
</div>
<br>
<div style="text-align: justify;">
•  ¿Cuál es el comando para enviar la captura de los archivos modificados a Github?
<br>
El proceso para enviar los cambios a GitHub consiste en varios pasos:
1.	Asegúrate de haber añadido los archivos modificados a la zona de preparación con:
  git add
<br>
2.	Haz un commit de los cambios:
git commit -m "Mensaje descriptivo"
<br>
4.	Finalmente, para enviar los cambios a GitHub, utiliza:
git push origin <nombre_de_la_rama>
<br>
Por ejemplo, si estás en la rama main, sería:
git push origin main
</div>

