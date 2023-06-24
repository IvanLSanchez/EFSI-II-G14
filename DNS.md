# DNS
Es un protocolo de traduccion entre los dominios web y las direcciones IP, permitiendo asi la comunicacion entre los usuarios e internet.
     
El protocolo esta conformado por 3 elementos:
   - Servidores DNS: Bases de datos que almacenan estos datos anteriormente dichos
   - Clientes DNS: IP de los servidores DNS, instaladas en nuestros dispositivos, a las cuales nosotros como ususarios haremos peticiones
   - Zona de autoridad: son servidores encargados de resolver un conjunto de dominios determinado (.com, .es, etc.).
     
Los pasos que realiza este protocolo son los siguientes:
   1. El usuario busca la web X desde el navegador.
   2. La petición se envía al servidor DNS.
   3. Este busca en su base de datos la dirección IP del servidor y los dominios que en él se alojan.
   4. Cuando la encuentra, le dice al servidor que el dominio está alojado en el servidor Y.
   5. Entonces, Y devuelve la consulta al cliente (el navegador del móvil en nuestro caso) y comienza la transferencia de datos.
   
Como dato curioso entre los servidores DNS mas utilisados son: Google DNS, Open DNS, Cloudfare DNS, Comodo Secure DNS, Quad9, DNS.Watch, AdGuard DNS y Dyn 

[inicio](README.md)
