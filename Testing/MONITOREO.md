1. Instalar nodeJS: [Node.js — Run JavaScript Everywhere (nodejs.org)](https://nodejs.org/en)
2. Installar Newman:  npm install -g newman
3. Exportar la collection de Postman
4. Ejecutar: newman run path/collection.json
5. newman run path/to/collection.json -e path/to/environment.json -r cli,html --reporter-html-export results.html
6. Abrir GitBash en la carpeta donde se va a realizar el monitoreo
7. Crear archivo de Script: touch monitor.sh
8. Editar el archivo creado: nano monitor.sh



|     |                                                                 |                                                                                                                |
| --- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
|     | Instalar nodeJS                                                 | [Node.js — Run JavaScript Everywhere (nodejs.org)](https://nodejs.org/en)                                      |
|     | Installar Newman                                                | npm install -g newman                                                                                          |
|     | Exportar la collection de Postman                               |                                                                                                                |
|     | Ejecutar la collection                                          | newman run path/collection.json                                                                                |
|     |                                                                 | newman run path/to/collection.json -e path/to/environment.json -r cli,html --reporter-html-export results.html |
|     | Abrir GitBash en la carpeta donde se va a realizar el monitoreo |                                                                                                                |
|     | Crear archivo de Script                                         | touch monitor.sh                                                                                               |
|     | Editar el archivo creado                                        | nano monitor.sh                                                                                                |
|     |                                                                 |                                                                                                                |
|     |                                                                 |                                                                                                                |

- `Abrir GitBash en la ruta donde se encuentra el archivo monitor.sh
- `Editar el script: nano monitor.sh
- `Grabar: Ctrl + O
- `Cerrar: Ctrl + X
- `Convertir el archivo en ejecutable: chmod +x monitor.sh
- `Ejecutar el script:  ./monitor.sh
- `Detener el script: Ctrl + C`
