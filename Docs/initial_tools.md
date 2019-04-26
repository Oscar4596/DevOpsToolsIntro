# Initial Tools

Para estar listos para empezar con lo básico, es menester tener ciertas herramientas para desarrollo básico.

### 0. Linux Subsystem for Windows
Para Windows 10 se desarrolló un *subsystem* de Linux para Windows, y se pueden descargar desde la misma tienda de Windows. Asegurate de estar en la última actualización de Windows e [instala el Subsystem](https://docs.microsoft.com/en-us/windows/wsl/install-win10).

#### Alternativas:
Emuladores de shell como:
* [Cygwin](https://www.cygwin.com/) 
* [Git bash](git.md#Instalar-Git)
* [Un virtualizador](#Un-virtualizador)

### 1. Un editor de texto:
Un buen editor de texto es imprecindible para cualquier tipo de desarrollo. Hay diversos editores gratuitos muy buenos, el que escojas depende de tus gustos, mis recomendaciones:
* [Visual Code](https://code.visualstudio.com/download)
* [IntelliJ](https://www.jetbrains.com/idea/download)
* [Atom](https://atom.io/)
Unos muy ligeros para edición rápida:
- [Sublime Text](https://www.sublimetext.com/3)
- [Notepad++](https://notepad-plus-plus.org/download/v7.6.6.html)

### 2. Una terminal o command prompt 

Aceptemoslo, la ventana de comandos de Windows es la cagada. Siempre es bueno tener una buena terminal para interactuar con muchas cosas. Una vez sepas manejar bien comandos y terminales no tocarás el explorador de windows. Mis recomendaciones:
* [Cmder](https://cmder.net/)
* [ConEmu](https://conemu.github.io/)

### 3. Un virtualizador

No puedes evitarlo, tienes que trabajar linux. Windows permite correr otros sistemas operativos en máquinas virtuales.
Un virtualizador gratuito por excelencia es [VirtualBox](https://www.virtualbox.org/), bastaría con conseguir la imágenes de los sistemas operativos, y tener los requerimientos de sistema para correrlo.
Sin embargo, hay una herramienta mucho más versátil para tener máquinas virtuales para correr pruebas, y crear entornos virtuales, y es [Vagrant](https://www.vagrantup.com/), es muy fácil de instalar y manejar y probablemente sea tu mejor amigo cuando quieras probar nuevas cosas sin mucho problema provisionando una máquina sin tener que instalar todo por tu cuenta, todo sobre como usarlo está en la [documentación](https://www.vagrantup.com/intro/index.html).

[Volver al índice](index.md)
