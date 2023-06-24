# EFSI 2

# TP1

# Tabla Comparativa

<table class="tg">
<colgroup>
<col style="width: 105px">
<col style="width: 25px">
<col style="width: 90px">
<col style="width: 26px">
<col style="width: 79px">
<col style="width: 134px">
<col style="width: 185px">
<col style="width: 167px">
<col style="width: 223px">
</colgroup>
<thead>
  <tr>
    <th class="tg-baqh" colspan="6">Modelo de Capas (Layers)</th>
    <th class="tg-baqh" rowspan="2">Protocolos de red (que nos interesan)</th>
    <th class="tg-baqh" rowspan="2">Caracteristica principal</th>
    <th class="tg-0lax" rowspan="2">Dispositivo de conexion de red</th>
  </tr>
  <tr>
    <th class="tg-baqh">Tipos de capas</th>
    <th class="tg-baqh" colspan="2">Modelo OSI</th>
    <th class="tg-baqh" colspan="2">Modelo TCP/IP</th>
    <th class="tg-baqh">Unidad de datos de Protocolo (PDU)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh" rowspan="4">capas del host <br>"software"</td>
    <td class="tg-baqh">7</td>
    <td class="tg-baqh">Aplication</td>
    <td class="tg-baqh" rowspan="3">4</td>
    <td class="tg-baqh" rowspan="3">process</td>
    <td class="tg-baqh" rowspan="3">Datos</td>
    <td class="tg-baqh" rowspan="3">DNS FTP SSH SMTP POP SNMP DHCP HTTP/S</td>
    <td class="tg-baqh" rowspan="3">Aplicaciones</td>
    <td class="tg-baqh" rowspan="4">Aplicaciones // Arquiectura cliente-servidor</td>
  </tr>
  <tr>
    <td class="tg-baqh">6</td>
    <td class="tg-baqh">Presentation</td>
  </tr>
  <tr>
    <td class="tg-baqh">5</td>
    <td class="tg-baqh">Session</td>
  </tr>
  <tr>
    <td class="tg-baqh">4</td>
    <td class="tg-baqh">Transporte</td>
    <td class="tg-baqh">3</td>
    <td class="tg-baqh">transporte</td>
    <td class="tg-baqh">Segmento</td>
    <td class="tg-baqh">TCP / UDP</td>
    <td class="tg-baqh">Puertos / Sockets</td>
  </tr>
  <tr>
    <td class="tg-baqh" rowspan="4">Capas de Red<br>"firmware"<br>"Hardware"</td>
    <td class="tg-baqh">3</td>
    <td class="tg-baqh">Network</td>
    <td class="tg-baqh">2</td>
    <td class="tg-baqh">Internet</td>
    <td class="tg-baqh">Paquete</td>
    <td class="tg-baqh">IPV (Ipv4 y IPv6)</td>
    <td class="tg-baqh">Direccion IP</td>
    <td class="tg-baqh">Router / Switch capa 3</td>
  </tr>
  <tr>
    <td class="tg-baqh">2</td>
    <td class="tg-baqh">Data link</td>
    <td class="tg-baqh" rowspan="3">1</td>
    <td class="tg-baqh" rowspan="3">Media</td>
    <td class="tg-baqh">Trama</td>
    <td class="tg-baqh">ARP / MAC</td>
    <td class="tg-baqh">MAC adress</td>
    <td class="tg-baqh">Switch // LAN / WLAN / VLAN / WAN</td>
  </tr>
  <tr>
    <td class="tg-baqh">1</td>
    <td class="tg-baqh">Physical</td>
    <td class="tg-baqh">Bits</td>
    <td class="tg-baqh">IEEE 802.3 (ETHERNET) IEEE 802.11 (WIFI)</td>
    <td class="tg-baqh" rowspan="2">Puerto de Red / Cable</td>
    <td class="tg-baqh">Hub (no se usa)</td>
  </tr>
  <tr>
    <td class="tg-baqh">0</td>
    <td class="tg-baqh">Media</td>
    <td class="tg-baqh">Señal</td>
    <td class="tg-baqh">CABLE UTP (CAT5e Y CAT6), FIBRA OPTICA</td>
    <td class="tg-baqh">Cable UTP / Fibra / WIFI</td>
  </tr>
