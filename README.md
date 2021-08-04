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
### Primera face

![image](https://user-images.githubusercontent.com/86896526/128108177-f3790d5e-4f8c-44a1-956c-7e7456fd03bd.png)

En  imagen se nos muestra como es recomendable que los proyectos se puedan compartir desde un repositorio para sque sea disponible toda la solución al equipo de desarrollo

### Segunda fase Gestor de dependencias
Cuando tenemos que usar el codigo de alguien más, muchas veces es necesario utilizar librerias que no teniamos previstas usualmente tomadas de internet, para eso sirve el Gestor de dependencias.

![image](https://user-images.githubusercontent.com/86896526/128108825-68939532-ab56-4a3e-99e6-2f67c559fbce.png)

Agregará la librería de terceros y cual versión se tiene que descargar.
Usaremos maven.

### Tercer Apartado Repositorio de Artefactos.
Este tipo de repocitorio sirve para alojar las librerias que no quieren que se difundan, estarpiasn de una forma local pero los desarrolladores del proyecto pueden ingresar

![image](https://user-images.githubusercontent.com/86896526/128109189-7ed849ca-383a-4bb4-b704-cf2fbc6a249d.png)

