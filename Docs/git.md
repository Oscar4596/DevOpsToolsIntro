# Git & Git flow

Comencemos con lo más importante **¿Qué es Git?**

**Git** es una herramienta que permite el control de versiones; principalmente de código -aunque también de otras cosas, como este mismo texto-.

## Indice

- [Intro to git](#Git)
- [Instalar Git](#Instalargit)

---

## Git

Git es importante porque permite llevar un control de todos los cambios que lleva un código, es como una base de datos de todas las versiones que ha llevado nuestro código; y es muy importante porque generalmente los proyectos involucran a más de una persona, y estas personas necesitan acceso al mismo código fuente, lo que lleva consigo muchas responsabilidades,

Para ejemplificar esto de manera sencilla, mostraré la siguiente situación:

*Dos amigos deciden empezar un proyecto sencillo, un blog sobre lo que aprenden en su clase de programación. Este blog está escrito en archivos de texto que se guardan en una carpeta compartida de Google Drive.
Un día, uno de los amigos, accidentalmente borra el archivo indice y ambos se quedan sin el archivo.
Bueno, no es mucho problema, el amigo que lo borró se pone a hacer un indice de nuevo, pero sin saber que el otro amigo también anda haciendo lo mismo, y ambos trabajan sobre el mismo archivo. Al guardar el trabajo de uno de los amigos se pierde ya que el otro sobreescribió el archivo*

Con ese ejemplo podemos ver las cosas con las que no tendríamos que lidiar si se maneja **Git**, ya que con git, se podría restaurar el archivo borrado, y ambos podrían trabajar sobre el mismo indice, teniendo versiones distintas, y digamos que ya no son solo 2 amigos sino que otras 7 personas se quieren unir al proyecto ¡Sería una locura manejar a tanta gente! 

#### Ver también: [What is git?](https://es.atlassian.com/git/tutorials/what-is-git)

## Instalar Git

Esto no tiene mucha ciencia, bien podrías googlearlo y encontrar un tutorial mejor que este, pero acá dejaré todo lo que necesitas para tener git instalado en tu máquina.

Primero, si no sabes si tienes git instalado o no, abre un terminal y ejecuta el siguiente comando, si te sale algo como lo que se muestra a continuación tienes git instalado:
```s
$ git --version
git version 2.19.0
```

