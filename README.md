# objetos location
## Para que se usa el objeto location en Javascript

El objeto Location en JavaScript es una herramienta poderosa que le permite a los desarrolladores web interactuar con la URL actual de una página web. Si bien es posible que ya estés familiarizado con conceptos básicos, como **document.location** o **window.location**, este artículo explorará en detalle cómo aprovechar al máximo el objeto Location en JavaScript para realizar tareas avanzadas y útiles en el desarrollo web.

## Propiedades de location

`Location.href` (en-US)

Es un `DOMString` que contiene la URL completa. Si es cambiada, el documento asociado navegará a la nueva pagina. Puede ser cambiada desde un origen diferente que el asociado al documento.

`Location.protocol` (en-US)

Es un `DOMString` que contiene el esquema del protocolo de la URL, incluyendo el ':' final.

`Location.host` (en-US)

Es un `DOMString` que contiene el host, el cual esta compuesta por: hostname, ':', y el port de la URL.

`Location.hostname` (en-US)

Es un `DOMString` que contiene el dominio de la URL.

`Location.port` (en-US)

Es un `DOMString` que contiene el numero del puerto de la URL.

`Location.pathname` (en-US)

Es un `DOMString` que contiene el '/' inicial, seguido por la ruta de la URL.

`Location.search` (en-US)

Es un `DOMString` que contiene un '?' seguido por los parametros o el "querystring" de la URL. Navegadores modernos proveen URLSearchParams (en-US) y URL.searchParams (en-US) para hacer mas facil de obtener los parametros desde el querystring.

`Location.hash` (en-US)

Es un `DOMString` que contiene un '#' seguido por el fragmento identificador de la URL.

`Location.username` (en-US)

Es un `DOMString `que contiene el username (usuario) especificado antes del dominio.

`Location.password` (en-US)

Es un `DOMString `que contiene el password (contraseña) especificado antes del dominio.

`Location.origin` Read only
Es un `DOMString `que contiene la forma canonica del origin (origen) de la URL.

## Metodos de location 

La interface *Location* no hereda ningun metodo, pero los implementa desde URLUtils.

`Location.assign() `(en-US)
Carga el recurso en la URL proporcionada en el parámetro.

`Location.reload()`
Recarga el recurso desde la URL actual. Si unico y opcional parametro es `Boolean `(en-US), el cual, cuando es **true**, hace que la pagina siempre sea recargada desde el servidor. Si es **false** o no es especificado, el navegador puede recargar la pagina desde su cache.

`Location.replace() `(en-US)
Reemplaza el recurso actual por el recibido como URL. La diferencia con el metodo assign() es que luego de usar replace() la pagina actual no va a ser guardada en la sesión `History, `esto significa que el usuario no podrá usar el boton Atras para navegar a esta.

`Location.toString() `(en-US)
Retorna un `DOMString ` que contiene la URL completa. Es un sinonimo de URLUtils.href, aunque este no puede ser utilizado para modificar el valor.

