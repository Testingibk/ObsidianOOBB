## Funcionales
- [ ] Cómo funciona?
- [ ] Para qué sirve cada componente de la solución?
- [ ] Se puede obtener la firma del servicio?
- [ ] Por qué se añade capa de seguridad, tipo clave?
- [ ] Tiene alguna versión anterior?
- [ ] El cambio la actualización va a afectar de manera retroactiva?
- [ ] Cuánto tiempo de indisponibilidad se tendrá en el pase a PRD?
- [ ] Si dependemos de otro equipo se tiene que sincronizar da data que se va a pasar
- [ ] Se agregarán campos adicionales para la información solicitada o consultadas?
- [ ] Es Retroactivo?
- [ ] Será masivo o batch?
- [ ] Será masivo online??
- [ ] Qué servicio de mensajería se va a utilizar, Latinia o Enotria?
- [ ] Si se cambia el medio de respuesta
- [ ] Se puede EXTORNO o Revertir el Proceso?
- [ ] En qué puntos se aplica Seguridad a la aplicación?
- [ ] Se tiene tema de inactividad para el cierre de sesión?
- [ ] 
## Técnicas
- [ ] Qué es lo que has desplegado?
- [ ] Cómo nos relacionamos con otros equipos o con otras APIS?
- [ ] Cuánto tiempo de respuesta se esperar frente a una gran volumetría
- [ ] Consume una gran cantidad de recursos de CPU, Memoria, DTU?
- [ ] El formato y tamaño cómo va a evolucionar con el tiempo
- [ ] Longitud de campos
- [ ] 
## Base de Datos
- [ ] Apunta a Base de Datos?
- [ ] Qué tablas se tocan para la actualización?
- [ ] Tiene algún tipo de migración de tecnología?
- [ ] En migraciones hay que revisar si hay tiempo de convivencia
- [ ] Interviene dataFactory? se puede reemplazar por un microservicio?
- [ ] Se tiene que hacer rollback
- [ ] Es BD relacional o no relacional
- [ ] La BD es poblada por canales externos o solo por el aplicativo?
- [ ] Costo de incremento de data
- [ ] RU, Storage, limite de operaciones, acceso de lectura-escritura
- [ ] Frente a un crecimiento cómo se va comportar la aplicación o el micro servicio
## No Funcionales
- [ ] Se requiere la prueba con APIS?
- [ ] Se puede revisar en New Relic o dónde se visualizan las trazas?
- [ ] Cuál es la volumetría?
- [ ] Se ha probado hacerlo asíncrono?
- [ ] 

