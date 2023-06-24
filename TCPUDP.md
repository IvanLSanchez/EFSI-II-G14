# Protocolo TCP:
Permite que las aplicaciones puedan comunicarse con garantías independientemente de las capas inferiores del modelo TCP/IP. Por lo que los routers solamente tienen que enviar los segmentos, sin asegurarse de que esos segmentos lleguen correctamente o no a su destino. Este otorga soporte a muchos protocolos en la capa de "aplicación", dentro de ellos estan HTTP, HTTPS, POP3 y SMTP. También se utiliza TCP en protocolos tan importantes como FTP, FTPES y SFTP para transferir archivos desde un origen a un destino, e incluso el protocolo SSH para administrar equipos de forma local y remota de manera segura utiliza el protocolo TCP.

# Protocolo UDP:
Este protocolo principalmente tiene la misma funcion que el TCP, pero este en cambio hace que los routers solamente tengan que enviar los datagramas, una unidad de medida en UDP. Este protocolo al igual que el TCP da soporte a protocolos en la capa de aplicación, pero este da soporte a los DNS e incluso el protocolo DHCP, para conseguir y proporcionar un direccionamiento IP automaticamente. El protocolo permite el envío de datagramas sin necesidad de establecer previamente una conexión, tan solo es necesario tener abierto un socket en el destino para que acepte los datagramas del origen.

[inicio](README.md)
