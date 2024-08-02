### <font color = "yellow">Generación de Data</font>

<font color = "yellow">TABLA: USUARIO</font>
1. Elegir un usuario que tenga correo ofuscado
2. Editar directamente en la tabla ese correo y presionar el icono de Actualizar información

<font color = "yellow">OFFICE BANKING ACTUAL</font>
1. Ingresar a OBA y digitar el nombre del usuario elegido
2. Presionar OLVIDE CONTRASEÑA
3. Ingresar el correo ingresado en la tabla USUARIO DE SQLDEVELOPER

<font color = "yellow">TABLA : USUARIO_CODE_VERIFICATION</font>
1. Filtrar por el cliente que hemos seleccionado
2. Del campo CODE_VERIFICATION copiar el valor mostrado.

<font color = "yellow">OFFICE BANKING ACTUAL</font>
1. Pegar el código y presionar ENTER
2. Se abre directamente la vista donde se muestran las empresas a las que tiene acceso el usuario.

### otros apuntes
USUARIOGR
USUARIO CODE VERIFICATION

Buscar por numero de tarjeta en AS400 con la tabla USUARIO

USURIO
USG PASS INT

select * from usuariogr where USG_USERNAME IN ('VSANTINO', 'ACAMPOS', 'MVARRE');

update usuariogr set usg_pass_int = 0 where usg_username='VSANTINO';commit;


## <font color = "orange">CAPACITACIÓN SOFTTEK</FONT>

#### <font color = "sky blue">RESUMEN</font>
<font color = "sky blue">Creación Grupo Económico</font>
- Primer paso tener un cliente creado como prerrequisito
- 746 | 1 | 12 | F6 Crear
- Ingresar un nuevo Grupo Económico
- Nombre del Grupo a crear
- Añadir el miembro principal (el cliente creado en el paso anterior)
- N | S | VACIO
- Enter para terminar el Proceso
<font color = "sky blue">Creación Cliente o Empresa</font>
- 10 | 4 | 5 | Ingresar nuevo RUC de Empresa
<font color = "sky blue">Creación de Cuentas</font>
- 1 | 4 | 1 | 1 Asociarlo a un cliente que hemos creado 
- (Para afiliar al sistema se necesita que el cliente tenga mas de 2 cuentas)
<font color = "sky blue">Abonar a la cuenta</font>
- 1 | 5 | 1 | 
- Cajero 51
- Opción 151 : Nota de Abono (03 - nacer)
<font color = "sky blue">Afiliación de Cliente al Sistema OOBB</font>
- 19 | 1 | 4 | 1 | F6 Crear
- F4 para buscar el cliente
- Completar: F7 Empresas | F8 Cuentas + F10 Trx + F17 Datos Adic
<font color = "sky blue">Creación Usuarios</font>
- 19 | 1 | 4 | 1 | Consultar por nombre de Empresa
- Completar: F8 Usuarios + F6 Crear
- Generar Claves y Coordenadas
<font color = "sky blue">Asociación de Usuarios a Empresas</font>
- Después de generar claves y Coordenadas se regresar a la pantalla anterior y se muestra los datos en color blanco.
- F7 Empresas + F9
- Completar info con 1 y 1
<font color = "sky blue">Asociar cuentas al Usuario</font>
- Seleccionamos la empresa
- F8 Cuentas + F9 completar info con 1 - 1 1 
- F10 Transacciones
- F11 Roles
- F3 + F3 y las letras en blanco deben cambiar a Verde y desaparece la palabra Empresa- 
<font color = "sky blue">Sincronización</font>
- 19 | 14 | Buscamos por RUC o vamos a la parte final de la lista.
- Seleccionar
- F5 Aprobar solicitud
<font color = "sky blue">Confirmación de acceso correcto</font>
- 19 | 14 | Buscar por RUC
- No debe figurar en la lista
<font color = "sky blue">Info</font>
- 19 | 1 | 4 | 1 | Consultar por nombre
- Seleccionar y ya no debe aparecer MENSAJE EN ROJO

