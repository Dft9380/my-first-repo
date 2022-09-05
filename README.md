# my-first-repo
Cuenta de Práctica para Aprender Git

![image](https://user-images.githubusercontent.com/93413366/188342810-6cae9736-62fa-4822-ac7d-e59f107b8925.png)
main (rama principal)

## Clonar Repositorio

- en code copiar el link HHTPS

- abrig git : click derecho / git bush here
- Crear Carpeta : mkdir nombreCarpeta
- entrar a la Carpeta: cd nombreCarpeta
- Clonar repositorio : git clone linkHHTPS

- Listar todos los archivos : ls -la
- entrar al repo (en este ejemplo): cd my-first-repo
- Listar archivos : ls -l

## Agregar y Confirmar (Add and commit)

ver en que directorio estoy: pwd
listar todo : ls -la
ver estado de cambios y confirmaciones : git status
Crear un archivo de texto : touch nombreArchivo.txt
ver estado de cambios y confirmaciones : git status

NOTA en este caso vera que dice que el archivo aun no ha sido rastreado
osea no tiene seguimiento (color rojo)

Agregar el archivo de texto: git add nombreArchivo.txt
ver estado de cambios y confirmaciones : git status

NOTA en este caso vera que dice que el archivo ha sido rastreado
y tiene seguimiento y esta esperando a ser listo para confirmar(color verde),
en caso de querer revertir esto ejecutar git restore --staged nombreArchivo.txt

limpiar interfaz : clear
confirmar : git commit -m "aqui va el mensaje que desee poner"
ver estado de cambios y confirmaciones : git status

NOTA en este caso vera que dice que no hay nada que confirmar y que
el arbol(menu o rama principal) esta limpio

## Ramas Branches

Crear una nueva rama : git checkout -B feature/nombreDeLaRama
ver en que rama estoy : git branch
Crear un archivo de texto : touch nombreArchivo2.txt
Agregar el archivo de texto: git add nombreArchivo2.txt
confirmar : git commit -m "aqui va el mensaje que desee poner"
subir los cambios a GitHub : git push -u origin feature/nuevaRama 
Entramos GitHub

NOTA en este caso vera que se creo una nueva rama y debera de dar click en 
compare & pull request(comparar y solicitar extraccion) y luego en creat pull request

fusionar rama : hacer click en merge pull request
en git bash : git status
consultar rama principal : git checkout main
recibir los cambios de GitHub : git pull
listar : ls

## Saber que dice un archivo de texto
cat nombreArchivo.txt

## Escribir dentro de un archivo de texto
vim nombreArchivo.txt
escribir lo que quiera

## Comparar cambios en un archivo
git diff nombreDelArchivo

## Comparar cambios entre archivos
git diff nombreDelArchivo1 nombreDelArchivo2

## Buscar los cambios especificos de un archivo
(fechas, tiempos y usuarios que realizaron cambios)

git blame nombreDelArchivo



