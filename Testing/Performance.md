#### <span style="color:rgb(81,253,89);">Alcance</SPAN>
- [ ] Definir con Dev o LT Apis a Probar
- [ ] Establecer persona para el monitoreo de los recursos
- [ ] Establecer tipos de prueba a realizar
#### <span style="color:rgb(81,253,89);">Entorno de Pruebas</span>
- [ ] Establecer qué recursos se van a monitorear. Detalles de servidores, CPU, memoria y almacenamiento.
- [ ] Ubicar a la persona responsable del monitoreo para solicitar su apoyo para las pruebas.
- [ ] Configurar red y latencia.
#### <span style="color:rgb(81,253,89);">Data para las Pruebas</span>
- [ ] Capacitación para generar data masiva de pruebas
- [ ] Requerimiento de data del equipo QA
- [ ] Asegurar que la data cubre todos los escenarios posibles
- [ ] 
#### <span style="color:rgb(81,253,89);">Preparación para inicio de las Pruebas</span>
- [ ] Establecer fecha de inicio.
- [ ] Preparar el proyecto Jmeter
- [ ] Obtener data para inyectar data de forma masiva.
#### <span style="color:rgb(81,253,89);">Ejecución de las Pruebas</span>
- [ ] Establecer fecha de inicio.
- [ ] Preparación del proyecto Jmeter
#### <span style="color:rgb(81,253,89);">Herramientas y Configuración del entorno</span>
- [ ] Jmeter
- [ ] Dynatrace - para monitorear logs.
- [ ] 
#### <span style="color:rgb(81,253,89);">Métricas de Evaluación</span>
- [ ] Tiempo de respuesta
- [ ] Uso de memoria
- [ ] Uso de CPU
- [ ] Throughput: Número de transacciones por segundo.
- [ ] Errores: Tasa de errores y tipos de errores.
#### <span style="color:rgb(81,253,89);">Criterios de Aceptación</span>
- [ ] Tiempo de respuesta < 200 ms
- [ ] Uso de memoria <=70%
- [ ] Uso de CPU <=70%
#### <span style="color:rgb(81,253,89);">Análisis de Resultados</span>
- [ ] 
#### <span style="color:rgb(81,253,89);">Informe de Pruebas</span>
- [ ] 

-----------------------
Funcionalidades a probar
- Login
- Home
- Posición Consolidada
- Cuentas
- Si hasta el 10 de agosto no se tiene VPN Mexico no se puede hacer las pruebas de stress.
- Se debe cerrar 15 agosto. No se va a tener VPN Mexico.
- Condición: se debe tener conexión en QA directo a Mexico.
- Ruta critica: logueo, home cargo el tipo de cambio, la bandeja y la PC.
- Preguntar al QA de Surgir para ver cómo hacen sus pruebas.

- 2do pase a PRD
- Transferencias y bandejas : 31 agosto debe entregar VPNM
- Bandejas porque trae el contador.
- Transferencias se realizan 
Para pagos es carga de volumen de datos en las pruebas
- 20 setiembre no tenemos no se puede hacer pruebas de carga.
- Cuantos megas se van a cargar.

Front y back
- 5 usuarios concurrentes por 5 minutos
- En secuencia los 3 funcionalidades
- Buscar a Surgir para ver cómo hacen sus pruebas.
- Herramientas que usan
- En qué momento se realizan
- Es parte de la conformidad para hacer el pase a PRD.
- 1254 clientes activos Empresas y de aquí se tiene que ver cuántos usuarios se manejan
- máximo 5 usuarios preguntar a Ale.
- Se podría decir que se tiene 6000 usuarios se logueen a la vez.
- Este MVP va a ir por Landing Zone -> se debe hacer en un ambiente homologado con PRD no se puede hacer con la VPN actual. Se debe hacer con la que va a Mexico o sea conexión directa.
- 2da. Si no tiene hay que hacer por LZ 


\\bsfs02