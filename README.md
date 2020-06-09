# init-repo

Documentando la creación y configuración de un repositorio, según https://guides.github.com/activities/hello-world/

# CONFIGURACIÓN CUANDO COMIENZO UN PROYECTO CON GIT - RESUMEN
# PASOS

1. Siempre al empezar un proyecto primero se debe inspeccionar los elementos:
por consola (terminal) ejecutar comando: ls

2. para ubicarse en la carpeta donde se trabajará el proyecto, ejecutar comando: cd rutaCarpeta, ejemplo: cd Documentos

3. Ejecutar comando: git --version , para conocer la versión de git instalada en la pc o si éste está instalado o no en la pc.

4. Configurar USUARIO/MAIL con los comandos:
   git config —global user.name “userName”
   git config —global user.email correoElectronicoAsociadoAGitHub@xxxx"
   
5. Para conocer la configuración que se tiene, ejecutar uno de los siguientes comandos:
  git config --global --list (lista configuracion global)
  git config --list (lista toda la configuracion del git incluyendo la local como global)

6. Ir a la web de github, para crear un nuevo repositorio en https://github.com  (seguir pasos de https://guides.github.com/activities/hello-world/)

7. Desde la carpeta del proyecto, por consola, ejecutar los siguientes comandos: 
    git init - (crea el repositorio en local que es un directorio .git que contiene todo el historial).
    git status - (para ver el estado en ese punto).
    git pull - (para bajar todo lo que se encuentre en el repo)
    
8. crear un Br (branch) para empezar a trabajar en el proyecto, con el comando
   git checkout -b nombreBranch (te permite crear el branch y cambiarte a éste).
   
9. Luego de tener todo el desarrollo y/o parte del mismo, subir los cambios al br de trabajo con los siguientes comandos
    
    git add nombreArchivo (para subir archivo por archivo) o git add . (para subir todos los archivos)
    
    git commit -m "mensajeDescriptivoDeDesarrollo"
    
    git pull 
      (para bajar la úlitma version de la rama y así evitar sobreescribir código existente y verificar si no hay conflictos, en que  hayan, se dede, solucionar).
      
    git push origin nombreBranch
    
10. Ir a la web de github, para crear el Pull Request (PR) de la rama de trabajo con la rama master. Con la finalidad de mezcla o fusionar tu código con lo que esté en la rama master.
    
   
