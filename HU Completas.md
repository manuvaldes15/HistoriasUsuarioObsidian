
*HISTORIAS DE USUARIO — MÓDULO CYR
PANTALLA: SOLICITUD DE PRÉSTAMOS
SECCIÓN: FRONTEND — HISTORIAS FORMATEADAS DESDE DOCUMENTO HU

---
## :LiCheck: Historia 6: *[CYR]* [Solicitud de Préstamos] Pantalla de búsqueda de asociado para nueva solicitud

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** un formulario con campos de búsqueda para encontrar al asociado al que se le creará la solicitud de préstamo
**Para:**  identificar correctamente al asociado antes de iniciar el registro de una nueva solicitud

### Criterios de aceptación:
* Debe tener un botón/sección para realizar la búsqueda de asociados para asignarle una nueva solicitud
* La ventana muestra los siguientes campos de búsqueda: nombres,
  apellidos, código de asociado y DUI del asociado.
* El campo Nombres solo permite ingresar texto; no acepta números
  ni caracteres especiales.
* El campo Apellidos solo permite ingresar texto; no acepta
  números ni caracteres especiales.
* El campo Código de Asociado solo permite ingresar valores
  numéricos.
* El campo DUI aplica la máscara de formato 99999999-9 para
  garantizar el ingreso correcto.
* El campo NIT aplica la máscara de formato 9999-999999-999-9.
* La ventana cuenta con un botón Buscar para ejecutar la consulta
  y un botón Limpiar para vaciar los campos. **separar
* No es obligatorio completar todos los campos para ejecutar
  la búsqueda; basta con al menos un valor ingresado.

---
## :LiCheck: Historia 7: *[CYR]* [Solicitud de Préstamos] Pantalla de resultados de búsqueda de asociado

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** ver los resultados de la búsqueda de asociado en una tabla
**Para:**  seleccionar al asociado correcto de entre los registros encontrados

### Criterios de aceptación:
* Los resultados de búsqueda se muestran en una tabla con las
  columnas: nombre completo, fecha de nacimiento y estado.
* La tabla permite seleccionar un registro a la vez.
* Si la búsqueda retorna resultados, se muestran en la tabla
  de forma inmediata.
* Si la búsqueda no encuentra registros con los filtros ingresados,
  el sistema muestra un mensaje de notificación informando que
  no se encontraron registros.
* La tabla incluye paginación cuando el número de registros
  supera los que se muestran por página.


---
## :LiCheck: Historia 8: *[CYR]* [Solicitud de Préstamos] Pantalla de asignación de asociado a la solicitud

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** poder seleccionar un asociado de la tabla de resultados y asignarlo a la nueva solicitud de préstamo
**Para:**  que el formulario de detalle se cargue automáticamente con los datos del asociado seleccionado

### Criterios de aceptación:
* Debe tener un botón que permita asignar la solicitud 
* Debe mostrar un mensaje de confirmación de la selección del asociado
* Al presionar "Asignar Solicitud" con un registro seleccionado el sistema carga el formulario
  de detalle de la solicitud.
* El formulario de detalle muestra automáticamente los siguientes
  datos del asociado y la solicitud: número de préstamo generado,
  código del asociado, nombre completo del asociado, estado inicial
  de la solicitud y agencia con código y nombre.
* Todos los campos cargados automáticamente se muestran bloqueados;
  el usuario no puede modificarlos desde este formulario.
* Si el usuario presiona "Asignar Solicitud" sin haber seleccionado
  ningún registro de la tabla, el sistema muestra un mensaje de
  advertencia indicando que debe seleccionar un asociado primero.

---
## :LiCheck: Historia 9: *[CYR]* [Solicitud de Préstamos] Pantalla de validaciones y alertas al asignar un asociado

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** que el sistema me muestre un mensaje de las alertas relevantes sobre el asociado al momento de asignarlo a la solicitud
**Para:**  tomar decisiones informadas antes de continuar con el ingreso de datos del crédito

### Criterios de aceptación:
* Si el asociado tiene datos desactualizados (teléfono, dirección
  o DUI), el sistema muestra un mensaje de advertencia indicando
  que se debe actualizar la información antes de continuar.
