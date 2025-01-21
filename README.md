#Comandos para instalar librerias de python en un entorno virtual
Se hace por medio de ir instalando las librerias por proyectos osea en entornos virtuales osea se instalan las librerias no globalmente

1-
cd  ruta del proyecto
2-
python -m venv venv - crea una carpeta llamada venv o .venv
3-
.venv\Scripts\activate.bat - o en caso que te mencione que no puedes ejecutar scripts en power shell usa este otro: powershell -ExecutionPolicy Bypass -Command ".\.venv\Scripts\activate"
4-
pip install nombre-de-la-libreria - aqui ya instalas las librerias solo en el proyecto
5-
pip list - lista de las librerias instaladas
