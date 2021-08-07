# Git-GitHub-y-GitLab

Uso rápido de estás herramientas.
# 1 Introducción y Herramientas
## GIT
En primera instancia vamos al link: https://git-scm.com/ y descargamos Git.
Instalasmos Git y para saber si esta bien instalado corremos el siguiente comando desde el CMD

```CMD
git --version
```
![image](https://user-images.githubusercontent.com/86896526/128102083-8433bbef-100b-4d95-b1fb-4227d4d958e3.png)


Usaaremos Visual Studio Para poder manejar las versiones.

## GitHub
Posteriormente usaremos GitHub Desktop.

https://desktop.github.com/

Es una herramienta gráfica que ayudará ha tener el control de versiónes, pero tambien se puede desde linea de comando.

### Sourcetree
Una herramienta adicional es Sourcetree
https://www.sourcetreeapp.com/

Surf Street es una herramienta que nos permite ver de una manera más visual todo nuestro trabajo con
el kit, sobretodo en el tema de las ramificaciones de las diferentes branch de las diferentes ramas
que tengamos en nuestro código.

### GitKraken
Otro gestor de versiones parecido al anterior es GitKraken
https://www.gitkraken.com/

## Principales comandos
## Comenzamos Con lineade comando desde Git (tipo terminal linux)
1. Abrimos git
2. Nos pocicionamos en la carpeta donde trabajaremos ```cd d```
3. Creamos un nuevo directorio (carpeta) con el comando ```mkdir gitbasico```
4. Nos metemos dentro del nuevo directorio ```cd gitbasico.```
5. Creamos un archivo txt con:  ```touch file.txt```.
7. Para poder ver los archivos que hay en una capeta podemos usr ```ls```  número de ellos.
8. Para poder ver el listado de todos los archivos y los permisos que tienen es con ```ls -la``` y nos enlista el tipo de archivo.
9. Para poder abrir la carpeta desde el explorador de archivos => ```start .```  o ```explorer .```.

# 2 Entendiendo DevOps
## Entendiendo la arquitectura DevOps
### Fase 1

![image](https://user-images.githubusercontent.com/86896526/128108177-f3790d5e-4f8c-44a1-956c-7e7456fd03bd.png)

En  imagen se nos muestra como es recomendable que los proyectos se puedan compartir desde un repositorio para sque sea disponible toda la solución al equipo de desarrollo

### Fase 2 Gestor de dependencias
Cuando tenemos que usar el codigo de alguien más, muchas veces es necesario utilizar librerias que no teniamos previstas usualmente tomadas de internet, para eso sirve el Gestor de dependencias.

![image](https://user-images.githubusercontent.com/86896526/128108825-68939532-ab56-4a3e-99e6-2f67c559fbce.png)

Agregará la librería de terceros y cual versión se tiene que descargar.
Usaremos maven.

### Fase 3 Repositorio de Artefactos.
Este tipo de repocitorio sirve para alojar las librerias que no quieren que se difundan, estarpiasn de una forma local pero los desarrolladores del proyecto pueden ingresar

![image](https://user-images.githubusercontent.com/86896526/128109189-7ed849ca-383a-4bb4-b704-cf2fbc6a249d.png)

### Fase 4 Servidor de integración.
Jenkins es un servidor de automatización open source escrito en Java. Está basado en el proyecto Hudson y es, dependiendo de la visión, un fork del proyecto o simplemente un cambio de nombre.

Como servidor de automatización, Jenkins permite que una máquina realice numerosas tareas a las que los humanos destinamos demasiado tiempo en demasiadas ocasiones. ... Aunque podríamos hacer con él todo tipo de tareas automáticas, Jenkins se suele usar perfectamente como servidor de integración continua.

![image](https://user-images.githubusercontent.com/86896526/128261660-ec63f55c-f6cd-407e-bc91-57a0fd169d64.png)


### Fase 5 Testing  Test
- TDD es una práctica de desarrollo, enfocada en cómo escribir el código y cómo debería funcionar. 
-  Mientras que BDD es un enfoque de equipo que hace hincapié en por qué debes escribir ese código y cómo se debería comportar.

![image](https://user-images.githubusercontent.com/86896526/128262463-b91f8777-7a9e-4279-b2ee-36fa22fa4987.png)


### Fase 6 Calidad
Reglas de Calidad de nuestro código.

![image](https://user-images.githubusercontent.com/86896526/128263384-d7de72b5-e5b4-416f-83a0-cf46593deb07.png)

### Fase 7 Comunicación
Esta fase es importante ya qué se se intercambia información desde los colaboradores o los programas que se implantarón.

![image](https://user-images.githubusercontent.com/86896526/128263800-27e77dc6-ef46-4360-9f3f-54643296def4.png)

### Fase 8 Entornos
Uso de docker
Gestor de contenedores o entornos

![image](https://user-images.githubusercontent.com/86896526/128264275-99fc75b6-9977-4fcc-97b4-f8e3c75d245e.png)



 
