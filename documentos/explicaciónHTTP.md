### Las sesiones tipicas HTTP:

Estas tienen 3 fases, en la primer fase el cliente establece una conexion TCP, o establece una conexion correspondiente al protocolo que posea la capa de transporte. 
En la segunda fase, el cliente envia un pedido y espera una respuesta. En la tercera fase, el servidor procesa su pedido y responde con un codigo de estado y los datos correspondientes
(el codigo de estado sirve para que el servidor pueda hacerle saber al cliente si su peticion fue procesada de forma correcta). 

Luego de la tercera fase la sesion no se cierra por lo que el cliente puede seguir mandando peticiones, lo que implica que tanto la segunda como la tercera fase pueden ser repetidas las veces que sean necesarias.
Esto se debe a un cambio que se hizo en el protocolo HTTP 1.1.

### Establecer una conexión:

Dentro de un protocolo cliente-servidor siempre que el cliente inicia una conexion, inicia una conexion HTTP en la capa de comunicación que corresponda, comúnmente TCP

En el protocolo TCP el puerto para conexiones HTTP, es el puerto 80, tiene variantes como el 8000 o el 8080. La URL de la pagina posee el nombre del dominio y el numero del puerto, aunque el numero del puerto puede ser omitido cuando es el puerto 80. En una conexión cliente-servidor, no se permite que el servidor mande información al cliente sin una petición exacta debido al modelo cliente-servidor, esto es una problematica a la cual se le dio una solución parcial, haciendo un ping al servidor de forma periodica, a traves de XMLHTTPRequest, Fetch, APIs u otros protocolos.

### Mandar una petición: 

El cliente puede mandar peticiones de información, sus peticiones consisten en directivas de texto los cuales estan separados mediante CRLF (retorno de carro, y cambio de linea), esto se separa en 3 partes. 

- La primera parte contiene una linea la cual contiene un metodo y sus parametros, la direccion del documento solicitado: la URL entera, sin indicar el protocolo o el nombre del dominio y aparte la version del protocolo HTTP.

- La segunda parte esta conformada por un bloque de lineas consecutivas que representan las cabeceras de la petición HTTP. Le dicen al servidor que información es adecuada, que lenguaje utilizar u otros datos que modifiquen su comportamiento, como que evite enviar una respuesta si ya esta cacheada, estos bloques terminan con una linea en blanco.

- la tercera parte, es opcional y esta puede tener partes para ser usadas por el metodo post.

#### Ejemplo de peticion:

  GET / HTTP/1.1\
  Host: developer.mozilla.org\
  Accept-Language: fr

### Metodos en una petición:

El protocolo HTTP posee un conjunto de metodos de peticiones en donde se indican las acciones que se solicitan cuando se recibe información, los mas comunes son el GET y el POST

- El GET solicita algun dato en especifico, este metodo solo hace peticiones de datos.

- El POST le envia datos al servidor para que este pueda cambiarle datos al servidor.

### Respuesta del servidor:

Luego de que un usuario realize una petición, despues de que el servidor lo procesa, luego le responde. Esta respuesta esta compuesta por directivas de texto, separadas por CRLF y dividida en 3 partes.

- La primer linea, posee el estado del servidor, la cual se da a traves de la confirmación de version de HTTP que se usa con una corta descripción de texto 

- Las lineas que siguen representan cabeceras de HTTP, otorgandole al cliente información sobre los datos enviados, desde su tamaño, algoritmos de compresión utilizados o sugerencias de cacheoy estas tambien finalizan con una linea vacia. 

- El ultimo bloque, puede contener opcionalmente los datos

#### Ejemplo de respuesta de servidor:

HTTP/1.1 200 OK \
Date: Sat, 09 Oct 2010 14:28:02 GMT \
Server: Apache \
Last-Modified: Tue, 01 Dec 2009 20:18:22 GMT \
ETag: "51142bc1-7449-479b075b2891b" \
Accept-Ranges: bytes \
Content-Length: 29769 \
Content-Type: text/html 

[inicio](../README.md)