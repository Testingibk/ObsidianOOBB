1. Instalar nodeJS: [Node.js — Run JavaScript Everywhere (nodejs.org)](https://nodejs.org/en)
2. Installar Newman:  npm install -g newman
3. Exportar la collection de Postman
4. Ejecutar: newman run path/collection.json
5. newman run path/to/collection.json -e path/to/environment.json -r cli,html --reporter-html-export results.html
6. Abrir GitBash en la carpeta donde se va a realizar el monitoreo
7. Crear archivo de Script: touch monitor.sh
8. Editar el archivo creado: nano monitor.sh



|     | <font color="yellow">Paso                                       |                                                                                                                |
| --- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
|     | Instalar nodeJS                                                 | [Node.js — Run JavaScript Everywhere (nodejs.org)](https://nodejs.org/en)                                      |
|     | Installar Newman                                                | npm install -g newman                                                                                          |
|     | Exportar la collection de Postman                               |                                                                                                                |
|     | Ejecutar la collection                                          | newman run path/collection.json                                                                                |
|     |                                                                 | newman run path/to/collection.json -e path/to/environment.json -r cli,html --reporter-html-export results.html |
|     | Abrir GitBash en la carpeta donde se va a realizar el monitoreo |                                                                                                                |
|     | Crear archivo de Script                                         | touch monitor.sh                                                                                               |
|     | Editar el archivo creado                                        | nano monitor.sh                                                                                                |
|     | Grabar el archivo de monitoreo editado                          | Ctrl + O       Enter                                                                                           |
|     | Salir del modo edición                                          | Ctrl + X                                                                                                       |
|     | Convertir el archivo en ejecutable                              | chmod +x monitor.sh                                                                                            |
|     | Ejecutar el script                                              | ./monitor.sh                                                                                                   |
|     | Detener el script                                               | Ctrl + C                                                                                                       |

- `Abrir GitBash en la ruta donde se encuentra el archivo monitor.sh
- `Editar el script: nano monitor.sh
- `Grabar: Ctrl + O
- `Cerrar: Ctrl + X
- `Convertir el archivo en ejecutable: chmod +x monitor.sh
- `Ejecutar el script:  ./monitor.sh
- `Detener el script: Ctrl + C`


`newman run customerPositionv2.postman_collection.json -r htmlextra
```
newman run path/to/collection.json -e path/to/environment.json -r cli,html --reporter-html-export results.html
```
pm.test("Tiempo de respuesta es < 200ms", function(){
pm.expect(pm.response.responseTime).to.be.below(200);
});

pm.test("Codigo de respuesta es 200", function () {
pm.response.to.have.status(200);
});

### `Ejemplo de monitor.sh
#!/bin/bash

#### `Ruta a la colección de Postman
COLLECTION_PATH="customerPositionv2.postman_collection.json"

#### `Intervalo de tiempo en segundos entre cada ejecución (por ejemplo, 3600 segundos = 1 hora)
INTERVAL=3600

while true; do
  newman run $COLLECTION_PATH -r cli,html --reporter-html-export results.html
  sleep $INTERVAL
done



newman run customerPositionv2.postman_collection.json -r cli,html --reporter-html-export results.html

`newman run customerPositionv2.postman_collection.json -r cli

#!/bin/bash

### Ruta a la colección de Postman
COLLECTION_PATH="UAT-currency_Exchange.postman_collection.json";"UAT-CustomerPosition.postman_collection.json"

### Intervalo de tiempo en segundos entre cada ejecución (por ejemplo, 3600 segundos = 1 hora)
INTERVAL=3600

while true; do
  newman run $COLLECTION_PATH -r cli
  sleep $INTERVAL
done
