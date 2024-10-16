Bueno, no puedo garantizar nada. Si alguno de estos estándares te parece útil para tu trabajo, debes estar dispuesto a profundizar en su especificación y realmente entenderlo (o comprar un libro que lo cubra con más detalle). No tengo espacio para dar más que una visión general básica de estándares como Siren, CoAP y Hydra. Sin mencionar que ofrecer muchos detalles aburriría a todos los lectores que no necesitan esos estándares en particular para su trabajo.

Al navegar por el bosque de estándares, es útil tener en cuenta que no todos los estándares tienen la misma fuerza. Algunos están extremadamente bien establecidos, son utilizados por todos y, si vas en su contra, te estás causando muchos problemas. Otros estándares son solo la opinión de una persona, y esa opinión podría no ser mejor que la tuya.

Encuentro útil dividir los estándares en cuatro categorías: **estándares por decreto**, **estándares personales**, **estándares corporativos** y **estándares abiertos**. Utilizaré estos términos a lo largo del libro, así que déjame explicar cada uno con más detalle antes de continuar.

### Estándares por Decreto

Los estándares por decreto no son realmente estándares; son comportamientos. Nadie estuvo de acuerdo con ellos. Son simplemente una descripción de cómo alguien hace las cosas. El comportamiento puede estar documentado, pero falta la suposición central de un estándar: que otras personas deberían hacer las cosas de la misma manera.

Prácticamente todas las API hoy en día son un estándar por decreto, un diseño único asociado a una empresa específica. Por eso hablamos de la "API de Twitter", la "API de Facebook" y la "API de Google+". Es posible que necesites entender estos diseños para hacer tu trabajo y que escribas tus propios clientes para estos diseños, pero a menos que trabajes para la empresa en cuestión, no se espera que utilices este diseño para tu API. Si reutilizas un estándar por decreto, no decimos que tu API cumpla con un estándar; decimos que es un clon.

El principal problema que intento resolver en este libro es que cientos de años-persona de trabajo de diseño están encerrados en estándares por decreto donde no pueden ser reutilizados. Esto debe terminar. Diseñar una nueva API hoy en día significa reinventar una larga serie de ruedas. Una vez que tu API esté terminada, tus desarrolladores de clientes tendrán que reinventar ruedas correspondientes en el lado del cliente.

Incluso en las circunstancias ideales, tu API será un estándar por decreto, ya que tus requisitos comerciales serán ligeramente diferentes a los de los demás. Pero idealmente, un estándar por decreto sería solo una ligera capa sobre otros estándares.

Cuando describa un estándar por decreto, enlazaré a su documentación legible por humanos.

### Estándares Personales

Los estándares personales son estándares: se te invita a leer los documentos e implementar los estándares por ti mismo, pero no son más que la opinión de una persona. El estándar Maze+XML...
