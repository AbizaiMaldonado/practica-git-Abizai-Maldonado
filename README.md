# Nombre completo: 
Abizai Gamaliel Maldonado Delgado

# Matrícula: 
2630472

# Nombre de la práctica

## Creación y sincronización de repositorios con Git y GitHub

# Objetivo de la práctica

El objetivo de esta práctica fue aprender a crear un repositorio local utilizando Git, conectarlo con un repositorio remoto en GitHub y comprobar que los cambios se pueden enviar y recibir entre la computadora y GitHub, de esta forma se pudo practicar el flujo de trabajo Local → GitHub y GitHub → Local,

# Descripción del procedimiento realizado

Primero se creó una carpeta llamada `practica-git-nombre-apellido`, dentro de esta carpeta se abrió PowerShell y se inicializó Git con `git init`, después se cambió el nombre de la rama principal a `main` y se crearon los archivos `README.md` y `datos.txt`, en el archivo `datos.txt` se agregó un texto inicial relacionado con la práctica,

Después se revisó el estado del repositorio con `git status`, se agregaron los archivos al área de preparación con `git add .` y se creó el primer commit con `git commit -m "Primer commit"`, después se creó en GitHub un repositorio público con el mismo nombre, sin agregar README, .gitignore ni licencia,

Luego se vinculó el repositorio local con el repositorio de GitHub usando `git remote add origin`, se comprobó la conexión con `git remote -v` y se enviaron los archivos a GitHub con `git push -u origin main`, al entrar al repositorio se comprobó que los archivos aparecieran correctamente,

Después se modificó el archivo `datos.txt` directamente desde GitHub, agregando la línea "Este archivo fue modificado desde GitHub", el cambio se guardó haciendo un commit desde GitHub, posteriormente se utilizó `git pull origin main` en PowerShell para descargar ese cambio a la computadora,

Finalmente se modificó nuevamente `datos.txt` desde la computadora, agregando la línea "Este archivo fue modificado desde el repositorio local", se revisó el estado, se agregaron los cambios, se creó un nuevo commit y se utilizó `git push` para enviar la modificación a GitHub, comprobando que el cambio apareciera correctamente en el repositorio,

# Comandos de Git utilizados

Los comandos utilizados durante la práctica fueron:

- `git init`
- `git branch -M main`
- `git status`
- `git add .`
- `git commit -m "Primer commit"`
- `git remote add origin URL_DEL_REPOSITORIO`
- `git remote -v`
- `git push -u origin main`
- `git pull origin main`
- `git push`

# Explicación breve de la función de cada comando

`git init` sirve para convertir una carpeta en un repositorio de Git, permitiendo que Git pueda controlar los cambios realizados en los archivos,

`git branch -M main` cambia el nombre de la rama principal a `main`, que es la rama utilizada en esta práctica,

`git status` muestra el estado actual del repositorio y permite ver qué archivos tienen cambios o cuáles están preparados para realizar un commit,

`git add .` agrega todos los archivos y cambios de la carpeta al área de preparación, dejando los cambios listos para guardarse en un commit,

`git commit` guarda los cambios preparados en el repositorio local, el mensaje que se escribe después de `-m` sirve para describir qué cambio se realizó,

`git remote add origin` conecta el repositorio local con el repositorio remoto de GitHub, `origin` es el nombre que se utiliza normalmente para identificar ese repositorio remoto,

`git remote -v` muestra los repositorios remotos que están conectados con el repositorio local y sus direcciones,

`git push` envía los commits del repositorio local al repositorio remoto de GitHub,

`git pull` descarga los cambios que existen en GitHub y los agrega al repositorio local, permitiendo mantener ambos repositorios sincronizados,

# Explicación de la practica

El repositorio local se creó dentro de una carpeta nueva llamada `practica-git-nombre-apellido`, después se abrió PowerShell dentro de esa carpeta y se utilizó el comando `git init`, con esto Git comenzó a controlar los archivos de la carpeta, después se cambió la rama principal a `main` y se crearon los archivos necesarios para la práctica,

|

Primero se creó en GitHub un repositorio público y vacío con el mismo nombre que el repositorio local, después se copió la URL del repositorio y se utilizó el comando `git remote add origin URL_DEL_REPOSITORIO`, con esto se estableció la conexión entre la carpeta local y el repositorio de GitHub, después se utilizó `git remote -v` para comprobar que la conexión se hubiera realizado correctamente,

|

Para enviar los cambios de la computadora a GitHub primero se agregaron los archivos con `git add .`, después se creó un commit para guardar los cambios en el repositorio local, finalmente se utilizó `git push -u origin main`, este comando envió los archivos y el commit a GitHub, después se comprobó desde la página del repositorio que los archivos estuvieran disponibles,

|

Para comprobar el flujo contrario se modificó el archivo `datos.txt` directamente desde GitHub y se agregó una nueva línea, después de guardar el cambio mediante un commit, se regresó a PowerShell y se utilizó `git pull origin main`, este comando descargó los cambios de GitHub al repositorio local, después se abrió el archivo `datos.txt` y se comprobó que el cambio también estuviera en la computadora,

|

El repositorio contiene principalmente dos archivos,

- `README.md`, contiene la información y documentación de la práctica, incluyendo el objetivo, procedimiento, comandos utilizados y la conclusión,

- `datos.txt`, contiene el texto utilizado para comprobar los cambios realizados desde GitHub y desde el repositorio local,

# Conclusión personal sobre lo aprendido

Con esta práctica aprendí de una forma más clara cómo funciona Git y cómo se puede utilizar junto con GitHub, aprendí que Git permite guardar los cambios de un proyecto mediante commits y que GitHub permite tener una copia del repositorio en internet, también aprendí a enviar cambios con `git push` y a recibir cambios con `git pull`,

Lo que más me ayudó fue comprobar las dos formas de sincronización, primero enviando cambios desde la computadora hacia GitHub y después haciendo un cambio en GitHub para descargarlo a la computadora, con esto pude entender mejor cómo se pueden mantener sincronizados un repositorio local y uno remoto,