* Si el asociado tiene créditos en estado Otorgado, el sistema
  muestra un mensaje informando la cantidad de créditos activos.
* Si ya existe una solicitud en proceso y el usuario intenta
  crear una nueva sin guardar o cancelar la actual, el sistema
  muestra el siguiente mensaje de advertencia
* Los mensajes de alerta son informativos; no bloquean el flujo.
* Los mensajes se muestran de forma secuencial si hay más de
  una alerta aplicable.


---
---
---

---

## Historia 10: *[CYR]* [Solicitud de Préstamos]  Selección de línea de crédito y clasificación

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** seleccionar la línea de crédito de la solicitud y que el sistema asigne automáticamente la clasificación correspondiente
**Para:**  registrar correctamente la clasificación del crédito sin necesidad de digitarla manualmente

### Criterios de aceptación:
* El campo Línea de Crédito se presenta como lista desplegable con las opciones disponibles y activas en el sistema.
* Al seleccionar una línea de crédito, el sistema actualiza automáticamente el campo Clasificación con el valor que corresponde a esa línea.
* El campo Clasificación se muestra en modo solo lectura; el usuario no puede modificarlo directamente.
* Si la línea de crédito se cambia por otra, el campo Clasificación se actualiza automáticamente con el nuevo valor.
* Si se deja sin selección, el campo Clasificación permanece vacío.

---
## Historia 11: *[CYR]* [Solicitud de Préstamos] Campos de catálogos del formulario principal

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** completar los campos de catálogo del formulario principal de la solicitud seleccionando las opciones disponibles
**Para:**  registrar las condiciones y características del crédito de forma correcta y estandarizada

### Criterios de aceptación:
* Los siguientes campos se presentan como listas desplegables con sus opciones disponibles:  
	* Tipo de Crédito
	* Destino
	* Promoción
	* Asesor de Negocio
	* Origen de Fondos
	* Nivel de Aprobación
	* Garantía
	* Sector Destino
	* Detalle de Sector.
* Al seleccionar un Sector Destino, el campo Detalle de Sector Destino se actualiza automáticamente con las opciones correspondientes a ese sector.
* El campo Autorización de Consulta presenta las opciones "Autoriza" y "No Autoriza" como lista desplegable.
* El campo Fecha de Recepción incluye un selector de calendario y no permite seleccionar fechas futuras.

---
## ⚠Historia 12: *[CYR]* [Solicitud de Préstamos] Perfil crediticio del solicitante

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** registrar los datos del perfil crediticio y económico del solicitante en el formulario de la solicitud
**Para:**  complementar la información necesaria para el análisis y aprobación del crédito

### Criterios de aceptación:
* El formulario muestra los siguientes campos editables de texto libre o numérico: 
	* Puntaje de buró
	* Porcentaje de extraprima 
	* Sueldo
	* Comentario 
	* Destino del crédito.
* **Los campos puntaje de buró, porcentaje de extraprima y sueldo solo aceptan valores numéricos con decimales; no permiten ingreso de texto.
* El campo comentario y el campo destino del crédito aceptan texto libre con un límite máximo de caracteres y un formato de párrafo.
* Debe permitir de cargar los medios disponible por los cuales el asociado se dio cuenta del crédito, se presenta como lista desplegable con las opciones disponibles configuradas en el sistema.
* **El campo "¿Referido por Ejecutivo Financiero o Colector?" se presenta como lista desplegable con los ejecutivos financieros y colectores disponibles según la agencia.

---
## Historia 13: *[CYR]* [Solicitud de Préstamos] Ingreso de términos financieros del préstamo

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** ingresar los términos financieros de la solicitud en los campos editables de la sección de plan de financiamiento
**Para:**  registrar las condiciones económicas bajo las cuales se está solicitando el crédito

### Criterios de aceptación:
* La sección de términos muestra los siguientes campos editables:
	* monto
	* plazo
	* interés anual
	* aportación
	* ahorro simultáneo
	* seguro de deuda
	* ahorro navideño
	* cuota extraordinaria.
