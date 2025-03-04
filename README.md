#Comandos para instalar librerias de python en un entorno virtual
Se hace por medio de ir instalando las librerias por proyectos osea en entornos virtuales osea se instalan las librerias no globalmente

//Este paso 2 es para crear la carpeta .venv en caso de ser la primera ves en instalar una libreria del proyecto
1-
cd  ruta del proyecto
2-
python -m venv venv - crea una carpeta llamada venv o .venv

//Este paso es para ya instalar las librerias despues o antes como sea
3-
Primero, yo uso power shell lo cual no permite ejecutar scripts asi que antes se usa este comando para permitir ejecutar en esa pestaña: Set-ExecutionPolicy Bypass -Scope Process -Force
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

