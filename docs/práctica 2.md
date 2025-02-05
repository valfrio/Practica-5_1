# Segunda parte de la práctica

## Creación y actualización de un repositorio

### Ejercicio 1

#### Configurar Git definiendo el nombre del usuario, el correo electrónico y activar el coloreado de la salida.

Usamos los comandos de git config:

![1](includes/images/segunda%20parte/1.png)

### Ejercicio 2

#### Crear un repositorio nuevo con el nombre libro y mostrar su contenido.

Para crear un repositorio nuevo usamos el comando git init:

![2](includes/images/segunda%20parte/2.png)

### Ejercicio 3

#### Comprobar el estado del repositorio. Crear un fichero indice.txt con el siguiente contenido: Capítulo 1: Introducción a Git Capítulo 2: Flujo de trabajo básico Capítulo 3: Repositorios remotos. Comprobar de nuevo el estado del repositorio. Añadir el fichero a la zona de intercambio temporal. Volver a comprobar una vez más el estado del repositorio.

Usamos el comando git status para comprobar el estado del repositorio, git add para añadir el fichero a la zona de intercambio temporal y git status para comprobar de nuevo el estado del repositorio:

![3](includes/images/segunda%20parte/3.png)

### Ejercicio 4

#### Realizar un commit de los últimos cambios con el mensaje “Añadido índice del libro.” y ver el estado del repositorio.

Usamos el comando git commit -m "Añadido índice del libro." para realizar un commit de los últimos cambios y git status para ver el estado del repositorio:

![4](includes/images/segunda%20parte/4.png)

### Ejercicio 5

#### Cambiar el fichero indice.txt para que contenga lo siguiente: Capítulo 1: Introducción a Git Capítulo 2: Flujo de trabajo básico Capítulo 3: Gestión de ramas Capítulo 4: Repositorios remotos. Mostrar los cambios con respecto a la última versión guardada en el repositorio. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3 sobre gestión de ramas”.

Usamos el comando git diff para mostrar los cambios con respecto a la última versión guardada en el repositorio, git commit -m "Añadido capítulo 3 sobre gestión de ramas" para hacer un commit de los cambios y git status para ver el estado del repositorio:

![5](includes/images/segunda%20parte/5.png)

### Ejercicio 6

#### Mostrar los cambios de la última versión del repositorio con respecto a la anterior. Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.” Volver a mostrar los últimos cambios del repositorio.

Usaremos git show para mostrar los cambios de la última versión del repositorio con respecto a la anterior, git commit --amend -m "Añadido capítulo 3 sobre gestión de ramas al índice." para cambiar el mensaje del último commit y git show para volver a mostrar los últimos cambios del repositorio:

![6](includes/images/segunda%20parte/6.png)

## Ejercicios de manejo del historial de cambios

### Ejercicio 1

#### Mostrar el historial de cambios del repositorio. Crear la carpeta capitulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto: Git es un sistema de control de versiones ideado por Linus Torvalds. Añadir los cambios a la zona de intercambio temporal. Hacer un commit de los cambios con el mensaje “Añadido capítulo 1.” Volver a mostrar el historial de cambios del repositorio.

Usaremos el comando git log para mostrar el historial de cambios del repositorio con las opciones --oneline, --decorate --graph --all. Crearemos la carpeta capitulos y dentro de ella el fichero capitulo1.txt con el texto indicado, añadiremos los cambios a la zona de intercambio temporal y haremos un commit de los cambios con el mensaje "Añadido capítulo 1." y volveremos a mostrar el historial de cambios del repositorio:

![7](includes/images/segunda%20parte/7.png)

### Ejercicio 2

#### Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto: El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios. Añadir los cambios a la zona de intercambio temporal.Hacer un commit de los cambios con el mensaje “Añadido capítulo 2.” Mostrar las diferencias entre la última versión y dos versiones anteriores.

Crearemos el fichero capitulo2.txt en la carpeta capitulos con el texto indicado, añadiremos los cambios a la zona de intercambio temporal y haremos un commit de los cambios con el mensaje "Añadido capítulo 2." y mostraremos las diferencias entre la última versión y dos versiones anteriores con git diff;

![8](includes/images/segunda%20parte/8.png)

### Ejercicio 3

#### Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto: Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas. Añadir los cambios a la zona de intercambio temporal. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3.” Mostrar las diferencias entre la primera y la última versión del repositorio.

Crearemos el fichero capitulo3.txt en la carpeta capitulos con el texto indicado, añadiremos los cambios a la zona de intercambio temporal y haremos un commit de los cambios con el mensaje "Añadido capítulo 3." y mostraremos las diferencias entre la primera y la última versión del repositorio con git diff;

![9](includes/images/segunda%20parte/9.png)

### Ejercicio 4

