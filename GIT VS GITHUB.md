# Diferencias

 ## git
 - sistema de control de versiones distribuido.
 
 ## Github
 -servicio de repocitorio de hosting.
 
 ###Inside GITHUB
 podmos crear  nuestros repositorios dentro del apartado *repositories* y darle en "new"
 ![image](https://user-images.githubusercontent.com/86896526/128585588-79d21887-ebd4-4084-88b6-b9964fba8fad.png)
 
Creamos un pequeño repositorio con una licencia libre MIT
![image](https://user-images.githubusercontent.com/86896526/128585809-5175fc4a-6da5-4859-961a-c9085328b6ac.png)

- Drento de la pestaña Settings del Proyecto podermos ver que hay diferentes opciones, un de ella es hacer una plantilla a partir de otro proyectos.
- Dentro de la pestaña de manage acces podemos colocar el acceso al repocitorio,asi como quienes pueden editar con el nombre de usuario.
- Dentro de la misma pestaña de configuración hay más opciones para nuestro proyecto.

## Como clonar proyectos

Desde GitHub hasta Git:
Como es un proycecto libre y sin restricciones, podemos descargar el zip. Pero usaremos la liga que nos genera para bajarlo desde git con comandos.
con el comando ``git clone https://github.com/UlisesCortes/proyecto_git.git``

![image](https://user-images.githubusercontent.com/86896526/128586137-4ed7f3ea-c609-4fae-b338-080e07e53463.png)

Podemos ver que ya estamos en el main del proyecto
![image](https://user-images.githubusercontent.com/86896526/128586201-b9db68c4-c69f-412f-9c01-a7780d97d36c.png)


##Como crear ramas en gitn hub
Para eso vamos a la pagina del proyecto principal, habrá una pestalña con las ramas existentes, como solo tenemos una sola rama "main", procederemos a hacer una.
Se llamará "feature1" y la haremos dentro de la rama master.
![image](https://user-images.githubusercontent.com/86896526/128607504-b31eca60-cb92-46ec-9ac5-4b32657cb0ca.png)

Ahora nos aparece con dos ramas.
![image](https://user-images.githubusercontent.com/86896526/128607536-eddb3fdf-1954-4254-ae87-8d3fe342a056.png)

Dentro de esa opcion podemo visualiar las rams existentes con fecha y autor.

### Cambiar rama predeterminada
Primero ingresara Settings >> Branchs
![image](https://user-images.githubusercontent.com/86896526/128607671-8f63d17b-8648-4f2a-963a-c1c555641db9.png)

## Permisos
Podemos hacer reglas en las ramas con el apartado de Rules
![image](https://user-images.githubusercontent.com/86896526/128607722-7530bf22-6615-4219-8bb0-bec373e9e07b.png)

![image](https://user-images.githubusercontent.com/86896526/128607744-6a2e01e4-d028-4dc6-8bce-7037fe54cef2.png)

#Diagrama en general en como se relacionan con comandos
Denominamos ORIGIN al Repocitorio remoto

![image](https://user-images.githubusercontent.com/86896526/128608184-0167a1fd-0a90-46d2-9a96-ef2c72e16d22.png)

Podemos ver que es el origin con :```git remote```
Vemos que podemos hacer con este repsitorio con ```git remote -v```
- fetch : cuando queremos actualizar el repocitorio con lo que hay en el remoto
- push : acturalizar el proyecto remoto.
Vemos las ramas que hay localmente (como aun no hemos actualizado el repositorio solo muestra el "main") : ```git branch ```
Para ver solo las remotas usamos: ``git branch -r``
Para ver tanto locales como remotas: ``git branch -a``

![image](https://user-images.githubusercontent.com/86896526/128608410-19705878-1fa0-4f67-b572-418d53830369.png)
![image](https://user-images.githubusercontent.com/86896526/128608424-94e28333-e2d6-44ee-8d4f-43a24855e6da.png)

### Actualizar la rama
* con el comando : ``git fetch``
* Posterioremente nos switcheamos al al rama "feature": ``git checkout feature``
* Comprobamos que estamos hay con el comando: ``git branch``
* Comprobamos que los archivos tambien estan en la caperta con el comando: ``ls -la``
* chechamos que nuestro archivo anterio tambien conserva el contenido: ``cat featurebranch.txt``.

![image](https://user-images.githubusercontent.com/86896526/128608771-ae25e723-3c42-4a6b-b1ae-4ea4e9b484ca.png)
![image](https://user-images.githubusercontent.com/86896526/128608782-f5caf4d6-24d2-4601-9e8a-2c920b290986.png)
![image](https://user-images.githubusercontent.com/86896526/128608788-176b6280-d7b8-4c01-85a1-2b1b24021295.png)
![image](https://user-images.githubusercontent.com/86896526/128608792-814cfc1e-33b4-4d36-8166-b0a297c7e0e1.png)


### Motrar mas info del repos remoto
Usamos el comando : ``git remote show``
![image](https://user-images.githubusercontent.com/86896526/128609034-99368395-4305-47cc-b997-de27760cca55.png)

En la parte de (up to date) lo que nos quiere decir es que estan sinconizado el repocitorio local con el remoto.

-* Para el siguient ejemplo haremos un nuevo fichero en la rama feature
 Pdemos ver que ahora se nos cambia el mensaje de la rama feauture
 ![image](https://user-images.githubusercontent.com/86896526/128609171-92f42d17-0138-4f43-b698-5bad81a24e59.png)

Se agregó una nueva rama llamada feature2 y luego hicimos un git fetch para sincronizar los documentos.
Posteriormente hicimos un ``git pull`` para poder visualizar los ficheros faltantes al git Directory.

Tambien podemos utilizar el ``git pull -v`` para visualizar documentos y chechar que tosos se hayan pasado indicando que todo esta up to 

![image](https://user-images.githubusercontent.com/86896526/128609552-1741bb45-e551-4de1-8d48-e5dccaa51290.png)

### Apuntadores
Todas estas fetch y pull utilizan apuntadores de denode tomar la infomación, para entrar a esos apuntadores debemos acceder a la carpeta .git/res/remotes
![image](https://user-images.githubusercontent.com/86896526/128609707-a096965f-91ba-4efc-a614-846c29e6ebb8.png)

Temos locales y los remotos(GitHub)

##Git Push
Sube y actualiza lo que tenemos localmente al repocitorio remoto
``git push``

nos dice que necesitamos un permiso y que copiemos el codigo.
Nos abrirá una pestaña para aceptar.

![image](https://user-images.githubusercontent.com/86896526/128610286-05ea63f1-39cd-49da-9cf5-1443b076b51e.png)

# Usuario
Para cambiar el ususario.
![image](https://user-images.githubusercontent.com/86896526/128610474-b7f5f321-2b2d-4192-b74f-747f216e87a9.png)

## Agregar colaborador:
Settings\Manage access\\
nos abre un menú de quienes tienen acceso y si pueden modificar.
![image](https://user-images.githubusercontent.com/86896526/128610531-2dc12ed0-dd1e-4420-b00e-8897d0ca0ff5.png)

Como yo soy colaborador,me puedo dar permisos Directamente.

Podemos tener un pequeño chat con la persona (tambien la podemos ocultar)

#Pull Request
sirve para hacer una peticion alos colaboradores,
podemos hacer una nueva ramas
- hacemos un nuevo fichero pero lo guardaremos ccreando una nueva rama: nos dira que harémos un commit y comenzar un pull request
- ![image](https://user-images.githubusercontent.com/86896526/128610715-4ec0033f-ee51-4690-9e70-1855d81caadc.png)
![image](https://user-images.githubusercontent.com/86896526/128610755-59cc0f69-e742-445d-ba2f-817037a722d2.png)


# crear una rama en Git y subirla en GitHub
1. nos movemos al  main ``git checkout main``
2. Creamos la nueva rama ``git checkout -b feal3``
3. checamos que se haya creado ``git branch -a``
4. con el otro ``git branch -vv``
5. Hacemos un fichero dentro ``echo "Hola amigos" > filefeal3.txt``
6. Subimos el archivo a remote (origin) ``git push --set-upstream origin feal3``
7. Revismao que ya esta en carpetas de origin ``git branch -vv``
8. subimos el proyecto a GitHub: ``git fetch``

![image](https://user-images.githubusercontent.com/86896526/128611611-91817011-6ba9-4c8e-bb63-8e1ef8aea263.png)
![image](https://user-images.githubusercontent.com/86896526/128611618-f69e2b30-b844-4eb1-a663-f93d0d2edf87.png)
![image](https://user-images.githubusercontent.com/86896526/128611623-db070e9d-ef06-492e-9366-ebb019bd6907.png)
![image](https://user-images.githubusercontent.com/86896526/128611628-46aff626-1a14-4624-a1d0-2c7384d1c8f3.png)

Ahora podemos ver que en el navegador se refleja el cambio.(solo la Rama)
"flea3"
![image](https://user-images.githubusercontent.com/86896526/128611648-0db5fe83-0c16-4fc9-9cb8-3fda81652510.png)

## subir archivo de la rama:
1. para subir el archivo primero lo subimos al staging Area ``git add .``
2. luego hacemos un commit  ``git commit -m "flea3.txt subido"``
3. hacemos un push con un -v para que muestre mas info ``git push -v``
![image](https://user-images.githubusercontent.com/86896526/128611779-773afcad-b822-4353-b0d5-25f52a89b49e.png)

- Y ahora si ya aparece:

![image](https://user-images.githubusercontent.com/86896526/128611794-4f270ff0-1b53-4f64-9a1a-e03ed73b2663.png)

# creando y borrando una rama
## Creación
1. creamos una rama temporal y nos swichamos  ``git checkout -b temp``
2. checamos que se haya creado ``git branch -vv``
3. Hacemos una subida y trackeo en una misma linea ``git push -u origin temp``
4. Revisamos que ya esta en carpetas de origin ``git branch -vv``

![image](https://user-images.githubusercontent.com/86896526/128611886-74ac7d6c-a302-4962-a085-adfbbb712a65.png)
![image](https://user-images.githubusercontent.com/86896526/128611889-e1516a45-455d-456a-9702-6cd683d61cfe.png)
 
 Podemos ver que ya se subío
 ![image](https://user-images.githubusercontent.com/86896526/128611916-f417904d-c52f-46bb-8334-15bcd466b2ef.png)

## Borrado
ya que sabemos que rama borrar ahora hamos los siguientes comandos:

1.borramos desde el GitHub ``git push origin-d temp``
2. checamos que se haya creado ``git branch -vv`` // ahorra aparece gone en la rama lo que significa que ya no está.
![image](https://user-images.githubusercontent.com/86896526/128612001-958e067c-ba0f-4655-9a20-5c82962d98c8.png)

Ahora para borrarla de Git:
1. nos cambiamos a la rama main ``git checkout main``
2. eliminamos con este comando ``git branch -D temp``
![image](https://user-images.githubusercontent.com/86896526/128612027-2be6d273-e605-4597-8f08-1711d5f8fa82.png)

y vemos que ya no se encuentra:
![image](https://user-images.githubusercontent.com/86896526/128612052-39c23ae9-e5e8-4eac-8cf3-74eae58f6fae.png)

## ISSUES 
Estas survern para dejer una tarea por haceer en el proyecto, puede hacerlo cualquiera o asiganarlas. En pocas palabras son tareas que estan pendientes.

# Utilidades

## Historial
Se guarda durante 90 dias
Con el comando ``git reflog``
![image](https://user-images.githubusercontent.com/86896526/128612387-5be5dfe3-5afd-4228-a69c-fbb1fb21d8ae.png)

## Rebase 
Sobre escribir la rma que tengamos como defaul (susualmente Mastes/main) con otra rama.
podemos hacer esto con ``git rebase main``
Se puede usar la herrammienta de source tree para ver como se cambio
o con el comando directamente desde bash ``git log --graph``

Ejemplo práctico:
![image](https://user-images.githubusercontent.com/86896526/128612978-48c1865b-b4f0-440a-b594-a0ebc16bbd2c.png)

##Historial de commits
con los siguinetes ejemplos podemos ver distinta información

o si lo queremos el nombre de un solo autor
![image](https://user-images.githubusercontent.com/86896526/128613128-db3f7f01-19f0-4e39-aa4e-2324cafd5c77.png)


git log --author="UlisesCortes" --oneline
![image](https://user-images.githubusercontent.com/86896526/128613160-4066263d-4811-492c-a4d5-7694e41ce1d5.png)

Ver todos los merges
git log --merges --oneline


## git Resets
resetear a un estado anterior a donde estabamos.

![image](https://user-images.githubusercontent.com/86896526/128613324-392613dc-1ac8-463f-9854-359143b2c1f4.png)

git reset --mixed
git reset --hard
git reset --soft
lo podemos ver desde git status

## Cambios en la información de commit
Par esto esse tiene que tener un commit.
vamos a ver como cambiar puede ser el mensaje, el autor, etc.
``gut comiit "los nombre, email y lo demas"``

## Git Cherry Pick
replicar un commit en la rama master
se crea un nuevo cherry
``git cherry-pick [hexadecimal del commit]``

# Git Stash
es lo que tenemos guardado en el Staing Area
``git stash``
guarda una referencia en como esta el Staging Area

# Git GC (Garbage Colector)
Recolector de basura, limpia las cosas que ya no sean utiles, para no tener tanta basura en el proyecto
``git gc``

# Squashing
"lo hace en GitHub"
Cuando hacemos un nuevo fichero con rama y vamos al pull request
![image](https://user-images.githubusercontent.com/86896526/128614011-1fd7e309-d932-4990-aaef-6fb6273763ad.png)

El Squashing sirve para combinar los commits para una branch


# ENLACES VARIOS
- semantic - para etiquetas
- gitignore.io - Para el archivo gitignore pero con diferentes lenguajes
- Source tree - Administrador visual
- git Hooks- filtro de interseccion para lansar diferentes mensajes cuando pase alfo
- pre-commit - freamwork para usar antes de hacer commit
- git flow - Revisiones para git
- GitHub Pages- subir un codigo html para hacer una pagina 
* - Cucumber

# End Game