* Los campos Tipo de Plazo y Forma de Pago se presentan como listas desplegables con sus opciones disponibles.
* Todos los campos de monto y valor solo aceptan valores numéricos con decimales; no permiten texto.
* La casilla "Aplica Otros Seguros" se presenta como opción seleccionable. Al activarla, el campo Otros Seguros se habilita para ingresar el valor correspondiente; al desactivarla, el campo se deshabilita y su valor se limpia.
* El campo Otros Seguros está deshabilitado por defecto hasta que se active la casilla correspondiente.

---
## ⚠Historia 14: *[CYR]* [Solicitud de Préstamos] Visualización de cálculos automáticos de los términos

Descripción
**Yo como:** usuario del sistema financiero 
**Quiero:** visualizar los valores calculados automáticamente por el sistema en la sección de plan de financiamiento
**Para:**  verificar los resultados del crédito sin necesidad de calcularlos manualmente

### Criterios de aceptación:
* Los siguientes campos se calculan automáticamente y se muestran en modo solo lectura: 
	* tasa de mora
	* cuota
	* cuota total
	* porcentaje de cuota sobre el salario 
	* tasa efectiva anual.
* Los campos calculados se actualizan automáticamente cada vez que el usuario modifica alguno de los campos que los afectan.
* Si la tasa efectiva anual calculada supera la tasa máxima permitida, el campo muestra una advertencia en color rojo junto a su valor.
* El usuario no puede modificar directamente ninguno de estos campos calculados.
* Los valores se presentan con dos decimales y formato numérico consistente con el resto del formulario.

---
## Historia 15: *[CYR]* [Solicitud de Préstamos] Sección de cantidad en letras y detalle de documentos a presentar


Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** ver el monto solicitado expresado en palabras y contar con un apartado para registrar los documentos requeridos
**Para:**  tener la descripción textual del monto y documentar los requisitos de la solicitud en el mismo formulario

### Criterios de aceptación:
* Debe tener un apartado en donde se convierta el monto a su Cantidad en letras incluyendo los centavos y su moneda de curso legal muestra automáticamente el monto solicitado convertido a su expresión en palabras en español.
* El campo se actualiza automáticamente cada vez que el monto solicitado cambia.
* El campo "Cantidad en letras" es de solo lectura; el usuario no puede modificarlo directamente.
* El apartado "Detalle de documentos a presentar" es un campo de texto editable donde el usuario puede escribir o el sistema puede mostrar los documentos requeridos según las condiciones del crédito.
* El apartado de documentos se muestra en color rojo y con
  formato destacado para llamar la atención del usuario.

---
## Historia 16: *[CYR]* [Solicitud de Préstamos] Pantalla de información de contacto del solicitante

Descripción
**Yo como:** oficial de crédito o usuario del sistema
**Quiero:**  visualizar los datos de contacto del asociado solicitante en la sección de Información de Solicitante
**Para:** verificar que la información de ubicación y contacto esté completa y actualizada al tramitar la solicitud

### ### Criterios de aceptación:
* La sección muestra la lista de direcciones del asociado con
  las columnas: tipo de dirección, departamento, municipio,
  distrito, colonia-barrio y dirección.
* La sección muestra la lista de correos electrónicos del
  asociado con las columnas: tipo de correo, email y si es
  el correo principal.
* La sección muestra la lista de teléfonos del asociado con
  las columnas: tipo de teléfono, número y si es el teléfono
  principal.
* Todas las listas son de solo consulta; la información proviene
  del perfil del asociado y no puede modificarse desde esta
  pantalla.
* Si alguna de las listas no tiene registros, la tabla correspondiente se muestra vacía sin generar error.

---
## Historia 17: *[CYR]* [Solicitud de Préstamos] Pantalla de situación económica del solicitante

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:** registrar si el solicitante es contribuyente de IVA
        y si lleva contabilidad formal
**Para:**  documentar las características económicas básicas del
      solicitante como parte del expediente del crédito

### Criterios de aceptación:
* El campo "Es Contribuyente de IVA" se presenta con dos opciones
  seleccionables: Sí y No.
* El campo "Lleva Contabilidad" se presenta con dos opciones
  seleccionables: Sí y No.
