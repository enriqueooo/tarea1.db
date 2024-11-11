de formulario (la plantilla), que usted completa para crear un documento. Entonces envías eso
documento al servidor con una solicitud POST.
Nuevamente, el Capítulo 6 cubre Colección+JSON en detalle, así que aquí está la versión rápida. Mira a
El gran objeto que les mostré antes. Su propiedad de plantilla es el menú "objeto de plantilla".
mencionado en la especificación Collection+JSON:
 {
 ...
 "plantilla": {
 "datos": [
 {"prompt": "Texto del mensaje", "nombre": "texto", "valor":""}
 ]
 }
Para completar la plantilla, reemplazo la cadena vacía debajo del valor con la cadena que quiero
publicar:
 { "plantilla":
 {
 "datos": [
 {"prompt": "Texto del mensaje", "nombre": "texto", "valor": "¡Calamar!"}
 ]
 }
 }
Luego envío la plantilla completa como parte de una solicitud HTTP POST:
ENVIAR /api/HTTP/1.1
Anfitrión: www.youtypeitwepostit.com
Tipo de contenido: aplicación/vnd.collection+json
{ "plantilla":
 {
 "datos": [
 {"prompt": "Texto del mensaje", "nombre": "texto", "valor": "¡Calamar!"}
 ]
 }
}
(Tenga en cuenta que el tipo de contenido de mi solicitud es application/vnd.collection+json. Esto
La plantilla completa es un documento Collection+JSON válido por sí solo).
El servidor responde:
HTTP/1.1 201 creado
Ubicación: http://www.youtypeitwepostit.com/api/47210977342911065
El código de respuesta 201 (Creado) es un poco más específico que 200 (OK); significa que
todo está bien y que se creó un nuevo recurso en respuesta a mi solicitud. El
El encabezado de ubicación proporciona la URL del recurso recién nacido.
