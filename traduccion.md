de formulario (la plantilla), que usted completa para crear un documento. Entonces envías eso  
documento al servidor con una solicitud POST.  
Nuevamente, el Capítulo 6 cubre Colección+JSON en detalle, así que aquí está la versión rápida. Mira a  
El gran objeto que les mostré antes. Su propiedad de plantilla es el menú "objeto de plantilla".  
mencionado en la especificación Collection+JSON:

```json
{
  ...
  "plantilla": {
    "datos": [
      {"prompt": "Texto del mensaje", "nombre": "texto", "valor":""}
    ]
  }
}
{ 
  "plantilla": {
    "datos": [
      {"prompt": "Texto del mensaje", "nombre": "texto", "valor": "¡Calamar!"}
    ]
  }
}
ENVIAR /api/HTTP/1.1  
Anfitrión: www.youtypeitwepostit.com  
Tipo de contenido: aplicación/vnd.collection+json

{
  "plantilla": {
    "datos": [
      {"prompt": "Texto del mensaje", "nombre": "texto", "valor": "¡Calamar!"}
    ]
  }
}
HTTP/1.1 201 creado  
Ubicación: http://www.youtypeitwepostit.com/api/47210977342911065