_FLUJOS DE CONSULTA_
Consulta de Cuentas del Cliente
- 10 | 3 | 1 | Ingresar nombre o RUC  | Seleccionar y Consultar
Movimientos de la Cuenta
- 1 | 3 | 1 | Ingresar nombre o RUC | Campo OPCION colocar 1 y Enter
Consultar Abono en la Cuenta
- 1 | 3 | 1 | Ingresar nombre 
### <font color = "orange">SESION 01</FONT>

- 1ro: Crear la empresa o Cliente  RUC 20600508581
- SCLR235 se da _Enter_ para validar si es que falta completar algún dato

- 2do Crear CUENTAS 8140910  8140928  8140936
- OPCION 10 - 3 - 9 - 1 

- 1 - 3 - 1 Cuentas alfabético

- 1 - 5 - 1 TRANSACCIONES EN LINEA
- Código de Cajero solicitar este dato para realizar transacciones en línea
- Solicitar SUPERVISOR Y CLAVE para realizar ingreso de transacciones en línea como ABONOS

- AFILAICION AL SISTEMA
- 19 E BUSSINES

- Afiliación por correo se debe solicitar por acceso a IBM

- SINCRONIZCION
- Necesitamos gestionar:
- Cajero, Supervisor y Clave para realizar Abonos o Cargos

PASO 01: Creación de Cliente
10 .- Clientes
4 .- Mantenimientos de usuario
5 .- Registro de clientes

PASO 02: CREACION DE CUENTAS
1 .- Cuentas corrientes y ahorro
4 .- Mantenimiento del usuario
1 .- Plataforma
1 .- Apertura cuentas ctes/ahorros

CONSULTA DE CUENTAS DEL CLIENTE
10 .- Clientes
3 .- Consultas
1 .- Consulta al padrón de clientes
	buscar por nombre o RUC

PASO 03: ABONO A LA CUENTA
1 .- Cuentas corrientes y ahorro
5 .- Cajas en línea
1 .- Transacciones en línea

CONSULTA DEL ABONO A LA CUENTA
1 .- Cuentas corrientes y ahorro
3 .- Consultas
1 .- Cuentas: alfabético
	Consultar por Nombre o RUC

8141088
8141096

AFILIACION AL SISTEMA
19 .- E-Bussiness
1 .- Office Banking
4 .- Mantenimiento Usuario
1 .- Afiliacion al Sistema
F6 Crear
Seleccionar la Empresa a afiliar.
- F7 EMPRESAS | F8 CUENTAS | F10 TRANSACCIONES | F17 DATOS ADIC.
- Salir con F3 | F8 Usuarios | F6 Crear
Generar Claves y Coordenadas

ASOCIACIÓN DE USUARIOS A EMPRESAS
F7 Empresas



### <font color = "orange">SESION 02</FONT>
- Preguntas:
	- Se puede asociar una misma cuenta a dos Empresas?
	- Las cuentas creadas también pertenecen al Holding?
	- En qué parte del flujo se agregan más usuarios a la empresa?
	- Cuándo se sincroniza, qué se sincroniza. Holding, Cliente o Usuario?
	**_Puntos tratados en la sesión_**
	- Generación de nueva clave 
	- Reseteo de clave
	- Grupos económicos
	- 

### <font color = "orange">SESION 03</FONT>
- 
### <font color = "orange">SESION 04</FONT>
- GARANTIAS
- Se puede vincular a varios productos de acuerdo a la necesidad del cliente o usuario
- 30 Y 31: se vincula a una Cta Cte o Ahorros.
- 32: Acciones pide si es de tipo terreno, no se enlaza a cuentas. Es registro manual donde se solicta garantia para un seguro o un terreno.
- 34: Seguros, pide el tipo de seguro
- 35: se vincula a un deposito a plazo
- TIPO 30: Generica es garantia simple pero si se coloca Especifica pide vincular a un cliente especifico

VWBMWPC1  <---- Clave AS400
Puntos tratados
- Garantía tipo 30
- Garantía tipo 35

#### SESION 05
- Garantía tipo 32

