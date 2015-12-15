## Repositorio ejercicios Data Science Toolkit

#### 2.1 Repositorio campusciff (I)

Creo el repositorio en GitHub a través de la opción de menú “New repository”. El nombre es "campusciff" y como descripción "Repositorio ejercicios Data Science Toolkit".

#### 2.2 Repositorio campusciff (II)

Me sitúo en el directorio local donde quiero clonar el repositorio remoto y ejecuto el comando:
	
	git clone git@github.com:davpacheco/campusciff.git

#### 2.3 Readme

No es necesario crearlo en el repositorio local porque se generó inicialmente en el repositorio remoto y al clonarlo lo tengo también en local.

#### 2.4 Commit inicial

	git add .
	git commit -m “commvi it inicial”

#### 2.5 Push inicial

	git push origin

#### 2.6 Ignorar archivos (I)

Creo en el directorio local el archivo "privado.txt" y el directorio "privada":

    touch privado.txt
	mkdir privada

#### 2.7 Ignorar archivos (II)

Creo el archivo .gitignore:

	touch .gitignore

A continuación lo edito para introducir el archivo y la carpeta que quiero que git ignore. Utilizo vi:

	vi .gitignore
    
	<pulso tecla “i”>
	<escribo en la primera línea: privado.txt>
	<escribo en la segunda línea: privada>
	<pulso tecla “esc”>
	<escribo para guardar el archivo con los cambios :wq>

#### 2.8 Añadir fichero 1.txt

	touch 1.txt
	git add .
	git commit -m “añado fichero 1.txt”

#### 2.9 Crear el tag V0.1

	git tag v0.1

#### 2.10 Subir el tag v0.1

	git push origin master

#### 2.11 Crear una rama

Creo la rama y me posciono:

	git branch v0.2
	git checkout v0.2


#### 2. 12 Añadir fichero 2.txt

	touch 2.txt
	git add .
	git commit -m “añado el fichero 2.txt en la rama v0.2”

#### 2.13 Crear rama remota v0.2

	git push origin v0.2

#### 2.14 Merge directo

	git checkout master
	git merge v0.2

#### 2.15 Merge con conflicto (I)

	echo Hola > 1.txt
	git add .
	git commit -m “modifico 1.txt para meter Hola”

#### 2.16 Merge con conflicto (II)

	git checkout v0.2
	echo Adios > 1.txt
	git add .
	git commit -m “modifico 1.txt para meter Adios”

#### 2.17 Merge con conflicto (III)

	git checkout master
	git merge v0.2

#### 2.18 Listado de ramas

	git branch —merged
	git branch —no-merged

#### 2.19 Arreglar conflicto

Edito el fichero 1.txt para dejar únicamente Hola.

	vi 1.txt
	git add .
	git commit -m “modifico 1.txt para solucionar conflicto”
	git merge v0.2

#### 2.20 Borrar rama

	git tag v0.2
	git branch -d v0.2

#### 2.21 Listado de cambios

	git list
    
#### 2.22 Cuenta en Github

1. Poner una foto en el perfil de Github :white_check_mark:
2. Poner el factor de autentificación :white_check_mark:
3. Añadir clave pública :white_check_mark:

#### 2.23 Uso social de Github

1. Buscar y seguir a los usuarios de Githu de compañeros de clase :white_check_mark:
2. Seguir los repositorios campusciff de los compañeros :white_check_mark:
3. Añadir una estrella a dichos repositorios :white_check_mark:

#### 2.24 Crear una tabla

|NOMBRE|GITHUB|
|------|------|
|Amalia|http://github.com/asuarezg|
|Ulises|http://github.com/ulisesojeda|
|Carlos|http://github.com/cpazsantos|
|Sergio|http://github.com/sergiotorrespalomino|
|Paola|http://github.com/plopez76|

#### 2.25 Colaboradores

Poner a asandiego como colaborador del repositorio campusciff  :white_check_mark:

#### 2.26 Crear una organización

Crear organización llamada campusciff-davpacheco :white_check_mark:

#### 2.27 Crear equipos

1. Crear los equipos administradores y colaboradores, con sus permisos correspondientes, en mi organización :white_check_mark:
2. Incluir a dos compañeros en administradores :white_check_mark:
3. Incluir a dos compañeros en colaboradores :white_check_mark:

#### 2.28 Crear un index.html

Crear index.html como página para web de la organización :white_check_mark:

#### 2.29 Crear Pull-Request

1. Hacer 2 forks de 2 repositorios :white_check_mark:
2. Crear una rama en cada fork :white_check_mark:
3. En cada rama añadir nombre en el index.html :white_check_mark:
4. Hacer pull-request con cada rama :white_check_mark:

#### 2.30 Gestionar Pull-Request

Aceptar los pull-request que lleguen :white_check_mark:
