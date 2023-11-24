# Control de versiones
    Seguimiento 
        Nos permite entender
    Que     Porque Quien     Cuando
     De los cambios que realizamos

VCS version control system

Nos permite

    Conocer el historial de versiones
    Conocer el qué, porqué, cuándo y quién en cada versión.
    Ver los cambios realizados en cada versión.
    Restaurar versiones anteriores
    Trabajar en equipo

Se almacena en una carpeta llamada repositorio donde se almacena los archivos y BD con el historial de cambios de todos los archivos.

# Tipos de control de versiones
1.  Version Local: esta todo almacenada en nuestra PC.
    Cada version se llama pach tiene los cambios realizados.
2.  Centralizado: esta todo almacenado en un servidor.
    El historial de versiones esta en el servidor.
3.  Distribuido: cada miembro tiene una copia del repositorio.
    El historial se puede acceder desde la PC.

# GIT 
1.  es un VSC distribuido
2.  especialido en proyectos de software
3.  Gratuito
4.  Open Source 

## Áreas de GIT

1.  Área de trabajo: donde trabajamos el código
2.  Área de staging: cambios que estan listos para ser parte del repositorio 
3.  Área del repo: donde estan almacenados nuestros cambios.

## GitHub

Es donde almacenamos nuestro repositorios remotos, gestionar nuestros proyectos, etc.

## Comandos utiles:

    git config --global user.name "name"
    git config --global user.email "email"

el `--global` indica que sera la version por defecto para todo los repositorios que creemos.

## Nota: se puede cambiar el email o user ingresando al repositorio, y escribir el mismo comando pero sin el `--global`.

Para comprobar nuestras configuraciones:

    git config --list
    git config user.name
    git config user.email

Generar un nuevo repositorio.

    git init

Mover cambios del Área de Trabajo al Área de staging

    git add nameFile    un archivo
    git add *.js        todos los archivos con .js
    git add .           todos los archivos en el directorio actual
    git add -A          todos los archivos del proyecto
    git add -u          todos los archivos con modificados o eliminados no asi los nuevos.

Son los cambios que no queremos perder. Que luego decidiremos subirlos al repo remoto.

La operacion inversa, quitar los de staging al area del trabajo usaremos:

    git reset 

Mover del Área de staging al Área del repositorio

    git commit      Se abrir un editor de codigo propio de git, donde escribiremos la descripcion del commit

Luego al usar `git status` veremos que no hay nada en las Áreas de trabajo y staging.
Para revisar los commit usamos ``git log``