### <font color = "orange">SESION 06</FONT>
- Créditos directos e Indirectos
- Es necesario tener línea de crédito
- Leasing en Proceso y Leasing normal
- En Proceso, necesita aprobación de todos los datos conforme.
	- No se  mueve dinero solo registro visual en PosCon 
	- No disminuye el saldo de la cuenta.
	- Opción 300 Menú contratos en proceso
	- Queda pendiente responder Qué es el spread?
	- 
### <font color = "orange">SESION 07</FONT>
- No se pudo completar Confirming por el tema de la fecha que tiene que estar sincronizada el OBActual con el AS400. Eso se debe coordinar para mover la fecha.
- Cartas Fianza
- Tiene "Emisión" y "Modificación" que se realiza el mismo día además de "Renovación" y "Cancelación".
- Se necesita Línea de Crédito para que no salga error.
- Después de la liquidación se realiza el refrendo
- Se debe correr este comando para que el usuario pueda utilizar la Tarjeta de Coordenadas
	- UPDATE ALTEQBSP.SOFBF01 SET NROTAR = '90000002' WHERE NOMUSU IN ('ECORDERO')
	- 90000002 --> es la tarjeta a utilizar
	- ECORDERO --> actualizar al usuario que se va a hacer las pruebas con Tarjetas
- 
### <font color = "orange">SESION 08</FONT>

Consultas:
- Hacer ejemplos de 2da y 3ra Firma
- El RUC se puede utilizar para crear Grupo Económico y Clientes??
- Cash Nexus y Host to host
## <font color = "orange">Checklist Gestión Capacitación</FONT>

- [x] Enviar correo a Paola Martínez
- [x] Respuesta de correo solicitando detalle de ítems propuestos
- [x] Reunión con Paola
- [x] Preparar lo que se va a presentar a Paola  #FV: 24 junio
- [x] Paola debe responder el correo con la propuesta fina #FV <font color="red">25 junio</font>
- [x] Separar agenda para las capacitaciones de Softek para AS400
- [x] Correo de respuesta de PM
- [x] Reunión con Alfredo para evaluar la propuesta de PM 01/07/24
- [ ] Evaluación y respuesta al correo de OOBB a Softtek
#### Alfredo Llona - Plan B
- [x] Enviar a Alfredo el plan de generación de data con su equipo.
- [x] Pendiente de respuesta del plan enviado a Alfredo Llona.
- [x] Designó a Roger para apoyarme en la generación de data.
- [ ] 


## <font color = "yellow">Query Oracle para obtener cuantas cuentas tiene un cliente</font>

<font color = "yellow">Con esta query se obtiene el código de usuario</font>
select * from usuariogr where usg_username = 'VSANTINO';
Output: 1220100065038001  

