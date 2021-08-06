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


# 3. GIT
## ¿Cómo funciona?
En pocas palabras es un repositorio local. (tiene historial y versiones).

Cuando hagamos trabajos o estemos laborando hay tres tipos de aprtados:
1. WD - WorkingDirectori (directorio de trabajo local):aquí tendremos nuestros ficheros, carpetas y subcarpetas.
2. SA - Staing Area (Index): Es un lugar donde yo subo como si fuera un temporal, un entorno, un apartado, donde yo subo todos estos ficheros.
3. GR (Git Repository).

Al final, SA enlaza ambos. Wk y GR nunca se comunican.
Todo esto es dentro de un entorno local.

![image](https://user-images.githubusercontent.com/86896526/128265131-33053e65-fd08-401e-b565-3dd1de8feba3.png)

## Git Init
primero nos pocicionamos en el directorio que habiamos creado anteriormente de Git "gidbsasico".
posteriormente limpiamos la consola con el comando 

```CMD
clear
```
Inicializamos esta carpeta como un proyecto Git.

```CMD
git init
```
![image](https://user-images.githubusercontent.com/86896526/128265876-970db996-51af-44a3-b62d-c1e47d71e919.png)

Master siginifica Rama principal.

Observamos que dentro del directorio se nos ha creado un nuevo archivo llamado .git el cual es la configuración para poder usar el repocitorio.

##  Otros Comandos basicos 
### help
-- help sirve para ver el manual de algún comando
ejemplo: 
```CMD
touch --help
```

![image](https://user-images.githubusercontent.com/86896526/128266418-3f137df1-d929-4f85-aef7-4118a9d35c6c.png)

### Hacer un Fichero y colocarle información directamente
Damos el mensaje y decimos que se cree un nuevo archivo con el nombre
```CMD
echo "Hola mundo" > File3.txt
```
![image](https://user-images.githubusercontent.com/86896526/128266770-ebf8bbad-d036-4374-969c-96810186ffae.png)

### cat
sirve para leer un fichero  ```cat File3.txt```

![image](https://user-images.githubusercontent.com/86896526/128266982-cadc3ec4-a3fe-4652-9c4c-04fa7b8c6a7a.png)

### >> (Concatenar información)
Cuando ya tenesmo un archivo creado y queremos ingresar información.
En este caso el archivo esta vacío y le agregaremos info ```echo "Hola Segundo Mundo" >> file.txt``` ```cat file.txt```

![image](https://user-images.githubusercontent.com/86896526/128267196-afff294a-7043-4511-bb5f-3d5f09690a05.png)

En este segundo caso el archivo file3.txt ya tenia contenido, así que se le agregará.

![image](https://user-images.githubusercontent.com/86896526/128267432-6a831b2a-0830-4131-96b5-5641cb1c93fc.png)

### Editor de texto
Dento de git se nos puede permitir modificar el codigo (contenido de un fichero) dentro del pequeño editor nano
solo basta con escribir  ```nano file.txt``` y se nos habrira una pestaña con el archivo a editar.

![image](https://user-images.githubusercontent.com/86896526/128267816-fe7bae0d-fd45-4289-813c-e0125775cd34.png)

### Borra ficheros RM 
rm sirve para eliminar ficherossolamente
```rm file2.txt```
Como se ve solo queó el archivo 1 y 3: 
![image](https://user-images.githubusercontent.com/86896526/128268176-7e1b3c29-74c1-4e98-bca3-2728cd7cfc00.png)

Pero si nosotros quisieramos borrar algún directorio debemos de agregar -rf
- Creamos un directorio y eliminamos
```mkdir Carpetanueva```
```rm -rf Caprpetanueva```

![image](https://user-images.githubusercontent.com/86896526/128268481-6cacecb8-01fd-4447-beee-db0c28c35aff.png)

## Primer vistazo de Git
Para poder ver la carperta anteriormente mencionada llamada Git 
abriremos el explorador de archivos con ```explorer .``` y tendremos que activar "ver archivos ocultos".

![image](https://user-images.githubusercontent.com/86896526/128269468-8419d088-cd63-4b8c-bafc-8328d5cb09bc.png)

Para ingresar desde git tenemos que entrar como antes
```cd .git``` y ```cat config```  ```cat HEAD``` que nos dirá hacia donde apunta el directorio , que en este caso es a la rama master (main).

![image](https://user-images.githubusercontent.com/86896526/128269690-e2efac87-7376-472e-b29e-38e4b2887796.png)

Para volver a la raiz anterior usamos el comando ```cd ..```

## Git Object Types o Tipos de objetos
Hay 4 tipos de objetos
- blob: .java .js archivos o carpetas
- tree (arbol): referencia hacia los diferentes blobs
- Commit: objetos que almacena la subida del proyecto a nuestro git repocitory
- Annotated Tag (Etiquetas anotadas): lo usamos para referencia y no confundirnos en versiones.

### Blobs
Convertir la cadena en un objeto hash (hash-object) 
 ```echo "Hola mundo" | git hash-object --stdin```

![image](https://user-images.githubusercontent.com/86896526/128270575-a02faed8-e386-43fb-a982-e48e99cea97c.png)

Aun qué nosotros hayamos hecho el comando anterior y lo busquemos no estrará, porque nos faltara gregar un -w (write) y lo podrémos ver reflejao en la carpeta de object en una carpeta con las inicales del archivo antes cifrado.  ```echo "Hola mundo" | git hash-object --stdin -w```


![image](https://user-images.githubusercontent.com/86896526/128270694-75478a57-786b-4722-92db-ca9769fab7d3.png)

Dentro de esto se almacenara la información cifrada que hay dentro del fichero y no el nombre como tal.

Hasta que no cambien el contenido de la cadena y codigo de la cadena cifrada será la misma.

Hay otro tipo de cifrado: 
![image](https://user-images.githubusercontent.com/86896526/128271141-f836dbcf-1556-4065-a7a7-6379d3fd505f.png)

Cuando queremos ver el contenido del objeto utilizaremos el siguiente comando:
git cat-file -p "5 inicalies del codigo cifrado del obejto"
ejemplo:
 ```git cat-file -p 2d9b695c```

![image](https://user-images.githubusercontent.com/86896526/128272218-7b37903f-4f06-4414-a161-69fc2df4aed3.png)

Si nosotro queremos ver el tipo de Objeto tnemos que cambiar el comando de -p Por -t
ejemplo:
 ```git cat-file -t 2d9b695c```
 
![image](https://user-images.githubusercontent.com/86896526/128272352-87e809ad-451d-4437-a4dd-d87db7545605.png)

para el numero de bits, es con -s

Cuando hacemos un objeto y lo queremos eleiminar no lo eliminamos por completo, porque git asume que quieres el archivo para futuras proyectos o referencias.

* generación de Hashes.
Contenido de objeto
tipo de objeto (Objetc Type).
Longitud de objetos (Object Length).

![image](https://user-images.githubusercontent.com/86896526/128273230-143a1af5-10d0-475b-940a-2eaa198ded40.png)

### Trees
Arboles y Ramas
Se relaciones con los hash-object y almacenan el nombre del fichero.
Para poder ver todos los objetos que hay en el directorio de objects se utiliza este comando : 
 ``` find .git/objects/ -type f```
 
 ![image](https://user-images.githubusercontent.com/86896526/128273501-a4cc6be5-33f9-45f1-9f79-fd58883c207b.png)

* ejercicio
Nos proporcionan el siguiente codigo en un archivo de texto llamado "temp-tree.txt" el cual usaremos para agregar objetos desde aqui al fichero de objects.
Primero, movemos ese fichero a la carpeta principal.
segundo, leemos lo que hay.
Tercero creamos y leemos el árbol creado. , y REVISASMOS el formato, es importante decir que antes del nombre del archivo va una TAB
 
 
![image](https://user-images.githubusercontent.com/86896526/128275497-f49c221d-7a4c-4da0-a02f-414a9dba2d31.png)

Se creo el archivo en formato tree

Para poder visualizar el contenido (-p), el tipo (-t) y el tamaño (-s).
![image](https://user-images.githubusercontent.com/86896526/128275831-fd440290-64d2-4a71-9d89-e05fd401d444.png)

El arbol es un tipo de objeto y lo uqe hace es el codigo hashcon informacion de fichero diferente
para poder diferencia el tipo de archivo es usar el codigo que le easignemos:

![image](https://user-images.githubusercontent.com/86896526/128420047-3c41bc07-162c-423f-8225-a84563217e2b.png)

- trees y blobs
en esta sección vamos a pasar dos archivo sde git repository al working directory pero pasando primero por staging Area.

* Para podder pasar archivos del git repository a Stain Area usamos el comando 
 ```git read-tree [5 inicales  del Tree en hexadecimal]```
y luego los buscamos en la carpeta:
```git ls-files```

![image](https://user-images.githubusercontent.com/86896526/128421162-0eb315a4-b0f6-4f1f-8e82-dd7562016916.png)

Para pasar archivos desde el staning Area al Working Directory usamos lo siguiente:
```git checkout-index -a```
Y lo podemos visualizar que ya se ha psado con el siguiente comandos:
```ls -la```

![image](https://user-images.githubusercontent.com/86896526/128421988-892bcb1a-b81b-4e56-b061-21be4e0c3f3c.png)

![image](https://user-images.githubusercontent.com/86896526/128422033-94c1155e-7d01-4797-8140-a878918d0100.png)

Para oder visualizar el contenido de los ficheros podemos usar el comando
```cat [nombre de tu archivo txt]```


* Comando nuevo
```git status```
- primero no dice en que rama estamos
- si es que hay commits
- Menciona que si queremos eliminar los archivos del Staing Area para solo dejarlos en el Working Directory (desenlazarlos).
- (Untracking) Que no han(ficheros) pasado a la Staing Area y no podran pasar al Git Repository.

![image](https://user-images.githubusercontent.com/86896526/128422936-93eaf436-a0f7-422f-a806-5ae84d6f4b28.png)


Hacemos la prueba con el documento file2.txt y observamos que y no esta en el Staning area pero si en el Workind Directory.

![image](https://user-images.githubusercontent.com/86896526/128429741-bef173eb-a415-4fd1-8879-ca9160de21d3.png)
![image](https://user-images.githubusercontent.com/86896526/128429862-e6834823-5248-4f32-a94b-b6181bde8684.png)

Si lo queremos añadir de nuevo usamos el sigueiente comando:
```git ad file2.txt```
 y de nuevo usamos ```git status``` para observar que se volvio a subir a Staging Area:
 
![image](https://user-images.githubusercontent.com/86896526/128430039-ba997d8e-7e76-4cc3-9266-2b6da7bbdc05.png)


### Usuario en Git
Recomendación , hacer ususario con una cuenta que ya tengas en github
Puede ser enlazado con git hub, pero aún  asi es necesario configurarlo localmente
uso de comando:
Creamo un usuario con nombre y otro con un correo al final visualizamos 
un usuario global
 ```git config --global user.name "UlisesCortes" ``` 
 ```git config --global user.email "ulisesdeoz@gmail.com" ``` 
 ```git config --list ``` 

![image](https://user-images.githubusercontent.com/86896526/128431449-50d2e20d-1a87-4a43-b5a1-573fe62b0f1d.png)



### Commit
Pasaremos la infomacion que hay en Staging Area a GitRepository, esto no creará un nuevo tipon de objeto (commit9 que va atener un arbol enlacado directamente con sus blobs.
Dentro de este commit vamos a tener:
- Autor
- fecha
- comentario
- Tree

![image](https://user-images.githubusercontent.com/86896526/128431862-0d1bea78-e2a4-4576-97e5-da38c1f7ce2b.png)

Codigo de commit en Git Repository:
                   *comentario*
 ```git commit -m "mi primer commit" ```

![image](https://user-images.githubusercontent.com/86896526/128432226-b84a4419-93d3-433e-8931-c2c382cc8b70.png)

Para poder visualisar el tamaño el tipo y el contenido usamoe el comando:
Introducimos el codigo que nos dio el commit anterior
 ```git cat-file -t [codigo del commit] ```
 Aquí nos dirá la información del commmit
 
![image](https://user-images.githubusercontent.com/86896526/128432572-dce7399e-92e7-4b9b-ba9b-35c29d78f353.png)

Para comrpobar que hay un arbol dentro del comit utilizamos el codigo que viene del tree
![image](https://user-images.githubusercontent.com/86896526/128432804-a451c128-917f-4b41-ad70-b2f913e15d6e.png)


### Git Log
Es una delas herrameintas mas importantes, porque es un comando que nos permite ver todos lo commit que se han utilizado sobre la rama que estemos ejecutando.

![image](https://user-images.githubusercontent.com/86896526/128433733-933aedd2-0d85-41a4-bfab-a352e52fc258.png)

### Cilcos de vida del Commit

![image](https://user-images.githubusercontent.com/86896526/128434027-1fbcbb76-3808-4eb7-9df2-00b7fff269d7.png)

- Untracket: fichero que se encuentra en un  repositorio pero no se a subido (sincronizado con los otros).

### Enlaces entre Commit
Primero añadimos el file.txt a la rama de git Repocitory ```git add file.txt``` y lo visualizamos
con el comando ```git ls-file -s```

![image](https://user-images.githubusercontent.com/86896526/128434311-24f5324b-919e-48bb-b8c6-941433e631cd.png)

Añadimos un nuevo fichero llamado fer.txt
```echo "hola fer" > fer.txt```
```ls -la```

![image](https://user-images.githubusercontent.com/86896526/128434378-2af4ee62-716b-4ef7-9982-7a38d0569a46.png)

Tambien lo añadimos al Staging Area 
```git add fer.txt```

![image](https://user-images.githubusercontent.com/86896526/128435079-e54cb229-52c1-4212-8879-e9964f48bce3.png)
![image](https://user-images.githubusercontent.com/86896526/128435128-2d9bc474-912f-4eeb-99e5-6dcc8a528ce0.png)
![image](https://user-images.githubusercontent.com/86896526/128435141-7d3ee51a-f938-4d38-badd-597c8e310dc3.png)

Hacemos un segundo commit con los archivos anteriores
```git commit -m "nuestro segundo commit"```
![image](https://user-images.githubusercontent.com/86896526/128435230-1fbe5963-8c3d-4b32-9a87-41a6482595f0.png)

Para comprobar lo commmits usamos los el comando 
```git log``` y observamos que tenemos 2 cambios.

![image](https://user-images.githubusercontent.com/86896526/128435371-dfd6d129-1190-4bd6-b884-45c68e560998.png)
checamos el contenido delos commits
![image](https://user-images.githubusercontent.com/86896526/128436012-1a7f79ba-3b55-4293-95d0-efa4c5440467.png)

![image](https://user-images.githubusercontent.com/86896526/128436130-e1105343-70d6-4033-94b2-4ef86a61bf1f.png)


## Git Hub Desktop
añadimos el repocitorio de forma local
con add y local path

hicimos un tercer commit en changes
![image](https://user-images.githubusercontent.com/86896526/128436930-77633516-a7ca-459c-b2e1-d5d5aab817b8.png)

### Como volver a un commit desde comando bash
esta opción no es muy recomndable.
```git checkout 4fd2a881```
si yo quisiera hacer un cambio en un commit al final se eliminarian
ejemplo, cvamos a la segunda rama y agregamos nuevos ficheros y modificamos el archivo fer, pero al momento de pasar a la rama master no se guardaron ninguno de los cambios.

![image](https://user-images.githubusercontent.com/86896526/128437561-beb07755-0e7f-4f09-a3c8-9a304fcea29b.png)
![image](https://user-images.githubusercontent.com/86896526/128437594-84888d6b-2d99-4df7-9c73-710e4c1adee3.png)
![image](https://user-images.githubusercontent.com/86896526/128437611-a68f092e-83f5-40d7-a454-2e78eec47682.png)

Como vemos al final no se hizo ningun cambio.
![image](https://user-images.githubusercontent.com/86896526/128437645-7affaf4a-2b15-423c-a9f6-6f63aac35e19.png)

### HEAD
c1: commit 1
t1: tree 1
b1: blob 1

Se dió un a explicación acerca de lo que se hizo con la rama 2 y su eliminación, ademas se dio una breve aclaración de que podemos trabajar en ramas (C3) en paralelo para luego juntarlas. (c3 y c4 con c5)
![image](https://user-images.githubusercontent.com/86896526/128438160-905f24da-412c-4de5-a900-02190ad67ef3.png)

veremos hacia adonde apuntan la referencia, en este caso a master 
![image](https://user-images.githubusercontent.com/86896526/128438467-fe5f9794-08b4-4c64-9eb1-6a50f7ac1336.png)


### Creacion de ramas
Para poder visualizar las rams usamos el comando ```git branch``` y par hacerlas ```git branch [nombre de la rama]```

![image](https://user-images.githubusercontent.com/86896526/128438703-9d2b4f64-e4e0-4f9f-8f80-7119019bc5b3.png)

Para movernos entre las ramsa usamos el comando 
```git checkout br1```
![image](https://user-images.githubusercontent.com/86896526/128438789-df01f3f5-3097-41e1-9c4e-886cb4d216ef.png)

*nota* no podemos eliminar una rama en donde estemos.
Para poder eliminarla nos pasmaos a la rama master y luego dmos con el comando 
```git branch -d br1```
![image](https://user-images.githubusercontent.com/86896526/128439144-59098e96-b368-4382-9b08-e89afd644fb7.png)

Este comando te crea y switchea a una nueva rama.
```git branch -d br1```

si queremos modificar el nombre de la rma usamos el siguiente comando
primero el nombre de la rama y luego el nuevo nombre
```git branch -m br1 branch1```
![image](https://user-images.githubusercontent.com/86896526/128439890-62c3206b-8010-4942-99ec-d575cabf1882.png)

Ahora vamos a ver como unimos dos ramas como el diagrama anterior.
1. estamos en la Rama branch1
2. modificamos el fichero fer con ```echo "Hasta luego" >> fer.txt```
3. Añadimos al GitDirectory con ```git add .```
4. cehcamos como esta con ```git status```
5. Creamos un Commit dentro de la rams con ```git commit -m "Commit dentro de la rama"```
6. checamos que el commit se haya ejecutado correctamente. ```git log```
7. Nos cambianmos a la rama master  ```git checkout master"```
8. Revisamos de nuevo que esten los cambios  ```git log```vemos que los commits solo estaban en la rama anterior
9. y que el archivo fer.txt no se modificó
10. Para poder conectar ambas ramas se usa el siguiente codigo : ```git merge branch 1```
11. Revisamos el archivo fer.txt y vemos que el archivo si se combinó con el de la otra rama.
12. aparte los commit también.

![image](https://user-images.githubusercontent.com/86896526/128441373-5ece7e23-f0f0-4d91-ac37-e7154942dae6.png)

 



