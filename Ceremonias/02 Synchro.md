#### 10 junio
- Pedro esta viendo el Jira para poder lograr la conexión.
- Oscar: depende de Ligia, se va a ver en una reunión posterior.
- Moisés: VPN hay correo pendiente por este tema.| Hay una semana de retraso por este asunto.
- Ambiente UAT ya está listo para el equipo de desarrollo.
- Reu 5 pm para revisar el cronograma.
- Multiplica: Augusto sale de vacaciones la semana del 24. 
- El correo de Yeltsin para estandarización del API.
- La reu busca el impacto sobre el proyecto en general. Luego hacer el seguimiento sobre este impacto.

#### 11 junio
- El Jira todavía tiene problemas de acceso | se esta viendo con el equipo de Seguridad | Solo desde Santander se puede acceder a Jira
- TI tiene temas con la VPN: Pedro ya esta levantada la conexión a CORE, sftpy ws | esta pendiente conexión a BD y se esta haciendo validaciones con Infra | A PRD se llega a la infraestructura pero no hay respuesta. | se tiene que homologar | Ojo con latencia.
- La comunicación con Mexico siempre es con Infra no DEV | Usar puerto correcto 20:22 
- Fecha limite el 15 de junio.
- Cuentas y Operaciones se mueve dos días y Operaciones 1 día útil.
	- El impacto viene por el lado de la VPN.
	- Algunos servicios se iban a ir a Integración sino se queda en OOBB.
- Henry: hay APIS que están en el catálogo que no están certificadas | hay contratos que no están aprobadas | Yeltsin debe gestionar .... | Existe un catálogo en el que se tiene todas las APIS - Gluon Alfredo tiene contacto en Latam para hacer el camino más rápido.
- Punto Importante cuando se van a crear nuevas APIS porque tienen un flujo que consume esfuerzo y tiempo.
- Arquitectura: Pedro esta avanzando para iniciar la gestión de la infra el 15 jun para aprovisionar la próxima semana. | Oscar está levantando la info para enviar borrador | Esto es sobre la nube de SURGIR | La otra nube es la Landing Zone | Hay conformidad del lado de SURGIR para hacer despliegue en PRD | 

#### 12 junio

- Arnoldo: esta retomando el tema del token, lo esta coordinando con Jhohan | Falta hacer puntualmente la propuesta de Integración.
- Edison: Esta viendo el tema de Transferencias
- Diego: La propuesta se esta viendo hacerla como el BCP sobre Transferencias | No va a haber migración de Operaciones 
- Los saldos serán en línea en ambos OB.

#### 13 junio
- Celebración del día del padre para el viernes, van a estar varias personas del proyecto.
- Cronograma y fechas de Moisés.
- Tenemos que revisar las tareas del cronograma porque se están cruzando las fechas.
- Perú va a exponer un primer API en el Gluon apoyado de una persona de Brasil.
- Ale: pendiente el Ok de Cyber con Eduardo.
##### 17 junio
- LT: tanto de OB e INT debe ser de acompañamiento, 
- Definiciones, cronograma y avances se tiene que dar por parte de NTT
- NTT no debe correr bajo el equipo Santander.  Santander se paga a un proveedor para construir el OB dentro del MVP.
- Enviar correo a Adolfo con copia a Marco. 