<font color = "yellow">Con esta query se obtiene</font>
select * from usuariogr_clientegr where ugc_usuariogr = '1220100065038001   ';  /*Respetar los espacios vacíos

SELECT * FROM USUARIOGR_CLIENTEGR WHERE UGC_USUARIOGR = '1220203058781002   '

Response: 220100065038

UGC_USUARIOGR     UGC_TIP_DOC_CLG  UGC_NUM_DOC_CLG  UGC_ACTIVO

1220100065038001           2             ==20100065038==        S
1220100065038001           2             20130459090        S
1220100065038001           2             20331061655        S
1220100065038001           2             20491891255        S
1220100065038001           2             20513375736        S
1220100065038001           2             20531559526        S

<font color = "yellow">Con esta query se obtiene las empresas a los que está asociado el usuario. (Se debe añadir UGC_TIP_DOC_CLG)</font>
SELECT * FROM CLIENTEGR WHERE CLG_EMPRES_HLG = '220100065038';

Response:
CLG_TIP_DOC  CLG_NUM_DOC      CLG_NOMBRE                   CLG_ORIEMP_HLG   CLG_EMPRES_HLG
2                      20331061655          AJEPER S.A.                      01                 220100065038
2                      20100065038          VECTOR QA GLOBAL SAC             01                 220100065038
2                      20491891255          INVERSIONES PLATINUM S.A.C.      01                 220100065038
2                      20513375736          CORPORACION DRD S.A.C            01                 220100065038
2                      20531559526          ZZZZZZZZZZZZZZZZZZZZZZZZZZZ      01                 220100065038
2                      20130459090          SOCIEDAD LAS CASUARINAS S.R.L.      01                 220100065038
## <font color = "yellow">Correo enviado a PM</font> 

Hola Paola!

De acuerdo a lo coordinado con Alfredo Llona te enviamos la documentación solicitada.

Nuestra necesidad se basa en una capacitación sobre AS400 Por un lado tenemos la generación de la data que es un tema urgente para la primera fase y que comprende las funcionalidades de Login, Home y Posición Consolidada.

Los tópicos que vamos a abordar son los siguientes:
LOGIN
- [ ] Creación de empresas y usuarios nuevos con diferentes tipos de documento
- [ ] Asignación de permisos a los usuarios.
- [ ] Creación de grupos económicos
- [ ] Obtención de claves para usuarios nuevos
- [ ]  Reseteo de clave
- [ ] Recuperación de clave
- [ ] Obtención de usuarios antiguos con diferentes estados: activos, bloqueados, inactivos, deshabilitado, etc.

POSICION CONSOLIDADA
- [ ] Creación de cuentas corrientes y ahorros por tipos de moneda.
- [ ] Creación de movimientos (Abonos y cargos)
- [ ] Creación de Depósitos a Plazo
- [ ] Creación de Garantías
- [ ] Créditos Directos e Indirectos.
- [ ] Creación de Captaciones y servicios.
- [ ] Otros productos que forman parte de Posición Consolidada.

TRANSFERENCIAS
- [ ] Misma empresa
- [ ] Mismo grupo
- [ ] Tercero puntual
- [ ] Otros bancos (Diferida e inmediata) 
- [ ] Firma de transferencias (Configuración de hiperfirmas)
- [ ] Generación de clave para firmas (sms y correo)
- [ ] Notificaciones por correo

PAGOS
- [ ] Pago de proveedores 
- [ ] Pago de Haberes
- [ ] Pago de CTS
- [ ] Firma de los Pagos
- [ ] Pago en Línea
- [ ] Registro de Proveedores



<font color="blue">Este texto debería ser azul.</font>

## <font color = "yellow">Temario Capacitación AS400</font>
• *LOGIN* 
- Creación de empresas y usuarios nuevos con diferentes tipos de documento 
- Configuración de roles 
- Asignación de permisos a los usuarios. 
- Creación de grupos económicos 
- Obtención de claves para usuarios nuevos 
- Reseteo de clave 
- Recuperación de clave 
- Obtención de usuarios antiguos con diferentes estados: activos, bloqueados, inactivos, deshabilitado, etc. 
- Notificaciones por sms y correos
• POSICION CONSOLIDADA 
- Creación de cuentas corrientes y ahorros por tipos de moneda. 
- Creación de movimientos (Abonos y cargos) 
- Creación de Depósitos a Plazo 
- Creación de Garantías 
- Créditos Directos e Indirectos. 
- Creación de Captaciones y servicios. 
- Otros productos que forman parte de Posición Consolidada. 
• TRANSFERENCIAS
- Misma empresa 
- Mismo grupo 
- Tercero puntual 
- Otros bancos (Diferida e inmediata) 
- Firma de transferencias (Configuración de Hiperfirmas) 
- Generación de clave para firmas (sms y correo) 
- Notificaciones por correo
• PAGOS 
- Pago de proveedores 
- Pago de haberes 
- Pago de CTS 
- Firma de los pagos 
- Pago en línea 
- Registro de proveedores

###### <font color = "orange">PARA ABRIR UNA CUENTA</font>
1 .- Cuentas corrientes y ahorro
4 .- Mantenimiento del usuario
1 .- Plataforma
1 .- Apertura cuentas ctes/ahorros












https://gold-resonance-668307.postman.co/workspace/OfficeBanking-Santander~4d22adac-7f02-4e8e-b1e2-29273258e471/monitor/1ef4b5c5-3e9a-4430-8ab2-08979d901c7f