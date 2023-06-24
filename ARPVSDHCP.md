# Protocolo Arp vs Protocolo DHCP

* El protocolo Arp: 

Se encarga de encontrar la direcciòn MAC, enviando un mensaje ARP Request a la direccion MAC y el dispositivo le responde con un mensaje ARP Reply, donde devuelve la IP. Este protocolo es utilizado tanto en Ethernet como en Routers cuando tienen que comunicarse con un host o cuando tienen que enviar un paquete a un host a traves de otro router. 

Este protocolo puede recibir ataques de spoofing, que hace creer a los equipos de la red local que un equipo es el router y por ese equipo pasa todo el trafico de datos y esa informaciòn puede ser atrapada o modificada, esto se puede evitar configurando los switches poniendo una pareja de dirección IP-MAC asociada a un determinado puerto y a una determinada VLAN. De esta forma un atacante no podria hacer el ataque o interceptar informaciòn.
Este protocolo no existe en redes IPv6, su funcionalidad la hereda el protocolo ICMPV6. En cambio en redes IPv4 ARP es un protocolo muy importante, sin el no habria comunicaciòn. cuando se hacen solicitudes ARP para un host que no existe es frecuente que aumenten los intervalos de tiempo entre dichas solicitudes hasta que eventualmente ARP se da por vencido.

Las ventajas que tiene este protocolo es que: 
Las direcciones MAC se pueden conocer fácilmente si conoce la dirección IP del mismo sistema.
Los nodos finales no deben configurarse para «conocer» las direcciones MAC.
El objetivo de ARP es habilitar cada host en una red que le permita crear un mapeo entre las direcciones IP y las direcciones físicas.
El conjunto de asignaciones o tablas almacenadas en el host se denomina tabla ARP o caché ARP.

* El protocolo DHCP:

Este protocolo proporciona direcciones ip tando de forma dinamica como estaticata a los hosts que lo soliciten, este protocolo le va a asignar una direccion IP a cualquier dispositivo que se conecte, esta va a estar asignada dentro de un rango configurado dentro del servidor DHCP, que usualmente tiene un rango de 100 direcciones o todas las direcciones de host de una subred a excepcion de la primera, la cual tiene el router. La configuraciòn que se consiga depende del fabricante del router y su configuraciòn predeterminada, que sin importar cual de las 2 sea ambas son utiles, a menos que se busque conectar mas de 100 dispositivos a una red, en ese caso no sera util la primer configuraciòn.

DCHP permite reservar direcciones fijas ingresando dispositivos en la tabla "Static DHCP" del router, de no hacerlo sin importar el equipo que sea le otorgara una direccion dinamica cada vez que se conecte al router, esto significa que una vez puede tener la direcciòn 192.168.1.74 y en otra vez puede ser 192.128.1.143.
Algunos equipos que necesitan tener siempre la misma direccion ip, porque se haya hecho reenvio de puertos o se haya abierto la DMZ por motivo de seguridad, este protocolo permite dar una ip fija a la MAC que queramos.

Ventajas de este protocolo:
Gestión automática de direcciones IP, incluida la prevención de problemas de direcciones IP duplicadas.
Permite la compatibilidad con clientes BOOTP, por lo que puede cambiar fácilmente sus redes de BOOTP a DHCP.
Da poder al administrador para establecer tiempos de arrendamiento, incluso en direcciones IP asignadas manualmente.
Permite al administrador configurar tipos de opciones de DHCP adicionales, además de lo que es posible con BOOTP.
Permite la asociación de dos o más grupos de direcciones IP dinámicas en redes (o subredes) IP separadas. (Este es el soporte básico para redes secundarias. Permite que un enrutador actúe como un relé BOOTP para una interfaz que tiene más de una dirección IP de red o subred IP)


 [inicio](README.md)
