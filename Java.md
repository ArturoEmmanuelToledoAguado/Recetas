# Instalacion de Java en Ubuntu 

La instalacion de Java en ubuntu se puded hacer de diferentes 4 formas distintas según esta página 

  - https://help.ubuntu.com/community/Java

  Obtamos por la instalción  OpenJDK en la version 8

```console
sudo apt install openjdk-8-jdk
sudo apt install openjdk-8-jre
```

Si se tienen varias versiones se puede elegir cual utilizazr de acuerdo a
https://docs.datastax.com/en/jdk-install/doc/jdk-install/installOpenJdkDeb.html


# Instalación de IntelliJ IDEA

Se pude realizar desde _Ubuntu Software_

Se puede dedscargar el archivo desde la pagina https://www.jetbrains.com/es-es/idea/download/#section=linux

Si se decide por la Ultimate edition se puede pedir una beca con correo de una institucion eduativa. 


```console
sudo tar -zxvf ideaIU-2022.3.1.tar.gz -C /opt
cd /opt/idea-IU-223.8214.52/bin
./idea.sh
```

Para poder ejecutar Intellj desde la consola se tiene que hacer un enlace 

```console
sudo ln -s /opt/idea-IU-223.8214.52/bin/idea.sh /usr/local/bin/idea
```

## Tutoriales Java

- https://www.oracle.com/java/technologies/language-environment.html

- https://docs.oracle.com/javase/tutorial/index.html




## GITHUB

Trabajar en el mismo repositorio desde dos maquinas distintas

Ya se tiene el repositorio y se va a tabajare en una maquina adicional 

1. Clonamos 
- git clone repo <nombre_local>
2. Agregamos cambios
3. hacemeos push


Aqui faltaria agragar los permisos de la maquina 

1. PUede ser con tokens personalizados
2. Pude ser con un ky que generas localmente y depues lo cargas a tu cuenta de github

Tambien podemos almacenar las credenciales 




https://docs.github.com/es/authentication/keeping-your-account-and-data-secure/about-authentication-to-github

create a new repository on the command line
```
echo "# Recetas" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/rafneta/Recetas.git
git push -u origin main
```
or push an existing repository from the command line

```
git remote add origin https://github.com/rafneta/Recetas.git
git branch -M main
git push -u origin main
```


Evitar pedir credenciales una vez que que esto suceda 

https://www.freecodecamp.org/espanol/news/como-evitar-que-git-siempre-solicite-las-credenciales-de-usuario/

Lo mejor es hacer al conexión remota por ssh si iniciamelnte dfue por https entonces podemos cambair a ssh con la sigueinte instrucción 

```
git remote set-url origin git@github.com:username/repo.git¿
```
Podemos administrar las credenciales 
https://docs.github.com/es/get-started/getting-started-with-git/caching-your-github-credentials-in-git?platform=linux

1. Abrir una terminal (Control + Alt + T)
2. Tirar el siguiente comando:
   - git config --global credential.helper store
3. Asegurarse de estar parado en una carpeta que sea un repo cualquiera
Hacer un pull: (esto va a funcionar aunque no haya nada que pullear)
   - git pull

Luego de hacer el pull te pedirá tus credenciales (username y password) y estos datos serán guardados en un archivo en el disco (en la ubicación ~/.git-credentials). Esto quiere decir que no te los pedirá mas.

Pero la recomendacion es configurar una conexión ssh

https://docs.github.com/es/authentication/connecting-to-github-with-ssh

Aqui esta un prueba de primavera 2022

```
git config --global user.name "usuario"
git config --global user.email "correo.com"
git config --list
ls /al ~/.ssh
ls -al ~/.ssh
cd ~/.ssh
ssh-keygen -t ed25519 -C "correo"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519¿
cat ~/.ssh/id_ed25519.pub
```


# GITHUB

Establecer el bash como consola default

```
chsh -s /bin/bash

```

Para hacer de colores la terminal

1. download the zipped file from the Resources pane, or the bottom of this page
2. move the directory udacity-terminal-config to your home directory and name it .udacity-terminal-config (there's a dot at the front, now!)
3. move the bash_profile file to your home directory and name it .bash_profile (there's a dot at the front, now!)
   - if you already have a .bash_profile file in your home directory, transfer the content from the downloaded bash_profile to your existing .bash_profile

# Git Cursos

Git for authors https://pretextbook.org/gfa/html/frontmatter-1.html

Git with vscode https://code.visualstudio.com/docs/sourcecontrol/overview

Working with GitHub in VS Code https://code.visualstudio.com/docs/sourcecontrol/github#_github-repositories-extension

cursoso de microsoft https://learn.microsoft.com/en-us/training/paths/intro-to-vc-git/


# Consola cursos

Bash Guide https://guide.bash.academy/commands/#
Bash guide for Beginners https://tldp.org/LDP/Bash-Beginners-Guide/html/
Bash programming INtroduiction how to https://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO.html
Tranajar con expresiones regulares interactiva https://regexr.com/
Terminal cheatSheet MAc https://github.com/0nn0/terminal-mac-cheatsheet/tree/master/Espa%C3%B1ol
Linux command https://ss64.com/bash/

The linux command line for beginners (ubuntu) https://ubuntu.com/tutorials/command-line-for-beginners#1-overview

Pàgina de github con contenido curado https://learnbyexample.github.io/curated_resources/linux_cli_scripting.html



# Programación 

Introducción a la sínteis de porgramas 2022 Armando Solar-Lezama https://people.csail.mit.edu/asolar/SynthesisCourse/index.htm


Software contruction Armando Solar-Lezama https://web.mit.edu/6.031/www/sp19/

Understandong the world Through COde http://www.neurosymbolic.org/index.html

Create interactive content with PlaySkript https://code.playskript.com


Dynamnic Computer http://6.s081.scripts.mit.edu/sp18/schedule.html

# Machine learning

Practical machine learning  https://c.d2l.ai/stanford-cs329p/syllabus.html