</tbody>
</table>

*La capa de Medio (Media) no forma parte oficial del Modelo OSI, pero esquematicamente la estudiamos ahi

# Glosario

## Contenido del Glosario :
### Elementos de una red
  *  [Router](documentos/Router.md) 
  *  [Switch](documentos/Switch.md)
  *  [Switch Capa 2 (modelo osi)](documentos/SwitchCapa2(modeloOsi).md)
  *  [Switch Capa 3: Switch (modelo osi)](documentos/SwitchCapa3(modeloOsi).md)   
  *  [Hub](documentos/Hub.md)
  *  [Server](documentos/Server.md)
  *  [Host](documentos/Host.md)
  *  [Firewall](documentos/Firewall.md) 
  *  [IP phone](documentos/IpPhone.md)
  *  [Wireless Access-Point](documentos/WirelessAccessPoint.md)
  *  [Wireless Router](documentos/WirelessRouter.md)
  *  [Wan](documentos/WAN.md)   
  *  [Lan](documentos/Lan.md)
  *  [Media (Medio de Transporte)](documentos/Media.md)
  
### Protocolos
  *  [DNS](documentos/DNS.md)
  *  [FTP](documentos/FTP.md)
  *  [SSH](documentos/SSH.md)
  *  [SMTP](documentos/SMTP.md)
  *  [POP](documentos/POP.md)
  *  [SNMP](documentos/SNMP.md)
  *  [DHCP](documentos/DHCP.md)
  *  [HTTP/S](documentos/httpS.md)
  *  [TCP / UDP](documentos/TCPUDP.md)
  *  [Puertos](documentos/puertos.md)
  *  [IPv4](documentos/ipv4.md)
  *  [IPv6](documentos/ipv6.md) 
  *  [ARP](documentos/ARP.md)
  *  [MAC](documentos/MAC.md) 
  *  [IEEE 802.11](documentos/wifi.md)
  *  [Fibra Optica](documentos/fibraoptica.md)
  
#### Explicación HTTP

  * [Sesion HTTP](explicaciónHTTP.md)
  * [Metodos HTTP](metodosHTTP.md)
  
#### Diferencias entre puertos:
  * [Puertos UDP y TCP](diferenciasUDPTCP.md)

### Unidad de Datos de protocolo (PDU)
  * [Datos](documentos/Datos.md)
  * [Segmento](documentos/Segmento.md)
  * [Paquete](documentos/Paquete.md)
  * [Trama](documentos/Trama.md)
  * [Bits](documentos/Bits.md)
  * [Señal (dbm)](documentos/Señal.md)

  
###   Medios
  * [Conectores](documentos/conectores.md)
    
  * [CABLE UTP (CAT5e y CAT6)](documentos/cableutp.md)
    
  * [Full Duplex (802.3x)](documentos/fullduplex.md)
   
  * [POE (802.3af)](documentos/poe.md)

### extras
  * [ARP vs DHCP](documentos/ARPVSDHCP.md)
  * [Relacion bits de host con cantidad de host](documentos/BitsHost.md)
  * [Protocolo IPv4 vs IPv6](documentos/IPv46.md)

### apuntes de carpeta
  * [Como armar una red](documentos/Comoarmarunared.md)
  * [Como detectar mismas redes](documentos/DetectarmismasRedes.md)
  * [Practica Coloquio](documentos/PracticaColoquio.md)

### videos/articulos utiles
  * [Direccionamiento IPv4 y Subredes (Explicado)](https://youtu.be/SHbBso63X38)
  * [Que es una IP](https://youtu.be/YSVo21r3wBg)
  * [IPv4 vs IPv6](https://blog.hidemyass.com/es/ipv4-ipv6-whats-the-difference)
  * [ip privada vs publica](https://youtu.be/pcYIsXtq3ZM)