#### 17 junio
- [ ] Generación data y Capacitación - Accesos a AS400
- [ ] Pendiente el envío de la propuesta de capacitación de parte de Paola Martínez.
- [ ] Creación del usuario esta pendiente de Luis Cortez.
- Jira esta impactando a todas las tareas que se están desarrollando.
- Arnoldo: El cambio de password que es parte del Login. | La base de datos esta implementado para ir a lo ws | si se toca las BD se tendría que hacer pruebas de regresión. Los servicios si funcionan pero hay que enviar un argumento adicional | Hay que ver el impacto en las otras APIS.
- Felipe: Henry esta haciendo la POC con MQ | Integración . hay dependencias con PRD | Gobierno de APIS se va a cruzar con Alfredo y mañana con Marco..
- El tema del navegador oficial esta con Carlos Juscamaita y debe responder España | Ale va a hablar con Alfredo Llona.
- Negocio | Adolfo | Mañana hay reunión para ver el tema del diseño con España Ignacio Sanchez CIB | 2. Validación del desfase para ver el impacto en fechas. | hay un bosquejo de la solución técnica y se están validando este nuevo flujo y espera la aprobación de Marco.
#### 18 junio
- Pedro: hay un error en el flujo de devops | hay ticket para la documentación | ya se debe tener acceso para correr el pipeline. Es para entrar desde la red. El pipeline esta consultando la pagina. Se esta ingresando las excepciones correctas.
- Seguimiento de la VPN: Es mandatorio que vaya por México no por Perú | la implementación puede ser 2 meses. | Landing Zone es 30 junio | Respuesta de la VPN es para el 26 junio.
- Navegadores: NO debe soportar Internet Explorer. Este es un tema de comunicaciones.
- [ ] Generación data y Capacitación - Accesos a AS400
- [ ] Pendiente el envío de la propuesta de capacitación de parte de Paola Martínez.
- [ ] Creación del usuario esta pendiente de Luis Cortez.
#### 19 junio
- Se va a hacer la actualización del NODE se tiene que actualizar el pipeline. De esto depende otras aplicaciones. El corporativo tiene que hacer los cambios.
- Pedro; VPN ayer se iba a tener una reunión para ver los detalles | Se puede disminuir los dos meses.
- Ale; el tema de los navegadores se necesita una confirmación de Global | hay empresas que aún utilizan Internet Explorer | Agendar call para definir este punto.
- Moisés; AS 400 de una persona de NTTData porque tiene que hacer análisis del core de bandeja | el 1 de julio se debe terminar el análisis | Henry no tiene los datos suficientes para crear las APIs | este tema es cross. | Eduardo es un tema de gestión a nivel Global - Alfredo esta ayudando a hacer push. 
#### 20 junio
- Pedro; ya se dio la solución con el equipo de Oscar falta la confirmación si no queda nada mas para tener  la tarea completada.
- VPN: se va por la nube de Surgir, la conexión debe ser por Mexico. Rolando debe ingresar un ticket para tener una respuesta por ser primera vez ver estos procesos. Para los despliegues de agosto se toma la nube de Surgir. | Con esta definición se debe empujar todos los recursos para PRD | Se confirmó la creación de la base de datos solo falta el AKS
- Navegadores; esta pendiente de agendar un espacio para definir estos puntos.

	<font color="yellow">Conformidades</font>
- La generación de data se debe revisar con Alfredo
- Owner 
- Eduardo Sotero: desde riesgos validan Procesos y controles
- Grover, 
- Ale Diaz. PO | debe preguntar Compliance de los cambios que están haciendo si se esta cumpliendo la normativa interna y externa.
	- Debe revisar el impacto financiero
	- Debo buscar Conformidad de usuario y Owner 
	- Aprobación técnica (Alfredo Llona) y funcional (Ale Diaz).
- Usuarios trabaja con Javier Sabas
- Ciberseguridad

<font color="yellow">Moisés - Generación de data</font>
- Hay un Contrato Marco en el cual se definen las responsabilidades de ambas partes.
- Lo que tiene Eduardo es una copia de ese contrato donde se muestra las actividades que puede realizar el perfil o cada rol.
- La ADENDA es lo definitivo en el cual se limitan responsabilidades de cada rol, fechas y entregables.

#### 24 junio
- Pedro: Mexico todavía no esta listo | A nivel infra ya esta conectada. | 
- Ale: Navegadores no hay persona en si que lo vea | esta pendiente definir la cantidad de clientes que utilizan Internet Explorer

#### 25 junio
- Pedro: Mejor es por la VPn del Perú | la demora esta ir por Mexico | Lo mejor es tomar la ruta correcta y gestionar los grupos de recursos además del AKS. | Se puede dejar todavia los recursos de ambientes previos.
- Navegadores: Lo va a ver con Frncesca
#### 26 junio
- Pedro: Tiene pendiente de enviar la solicitud para el viernes y depende que termine el ambiente de UAT. | Para INT-UAT se está priorizando para tenerla conectada. Es por la cantidad de recursos. | Esta pendiente la fecha de aprovisionamiento.
- Navegadores
- RTO y RPO | instalación en la laptop de Noemi | 
#### 27 junio
- pedro: se esta viendo si se tiene alguna conexión | se va a generar un nuevo grupo de recursos donde vaa a estar comparrtido

#### 1 julio
- Pedro: Se tiene que actualizar formatos para completar el acceso | Oscar: va a enviar los diagramas y las nomenclaturas solo del SQL para UAT, pero son de los cuatro, solo se va a tener uno solo para todos los ambientes. Hoy se envía. | Se tiene que estimar la latencia si se va por Perú o Mexico -> se puede hacer prueba de Network Tools | Samuel: no se pudo conectar a la BD y otro al WS y se tiene que solventar ese problema. Los certificados para los WS se tiene que verificar.
- Navegadores: No se usan IE, se están haciendo muestras para ver el impacto.
- Ingreso de QA de Integración
- Fecha de despliegue de Login, Home.
#### 03 julio
- Pedro: se resolvió el problema de la conexión a la BD y al AKS.
- Se esta terminando el aprovisionamiento para los nuevos recursos de PRD.
- AS7+Q447Jg
- AS109555969
#### 08 julio
- VPN se tiene que hoy se puede iniciar con PRD y se va a crear tickets para iniciar con el proceso.
- Responsable regional con Alfredo Llona.
- Rudy Gutarra PM 09 julio
#### 16 julio
- 