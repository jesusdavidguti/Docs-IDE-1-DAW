# **Actividad 07. GIT. Secciones de un proyecto git. (2 Abril 2020)**

































































​								**Curso:** 1 DAW (19/20)

​								**Autor:** Jesús David Gutiérrez Delgado

​								**Asignatura:** IDE





​		**Índice**

[0. 	Introducción	3](#__RefHeading___Toc255_2896050065)

[1. 	Directorio de trabajo (Working directory)	4](#__RefHeading___Toc351_2719776763)

[2. 	Área de preparación (Staging area)	5](#__RefHeading___Toc353_2719776763)

[3. 	Repositorio (Directorio .git)	6](#__RefHeading___Toc355_2719776763)

















































































# **0.** **Introducción**

​	Git tiene tres estados principales en los que se pueden encontrar tus archivos: confirmado (committed), modificado (modified), y preparado (staged):

- **Confirmado**: significa que los datos están almacenados de manera segura en tu base de datos local.  
- ​	**Modificado**: significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos.  
- ​	**Preparado**: significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.

​	Esto nos lleva a las tres secciones principales de un proyecto de Git: 

​	El directorio de Git (Git directory), el directorio de trabajo (working directory), y el área de preparación (staging area).

​		![Working directory, staging area, and Git directory.](file:///C:/Users/Usuario/AppData/Local/Temp/lu8580266d42.tmp/lu8580266d6c_tmp_2b0bb5675658e760.png)


 

​	El **directorio de Git** es donde se almacenan los metadatos y la base de datos de objetos para tu proyecto. **Es la parte más importante de Git**, y es lo que se copia cuando clonas un repositorio desde otra computadora.

​	El **directorio de trabajo** es una copia de una versión del proyecto. Estos archivos se sacan de la base de datos comprimida en el directorio de Git, y se colocan en disco para que los puedas usar o modificar.

​	El **área de preparación** es un archivo, generalmente contenido en tu directorio de Git, que almacena información acerca de lo que va a ir en tu próxima confirmación. A veces se le denomina índice (“index”), pero se está convirtiendo en estándar el referirse a ella como el área de preparación.


 

El flujo de trabajo básico en Git es algo así:

1. ​	Modificas una serie de archivos en tu directorio de trabajo.
2. ​	Preparas los archivos, añadiéndolos a tu área de preparación.
3. ​	Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

​	Si una versión concreta de un archivo está en el directorio de Git, se considera confirmada (committed). Si ha sufrido cambios desde que se obtuvo del repositorio, pero ha sido añadida al área de preparación, está preparada (staged). Y si ha sufrido cambios desde que se obtuvo del repositorio, pero no se ha preparado, está modificada (modified).



































































# 1. Directorio de trabajo (Working directory)


 

​	El Directorio de trabajo (working directory) es un simple checkout de alguna versión del proyecto. Estos archivos son sacados de la base de datos que se encuentra en el GIT Directory y puestos a disposición nuestra para poder modificarlos y trabajar con ellos.

​	En lineas generales, el *Working Directory* es nuestra carpeta local en donde trabajamos y editamos los archivos. Puede tener el nombre que queramos y estar localizada en donde queramos de nuestro ordenador.

​	Al comenzar el proyecto tenemos que tener claro el tipo de proyecto que vamos a realizar, es decir, si vamos a acceder a el remotamente o si sólo vamos a trabajar en el de forma local (siempre en el mismo equipo).


 

# 2. Área de preparación (Staging area)


 

​	El Staging Area es el lugar donde vamos a ir añadiendo archivos cuando terminemos de editarlos. Es un paso intermedio, en el podemos ir añadiendo archivos hasta que queramos subirlos al repositorio. Por ejemplo, si hemos actualizado varios archivos relacionados pero no queremos subir otros, solo los seleccionados.

​	Las características más ventajosas de utilizar este área son las siguientes:

- Control y detección de cambios. Todos los archivos que vamos subiendo al staging area son susceptibles de poder verse los cambios que hemos realizado en ellos. Si hemos añadido lineas de código, esas lineas van a tener un símbolo + delante, si por el contrario hemos quitado lineas lo que veremos es el símbolo -.
- Es más eficiente. Hace un cacheo en los archivos antes de subirlos.
- Añadimos metadatos.


 


 


 


 


 


 


 


 


 


 


 


 

# 3. Repositorio (Directorio .git)


 

​	Un repositorio o “repo” es un directorio donde se almacenan los archivos de tu proyecto. Puede estar ubicado en el almacenamiento de *GitHub* o en un repositorio local en nuestro ordenador. Puede almacenar archivos de código, imágenes, audios o todo lo relacionado con el proyecto en el repositorio.

​	Cualquier carpeta de nuestro sistema puede ser un contenedor o repositorio para Git. Ahí se establecerá la configuración e historial bajo una carpeta nombrada .git que se encuentra oculta. No es necesario iniciar nuestro proyecto a la par que un repositorio. De hecho, estos se pueden crear aún cuando ya hemos avanzado con nuestro proyecto. Cada repositorio guarda un historial de los cambios realizamos en el.