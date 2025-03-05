##Comandos para instalar librerias de python en un entorno virtual || -usa Set-ExecutionPolicy Bypass -Scope Process -Force Antes de todo para poder ejecutar scripst
Se hace por medio de ir instalando las librerias por proyectos osea en entornos virtuales osea se instalan las librerias no globalmente

//Este paso 2 es para crear la carpeta .venv en caso de ser la primera ves en instalar una libreria del proyecto
1-
cd  ruta del proyecto
2-
python -m venv venv - crea una carpeta llamada venv o .venv

//Este paso es para ya instalar las librerias despues o antes como sea
3-
Primero, yo uso power shell lo cual no permite ejecutar scripts asi que antes se usa este comando para permitir 
ejecutar en esa pestaña: Set-ExecutionPolicy Bypass -Scope Process -Force
4-
Accedes a la ruta de tu proyecto donde creaste el .venv y ejecutas el siguiente comando: .\.venv\Scripts\Activate

5-
verificas que la ruta esa del proyecto y no la de python global con este comando: python -c "import sys; print(sys.executable)"

6-
Si te sale la lista del proyecto ya puedes instalar librerias o l oque sea: 
pip list - lista de las librerias instaladas
pip install "Nombre de la libreria" - Instalar librerias
pip list --outdated - Lista de librerias que necesitas actualizacion
pip install --upgrade "Nombre de la libreria"

//Para usar una version en especifico de python en un entorno virtual 
1- Instalar la version de python que usaras en el entorno virtual sin agregar las variables al PATH
2-borrar el antiguo entorno virtual con : Remove-Item -Recurse -Force .venv
con py -0
te muestra las versiones que tienes instaladas de python
3-Crea el entorno virtual con el python que quieres usar con: py -3.8 -m venv .venv | donde sice 3.8 va la version de tu python a usar
4-ahora ejecutaras : .venv\Scripts\Activate y te debera salir unas cosas alado de la ruta de donde te encuentras
5- ahora ya te encuentras adentro de tu entorno virtual con la version de python especial usa : python --version para verificar

 