#### Añadir al final del fichero indice.txt la siguiente línea: Capítulo 5: Conceptos avanzados. Añadir los cambios a la zona de intercambio temporal. Hacer un commit de los cambios con el mensaje “Añadido capítulo 5 al índice.”.Mostrar quién ha hecho cambios sobre el fichero indice.txt.

Añadiremos al final del fichero indice.txt la línea indicada, añadiremos los cambios a la zona de intercambio temporal y haremos un commit de los cambios con el mensaje "Añadido capítulo 5 al índice." y mostraremos quién ha hecho cambios sobre el fichero indice.txt con git blame;

![10](includes/images/segunda%20parte/10.png)

## Ejercicicos de deshacer cambios

### Ejercicio 1

#### Eliminar la última línea del fichero indice.txt y guardarlo. Comprobar el estado del repositorio. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero. Volver a comprobar el estado del repositorio.

Eliminaremos la última línea del fichero indice.txt y guardaremos los cambios, comprobaremos el estado del repositorio, desharemos los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero usando git restore y volveremos a comprobar el estado del repositorio:

![11](includes/images/segunda%20parte/11.png)

### Ejercicio 2

#### Eliminar la última línea del fichero indice.txt y guardarlo. Añadir los cambios a la zona de intercambio temporal. Comprobar de nuevo el estado del repositorio. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo. Comprobar de nuevo el estado del repositorio. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero. Volver a comprobar el estado del repositorio.

Eliminaremos la última línea del fichero indice.txt y guardaremos los cambios, añadiremos los cambios a la zona de intercambio temporal, comprobaremos de nuevo el estado del repositorio, quitaremos los cambios de la zona de intercambio temporal usando git restore --staged, pero los mantendremos en el directorio de trabajo, comprobaremos de nuevo el estado del repositorio, desharemos los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero con git restore y volveremos a comprobar el estado del repositorio:

![12](includes/images/segunda%20parte/12.png)

### Ejercicio 3

#### Eliminar la última línea del fichero indice.txt y guardarlo. Eliminar el fichero capitulos/capitulo3.txt. Añadir un fichero nuevo capitulos/capitulo4.txt vacío. Añadir los cambios a la zona de intercambio temporal. Comprobar de nuevo el estado del repositorio. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo. Comprobar de nuevo el estado del repositorio. Deshacer los cambios realizados para volver a la versión del repositorio. Volver a comprobar el estado del repositorio.

Eliminaremos la última línea del fichero indice.txt y guardaremos los cambios, eliminaremos el fichero capitulos/capitulo3.txt, añadiremos un fichero nuevo capitulos/capitulo4.txt vacío, añadiremos los cambios a la zona de intercambio temporal, comprobaremos de nuevo el estado del repositorio, quitaremos los cambios de la zona de intercambio temporal usando git restore --staged, pero los mantendremos en el directorio de trabajo, comprobaremos de nuevo el estado del repositorio, desharemos los cambios realizados para volver a la versión del repositorio con git restore y volveremos a comprobar el estado del repositorio:

![13](includes/images/segunda%20parte/13.png)

### Ejercicio 4

#### Eliminar la última línea del fichero indice.txt y guardarlo. Eliminar el fichero capitulos/capitulo3.txt. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Borrado accidental.” Comprobar el historial del repositorio. Deshacer el último commit pero mantener los cambios anteriores en el directorio de trabajo y la zona de intercambio temporal.Comprobar el historial y el estado del repositorio. Volver a hacer el commit con el mismo mensaje de antes. Deshacer el último commit y los cambios anteriores del directorio de trabajo volviendo a la versión anterior del repositorio. Comprobar de nuevo el historial y el estado del repositorio.

Eliminaremos la última línea del fichero indice.txt y guardaremos los cambios, eliminaremos el fichero capitulos/capitulo3.txt, añadiremos los cambios a la zona de intercambio temporal y haremos un commit con el mensaje "Borrado accidental.", comprobaremos el historial del repositorio, desharemos el último commit pero mantendremos los cambios anteriores en el directorio de trabajo y la zona de intercambio temporal con git reset --soft HEAD~1

![14](includes/images/segunda%20parte/14.png)

## Ejercicios de gestión de ramas

### Ejercicio 1

#### Crear una nueva rama bibliografia y mostrar las ramas del repositorio.

Crearemos una nueva rama bibliografia con el comando git branch bibliografia y mostraremos las ramas del repositorio con el comando git branch:

![15](includes/images/segunda%20parte/15.png)

### Ejercicio 2

#### Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.Añadir los cambios a la zona de intercambio temporal. Hacer un commit con el mensaje “Añadido capítulo 4.” Mostrar la historia del repositorio incluyendo todas las ramas.

Añado el archivo y hago el commit:

![16](includes/images/segunda%20parte/16.png)

### Ejercicio 3

#### Cambiar a la rama bibliografia. Crear el fichero bibliografia.txt y añadir la siguiente referencia: Chacon, S. and Straub, B. Pro Git. Apress. Añadir los cambios a la zona de intercambio temporal. Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.” Mostrar la historia del repositorio incluyendo todas las ramas.

