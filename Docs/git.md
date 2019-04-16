# Git & Git flow

Comencemos con lo más importante **¿Qué es Git?**

**Git** es una herramienta que permite el control de versiones; principalmente de código -aunque también de otras cosas, como este mismo texto-.

## Indice

- [Intro a Git](#Git)
- [¿Cómo funciona Git?]()
- [Instalar Git](#instalar-git)
- [Usar Git](#usar-git)

---

## Git

Git es importante porque permite llevar un control de todos los cambios que lleva un código, es como una base de datos de todas las versiones que ha llevado nuestro código; y es muy importante porque generalmente los proyectos involucran a más de una persona, y estas personas necesitan acceso al mismo código fuente, lo que lleva consigo muchas responsabilidades,

Para ejemplificar esto de manera sencilla, mostraré la siguiente situación:

*Dos amigos deciden empezar un proyecto sencillo, un blog sobre lo que aprenden en su clase de programación. Este blog está escrito en archivos de texto que se guardan en una carpeta compartida de Google Drive.
Un día, uno de los amigos, accidentalmente borra el archivo indice y ambos se quedan sin el archivo.
Bueno, no es mucho problema, el amigo que lo borró se pone a hacer un indice de nuevo, pero sin saber que el otro amigo también anda haciendo lo mismo, y ambos trabajan sobre el mismo archivo. Al guardar el trabajo de uno de los amigos se pierde ya que el otro sobreescribió el archivo*

Con ese ejemplo podemos ver las cosas con las que no tendríamos que lidiar si se maneja **Git**, ya que con git, se podría restaurar el archivo borrado, y ambos podrían trabajar sobre el mismo indice, teniendo versiones distintas, y digamos que ya no son solo 2 amigos sino que otras 7 personas se quieren unir al proyecto ¡Sería una locura manejar a tanta gente! 

## ¿Cómo funciona Git?

Básicamente, Git funciona de la siguiente manera:
![gitlocal](https://git-scm.com/figures/18333fig0106-tn.png)
Tenemos unos archivos locales, que a medida que vamos modificando, los vamos agregando a un *staging area*, cuando queremos que esos cambios que hemos hecho se guarden en una versión, hacemos un commit de esos archivos, y los guardamos en el repositorio.

#### Ver también: [What is git?](https://es.atlassian.com/git/tutorials/what-is-git)

## Instalar Git

Esto no tiene mucha ciencia, bien podrías googlearlo y encontrar un tutorial mejor que este, pero acá dejaré todo lo que necesitas para tener git instalado en tu máquina.

Primero, si no sabes si tienes git instalado o no, abre un terminal y ejecuta el siguiente comando, si te sale algo como lo que se muestra a continuación tienes git instalado:
```s
$ git --version
git version 2.19.0
```
Si no tienes git puedes seguir e instalarlo:
- [Windows](https://git-scm.com/download/win)
- [Mac OSX](https://git-scm.com/download/mac)
- [Linux/Unix](https://git-scm.com/download/linux)
Una vez lo hayas instalado, ejecuta este comando para confirmar la instalación, si se ve así todo bien, todo bien:
```s
$ git --version
git version 2.19.0
```

## Usar Git
Para empezar a usar git tenemos que tener un lugar en donde guardar nuestro código, hay varias páginas de repositorios, en lo personal recomiendo para empezar [GitHub](https://github.com/).

#### Algunos comandos básicos de Git

- `git config` - Configurar Git
- `git init` - Inicializar Git
- `git status` - Ver el estado del repositorio
- `git add` - Añadir archivos al próximo commit
- `git commit` - Hace commit de los archivos añadidos
- `git push` - Actualizar repositorio con los cambios realizados
- `git pull` - Descargar los cambios hechos en el repositorio

- Registrate y crea un nuevo repositorio:
![create repo](https://guides.github.com/activities/hello-world/create-new-repo.png)

- Una vez creado, clonemos e repositorio, copiando la URL del repositorio y corriendo ```git clone``` de la siguiente manera:

*Utilizaré un terminal shell que es el que viene por defecto en Mac OSX, en Windows recomiendo por el momento usar **Git bash** que viene con la instalación de Git.*

```
$ git clone https://github.com/tu-usuario/tu-repositorio.git
```

*Usaré unos comandos básicos de linux para la navegación, para más detalles ir a [Linux and Shell](linux.md)*
Por lo pronto...

#### Comandos básicos de linux

- `mkdir`   Make Directory - Crear un directorio (carpeta)
- `cd`      Change Directory – Cambiar de directorio
- `pwd`     Print Working Directory – Muestra el directorio en donde estás trabajando
- `ls`      List Directories – Muestra una lista de archivos y directorios

Entra a la carpeta del repositorio: 
```
$ cd tu-repositorio
```
Ahí verás un archivo README.md que es el que se creó cuando creaste el repositorio.

- Edita ese archivo y guarda los cambios.
- Añade el archivo al commit con `git add`:
```
$ git add README.md
```
o también, para añadir todos los archivos del repositorio
```
$ git add .
```
- Has el commit con un mensaje que discriba los cambios hecho
```
$ git commit -m "Añadidas algunas lineas al README.md"
```
- Guarda los cambios en el repositorio remoto
```
$ git push origin master
```
`origin` es el alias para el repositorio remoto, y `master` es la rama en la que estamos trabajando
- Es probable que se necesite configurar algunos parametros para poder hacer el *push* adecuadamente, para esto configura tu cuenta así:

        git config --global user.name "Firstname Lastname"
        git config --global user.email username@email.com

Con esto ya hemos creado un repositorio y añadido algunas cosas a él. 

Si se llegaran a hacer algunos cambios al repositorio los queremos tener en nuetra máquina local basta con correr
```
$ git pull
```
Para descargar los cambios.


# Enlaces externos

- [Getting started with git](https://www.taniarascia.com/getting-started-with-git/)
- [Git Book](https://git-scm.com/book/es/v2)
- [Tutoriales de Git](https://es.atlassian.com/git/tutorials)