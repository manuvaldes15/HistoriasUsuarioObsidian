![[Pasted image 20260603143344.png]]
- ¿Como podria definir lo que hace este apartado?


Linea de credito y Clasificacion deberian de ser una sola HU ya que al seleccionar una linea de credito me muestra ya la clasificacion de la linea de credito


## Nuevas HU a implementar
- En el popup "Buscar Asociado" estan los botones: buscar, limpiar y asignar solicitud




---




## HU de busqueda de asociados para asignar solicitud de prestamo
1. Click en Nuevo
2. ** Muestra un pop up que se llama "Buscar Asociado"
3. ** Muestra y Validacion de datos de: Nombres (Solo texto), Codigo de Asociado (Solo numerico), nit (9999-999999-999-9), apellidos (Solo texto), dui (formato 99999999-9)
4. Muestra una tabla con nombre completo, fecha de nacimiento y estado
5. Al llenar algun campo de busqueda y realizar la busqueda deberia de mostrar la informacion de la persona o en caso de no encontrar registros, mostrar un mensaje de notificacion

---
## HU de Asignar solicitud a un asociado

1. Si se selecciona un asociado se debe dar click al boton de "Asignar solicitud" para crear un nuevo correlativo de prestamo y cargar los datos del asociado en los campos respectivos (no. prestamo, cod asociado, nombre completo del asociado, estado de la solicitud, y agencia con codigo y nombre)

--- 
## HU de Validación de Asignación de solicitud de prestamo

1. Mostrar una mensaje de alerta en caso de que el asociado, tenga sus datos desactualizados como telefono, dirección, dui
2. Mostrar un mensaje en caso de que el caso el asociado tenga credito otorgados
3. Mostrar un mensaje de manejo de la solicitud "Warning: Guarde los cambios en la solicitud actual antes de generar una nueva, o cancelar la solicitud actual."

--- 

## HU de parametrizacion y clasificacion de prestamos

 1. En la parte de Linea de credito se debe mostrar un listado de las lineas de creditos disponibles
 2. Al seleccionar una Linea de credito, me debe de asignar la Clasificacion correspondiente
 3. En la parte de Origen de fondos se debe mostrar un listado de los tipos de origenes de fondos disponibles para poder seleccionarlas
 4. lo mismo con: Garantias, Tipo de Crédito, Destino, Nivel de aprobacion, sector destino, promocion, asesor de negocio 
 5. y poder ingresar fecha de recepcion la cual no puedan ser fechas futura

---
## HU de perfil de credito
1. Campos que se pueden ingresar: puntaje de buro, porcentaje de extraprima, sueldo (no texto) comentario, destino del credito
2. En la parte de ¿como se entero del credito? se debe mostrar un listado de diferentes opciones disponibles
3. En la parte de ¿Quien lo refiere? donde se mostraran la lista de ejecutivos financieros o colectores

---
## HU de Plan de Financiamiento

1. Mostrar los campos de Monto, plazo, interes anual, ahorro simultaneo, seguro de deuda,otros seguros, aportacion, ahorro navideño, cuota extraordinaria
2. Mostrar datos que se calculen solos (no editables) como tasa de mora,  cuota, cuota/salario, tasa efectiva anual, cuota total
3. En los campos de: Forma de pago y tipo de plazo se debe mostrar un listado de sus diferentes opciones disponibles en ambos
4. Al seleccionar Aplica Otros seguros considera o no otros seguros
5. Muestra un apartado con la cantidad en texto del total a solicitar en el prestamo
6. Darme un apartado en donde podria escribir los documentos a presentar  

## HU Informacion de Solicitante
1. Ver un listado de las direcciones del relacionadas a la persona de la solicitud donde se muestre: tipo de direccion, departamento, municipio, distrito, colonia-barrio, dirección
2.  Ver un listado de correos electronicos relacionados a la persona de la solicitud donde se muestre: tipo de correo, email y si es principal o no.
3.  Ver un listado de los telefonos relacionados a la persona de la solicitud donde se muestre: tipo de telefono, numero y si es principal o no.


## HU de Situación economica
1. Darme la opcion de seleccionar si la persona "Es contribuyente de IVA" con las opciones de SI o No
2. Darme la opcion de seleccionar si la persona "Lleva contabilidad" con las opciones de SI o No

## HU de Ingresos de situacion economica

1. Mostrarme 2 tablas con la informacion de mis Ingresos y Egresos
2. Un apartado por cada tabla que me despliegue una lista de tipos de ingresos/egresos con sus diferentes opciones disponibles
3. Un campo por cada tabla con la opcion de ingresar el monto de dicho tipo de ingreso/egreso (datos numericos) 
4. Un boton  por cada tabla que me guarde/agregue el tipo y monto de ingresos/egreso a un listas correspondientes segun el tipo
5. Al ya haber ingresado un ingreso/egreso quiero tener la opcion de quitarlo de la lista correspondiente