Cambiamos a la rama bibliografia, creamos el archivo y hacemos el commit:

![17](includes/images/segunda%20parte/17.png)

### Ejercicio 4

#### Fusionar la rama bibliografia con la rama master. Mostrar la historia del repositorio incluyendo todas las ramas. Eliminar la rama bibliografia. Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.

Fusionamos la rama bibliografia con la rama main, mostramos la historia del repositorio incluyendo todas las ramas, eliminamos la rama bibliografia y mostramos de nuevo la historia del repositorio incluyendo todas las ramas:

![18](includes/images/segunda%20parte/18.png)

### Ejercicio 5

#### Crear la rama bibliografia. Cambiar a la rama bibliografia. Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias: Scott Chacon and Ben Straub. Pro Git. Apress. Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014). Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.” Cambiar a la rama master. Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias: Chacon, S. and Straub, B. Pro Git. Apress. Loeliger, J. and McCullough, M. Version control with Git. O’Reilly. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.” Fusionar la rama bibliografia con la rama master.Resolver el conflicto dejando el fichero bibliografia.txt con las referencias: Chacon, S. and Straub, B. Pro Git. Apress. Loeliger, J. and McCullough, M. Version control with Git. O’Reilly. Hodson, R. Ry’s Git Tutorial. Smashwords (2014). Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.” Mostrar la historia del repositorio incluyendo todas las ramas.

Creamos la rama bibliografia, cambiamos a la rama bibliografia, cambiamos el fichero bibliografia.txt para que contenga las referencias indicadas, añadimos los cambios a la zona de intercambio temporal y hacemos un commit con el mensaje "Añadida nueva referencia bibliográfica.", cambiamos a la rama main, cambiamos el fichero bibliografia.txt para que contenga las referencias indicadas, añadimos los cambios a la zona de intercambio temporal y hacemos un commit con el mensaje "Añadida nueva referencia bibliográfica.", fusionamos la rama bibliografia con la rama main, resolvemos el conflicto dejando el fichero bibliografia.txt con las referencias indicadas, añadimos los cambios a la zona de intercambio temporal y hacemos un commit con el mensaje "Resuelto conflicto de bibliografía." y mostramos la historia del repositorio incluyendo todas las ramas:

![19](includes/images/segunda%20parte/19.png)

## Ejercicios de repositorios remotos

### Ejercicio 1

#### Crear un nuevo repositorio público en GitHub con el nombre libro-git. Añadirlo al repositorio local del libro. Mostrar todos los repositorios remotos configurados.

Creamos un nuevo repositorio público en GitHub con el nombre libro-git, añadimos el repositorio remoto al repositorio local del libro con el comando git remote add origin:

![20](includes/images/segunda%20parte/20.png)

### Ejercicio 2

#### Añadir los cambios del repositorio local al repositorio remoto de GitHub. Acceder a GitHub y comprobar que se han subido los cambios mostrando el historial de versiones.

Añadimos los cambios del repositorio local al repositorio remoto de GitHub con el comando git push origin main y accedemos a GitHub para comprobar que se han subido los cambios mostrando el historial de versiones:

![21](includes/images/segunda%20parte/21.png)

![22](includes/images/segunda%20parte/22.png)

### Ejercicio 3

#### Colaborar en el repositorio remoto libro-git de otro usuario. Clonar su repositorio libro-git. Añadir el fichero autores.txt que contenga el nombre del usuario y su correo electrónico. Añadir los cambios a la zona de intercambio temporal. Hacer un commit con el mensaje “Añadido autor.” Subir los cambios al repositorio remoto.

Lo hacemos con el usuario de Jaime Grueso:

![23](includes/images/segunda%20parte/23.png)

### Ejercicio 4

#### Hacer una bifurcación del repositorio remoto asalber/libro-git en GitHub.Clonar el repositorio creado en la cuenta de GitHub del usuario. Crear una nueva rama autoria y activarla. Añadir el nombre del usuario y su correo al fichero autores.txt. Añadir los cambios a la zona de intercambio temporal. Hacer un commit con el mensaje “Añadido nuevo autor.” Subir los cambios de la rama autoria al repositorio remoto en GitHub. Hacer un Pull Request de los cambios en la rama autoria.

Hacemos el fork, actualizamos el repositorio local, creamos la rama autoria, añadimos el nombre del usuario y su correo al fichero autores.txt, añadimos los cambios a la zona de intercambio temporal, hacemos un commit con el mensaje "Añadido nuevo autor.", subimos los cambios de la rama autoria al repositorio remoto en GitHub y hacemos un Pull Request de los cambios en la rama autoria:

![25](includes/images/segunda%20parte/25.png)

![26](includes/images/segunda%20parte/26.png)

![27](includes/images/segunda%20parte/27.png)
