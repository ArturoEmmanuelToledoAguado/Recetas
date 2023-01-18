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
