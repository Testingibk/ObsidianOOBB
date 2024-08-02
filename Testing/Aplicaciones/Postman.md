`Asertion de tiempo de respuesta
`pm.test("Response time is less than 200ms", function(){
    `pm.expect(pm.response.responseTime).to.be.below(200);
`});

##### `Newman Instalaciones
`npm install -g newman

##### `Reportes
`npm install -g newman-reporter-htmlextra

##### `Ejecutar collection de Postman y visualizar en consola
`newman run nombreDecollection.json

##### `Ejecutar collection de Postman y visualizar en Reporte html
`newman run nombreDecollection.json -r htmlextra
