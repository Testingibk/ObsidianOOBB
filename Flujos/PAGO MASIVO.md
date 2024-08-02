### Documentos
👇Documentación de Pagos Masivos (EM, Drawio y Macros)
[Proyecto Office Banking - 7. Pagos Masivos - Todos los documentos (sharepoint.com)](https://santandernet.sharepoint.com/sites/ProyectoOfficeBanking/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=rvFDcC&CID=251db94c%2De076%2D4ffb%2Dbb1c%2D4f174273b3b8&FolderCTID=0x01200023A6A8D0506CFD4298AB24E450191D4A&id=%2Fsites%2FProyectoOfficeBanking%2FShared%20Documents%2FGeneral%2FNTT%20DATA%2FHistorias%20de%20Usuario%2F7%2E%20Pagos%20Masivos)

👇Archivos que se utilizan para cargar Pagos Masivos
[Proyecto Office Banking - Macros - Todos los documentos (sharepoint.com)](https://santandernet.sharepoint.com/sites/ProyectoOfficeBanking/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=Gcw7rZ&ovuser=35595a02%2D4d6d%2D44ac%2D99e1%2Df9ab4cd872db%2Cpchavez%5Fexp%40santander%2Ecom%2Epe&OR=Teams%2DHL&CT=1719590911725&clickparams=eyJBcHBOYW1lIjoiVGVhbXMtRGVza3RvcCIsIkFwcFZlcnNpb24iOiI0OS8yNDA1MTYyMjIyMyIsIkhhc0ZlZGVyYXRlZFVzZXIiOmZhbHNlfQ%3D%3D&CID=7e1c37a1%2D0005%2D9000%2D3c86%2D7581477be521&cidOR=SPO&FolderCTID=0x01200023A6A8D0506CFD4298AB24E450191D4A&id=%2Fsites%2FProyectoOfficeBanking%2FShared%20Documents%2FGeneral%2FNTT%20DATA%2FHistorias%20de%20Usuario%2F7%2E%20Pagos%20Masivos%2FMacros)

#### <font color = "blue">Flujo de Pago de Haberes</font>
1. Pago de Haberes / Elaborar / Importar
2. Seleccionar: "Pago de Haberes Fija" y cargar el archivo de nuestro local
<font color = "blue">STATUS</font>
1. Pago de Haberes / Elaborar / Status
2. Para ver los errores en la importación se da click en "Ver detalle de errores"
<font color = "blue">LOTES EN PREPARACIÓN</font>
1. Pago de Haberes / Elaborar / Cerrar-Consultar
2. Ahí se ve los lotes de pagos de haberes en preparación
3. Seleccionar el Nro de pago de haber y dar click en CERRAR
4. Dar nombre de referencia y dar al botón CERRAR
<font color = "blue">AUTORIZAR EL PAGO</font>
1. Pago de Haberes / Autorizar
2. Elegir el nro. de lote
3. Obtener la clave virtual según la opción mostrada
4. Ingresar el código que se recibe según la opción elegida
5. Click en firmar
6. Se verá que el resultado de la operación se realizó con éxito.
<font color = "blue">ENVIAR</font>
1. Pago de Haberes / ENVIAR
2. Se puede seleccionar los pagos de lotes pendientes de envío
3. Se puede obtener clave virtual por Correo, SMS o Tarjeta de coordenadas
4. Ingresar el código y dar click en la opción enviar.
5. Ingresar a: Pago de Haberes / Consultar / Enviado para revisar el estado de los lotes enviados
6. 

PruebaPACG010720241546

#### 19 JUNIO
- El cliente se puede afiliar a pago proveedores
- Carlos dejó la siguiente información:
- De acuerdo con lo conversado te comparto los casos con el flag activo:
	- Cuando se registra un pago donde la cta es diferente al mantenimiento de proveedores, muestra un mensaje de error al cerrar el lote, impidiendo continuar el flujo.
	- Cuando se registra un pago donde la cta es igual al mantenimiento de proveedores, no presenta error y finaliza el flujo.
	- Cuando se registra un pago donde el CCI es diferente al mantenimiento de proveedores, no se presenta error y finaliza el flujo.  
	      
	    Estos casos contienen el flag deshabilitado; por lo tanto, no validará los datos del proveedor:
	
	1. Cuando se registra un pago donde la cta es diferente al mantenimiento de proveedores, muestra un mensaje de error al cerrar el lote, impidiendo continuar el flujo.
	2. Cuando se registra un pago donde la cta es igual al mantenimiento de proveedores, no presenta error y finaliza el flujo.
	3. Cuando se registra un pago donde el CCI es diferente al mantenimiento de proveedores, no se presenta ningún error e incluso al finalizar el flujo se corroborar que la CCI es actualizado.
#### 21 junio
- Haberes | Proveedores | CTS
- Ese archivo con clave se guarda en una BD? Se guarda para un tema de Auditoria después? Se puede reutilizar? 

#### 27 junio
- Registro manual: se esta definiendo los campos opcionales y obligatorios
- Dirección - ciudad - país
- Si existe un archivo y se incluye un proveedor que existe entonces debe responder con error.
- mínimo de registros para el proceso masivo?? 9999.99 máximo
- Siguiente reunión: Pago Haberes - Pago CTS
- Video 1:36:00 se da el concepto de Pagos y Descuentos.
	Si no tiene montos es ilimitado que firme uno o varios firmantes. Debe estar asociado a hiperfirmas y eso depende de la parametria que esta descrita ahí.
	
#### 28 junio
- Pago Manual
- La información cargada a través del archivo se pierde si es que nos dirigimos a otra pantalla o a otra sección del OBA.
- 1:29:00 Revisión de clave

#### 02 julio
- La paginación es de 25 registros en todas las pantallas.
- No se debe actualizar el archivo cargado cuando se edita online cada registro
- En la carga del pago a Proveedores 
- 3 meses sin transacciones muestra Cuenta Inmovilizada
- Verificar si el tipo de cuenta a utilizar para el pago esta activa o inactiva e Integración debe hacer un cambio para traer algunos estados de la cuenta.

#### 17 julio
 - 