* Ambos campos son obligatorios antes de guardar la solicitud;
  deben tener una opción seleccionada.
* Solo puede seleccionarse una opción por campo; no se permite
  dejar ambas sin seleccionar ni seleccionar ambas a la vez.

---
## Historia 18: *[CYR]* [Solicitud de Préstamos] Pantalla de registro de ingresos del solicitante

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:**  registrar los ingresos del solicitante en la sección
        de situación económica
**Para:**  documentar las fuentes de ingresos del asociado como
      parte del análisis de capacidad de pago

### Criterios de aceptación:
* La sección muestra una lista desplegable con los tipos de
  ingresos disponibles para seleccionar.
* La sección muestra un campo numérico para ingresar el monto
  del ingreso; no acepta texto y el campo debe permitir decimales
* Un botón de agregar permite guardar el tipo e ingreso
  seleccionados y añadirlos a la tabla de ingresos.
* La tabla de ingresos muestra las columnas: tipo de ingreso
  y valor.
* Cada registro de la tabla tiene una opción para eliminarlo
  de la lista.
* Si se intenta agregar un ingreso sin seleccionar tipo o
  sin ingresar monto, el sistema muestra un mensaje indicando
  los campos requeridos.

---
## Historia 19: *[CYR]* [Solicitud de Préstamos] Pantalla de registro de egresos del solicitante

Descripción
**Yo como:** usuario del sistema financiero
**Quiero:**  registrar los egresos del solicitante en la sección
        de situación económica
**Para:**  documentar las obligaciones de gasto del asociado como
      parte del análisis de capacidad de pago

### Criterios de aceptación:
* La sección muestra una lista desplegable con los tipos de
  egresos disponibles para seleccionar.
* La sección muestra un campo numérico para ingresar el monto
  del egreso; no acepta texto y el campo debe permitir decimales.
* Un botón de agregar permite guardar el tipo y monto del
  egreso seleccionados y añadirlos a la tabla de egresos.
* La tabla de egresos muestra las columnas: tipo de egreso
  y valor.
* Cada registro de la tabla tiene una opción para eliminarlo
  de la lista.
* Si se intenta agregar un egreso sin seleccionar tipo o
  sin ingresar monto, el sistema muestra un mensaje indicando
  los campos requeridos.

# FIN DEL DOCUMENTO

Total de historias generadas: 14

  Historia  1 - Pantalla de búsqueda de asociado para nueva solicitud
  Historia  2 - Pantalla de resultados de búsqueda de asociado
  Historia  3 - Pantalla de asignación de asociado a la solicitud
  Historia  4 - Pantalla de validaciones y alertas al asignar un asociado
  Historia  5 - Pantalla de selección de línea de crédito y clasificación
  Historia  6 - Pantalla de campos de catálogos del formulario principal
  Historia  7 - Pantalla de perfil de crédito del solicitante
  Historia  8 - Pantalla de ingreso de términos financieros del préstamo
  Historia  9 - Pantalla de visualización de cálculos automáticos
  Historia 10 - Pantalla de cantidad en letras y documentos a presentar
  Historia 11 - Pantalla de información de contacto del solicitante
  Historia 12 - Pantalla de situación económica del solicitante
  Historia 13 - Pantalla de registro de ingresos del solicitante
  Historia 14 - Pantalla de registro de egresos del solicitante

SEGMENTACIONES APLICADAS (HU originales → historias resultantes):
  HU Búsqueda de asociado          → Historias 1 y 2   (formulario + resultados)
  HU Asignar solicitud             → Historia  3        (sin cambios)
  HU Validaciones al asignar       → Historia  4        (sin cambios)
  HU Parametrización y clasificac. → Historias 5 y 6   (línea/clasificac. + resto)
  HU Perfil de crédito             → Historia  7        (sin cambios)
  HU Plan de Financiamiento        → Historias 8, 9, 10 (editables + calculados + letras/docs)
  HU Información de Solicitante    → Historia 11        (sin cambios)
  HU Situación económica           → Historia 12        (sin cambios)
  HU Ingresos de situación econom. → Historias 13 y 14  (ingresos + egresos)

==================================================================


## HU nueva