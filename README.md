# Laboratorio-de-Git - Entrega del Módulo 1 de LemonCode

## 1. Crear un repositorio en local
<p>Para ello nos hemos situado en el escritorio con la terminal y hemos creado una carpeta por medio del comando mkdir con el nombre de "Laboratorio de Git". A continuación vamos a iniciar el repositorio de Git. Nos situamos en la carpeta creada con la terminal mediante "cd Laboratorio de Git" y dentro de ella invocamos el comando git init en la terminal.</p>

> mkdir y git init.

## 2. Subir el repositorio a GitHub
- <p>Hemos creado un repositorio en GitHub privado y con creación de README.md. Le hemos dado el nombre de "Laboratorio de Git".</p> 

- <p>Después hemos copiado el enlace y hemos conectado el repositorio local con el remoto por medio del comando git remote add origin <enlace>.</p> 

  > git remote add origin
>

## 3. Hacer un commit y un push
- <p>Primero hemos creado un archivo llamado index.html con de la terminal por medio del comando "touch index.html".</p> 

> touch index.html

- <p>Después hemos añadido el archivo al staging por medio del comando git add . y lo hemos commiteado con el comando git commmit -m "Creación archivo index.html". </p>

> - commit git add .
> - git commit -m "Creación archivo index.html

- <p>Para subir los cambios al repositorio de GitHub hemos usado el comando git push -u origin main</p>

> git push -u origin main

- <p>Sin embargo, hemos tenido un conflicto con el archivo README.md que hemos creado con GitHub, lógicamente es un archivo posterior a la creación del repositorio local, por lo que hemos tenido que hacer uso del comando git pull origin main para traernos los cambios del directorio remoto. Después sí que hemos podido realizar el push.</p>

> git pull original main

## 4. Crear una rama
- <p>Creamos a rama por medio del comando git brunch development.</p>

> git bruch development

- <p>Cambiamos de rama con el comando git swicht development.</p>

> git swicht development 

- <p>Escribimos el comando code . para abrir el proyecto en VSCode. Usando VSCode entramos dentro del archivo index.html y pulsamos la tecla ! seguido de tabulador, lo que nos va a mostrar la estrucutra básica de HTML.</p>

> - code .
> - !+TAB

- <p>Utilizando git add . subimos a staging el proyecto desde la rama development y hacemos git commit -m "Cambios en index.html".</p>

- <p>Ahora subimos los cambios a GitHub usando el comando git push origin development, lo que crea la nueva rama también en GitHub.</p>

>git push origin development

## 5. Hacer un merge 

- <p>Para realizar un merge cambiamos a la rama main por medio del comando git swicht main. Una vez en la rama main usamos el comando git merge development lo que nos permite fusionar los últimos cambios de la rama development en la rama main. En nuestro caso no existen conflictos, así que se produce la fusión.</p>

> git merge development 

- <p>El merge realiza un commit, por lo que nosotros no tenemos que hacerlo y podemos subir directamente los cambios a GitHub por medio de git push.</p>

> git push.

### Conclusiones finales
<p>Este ha sido todo el recorrido que he realizado para hacer la prática. Sí bien es cierto que no he realizado captruas mientras que lo hacía, así que no he podido incorporarlas. Espero que lo haya resumido claramente. Estaré muy agradecido si realizas cualquier corrección, aclaración o sugerencia para poder mejorar y aprender. Un saludo, David.</p>
