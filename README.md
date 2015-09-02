# nosnmp-hack-observium

Hack to add devices without snmp to observium

<h3>requirements </h3>
  
<li>  python
<li>  iptables
<li>  pysnmp

<h3>Usage</h3>
<li>login to your observium box<br>
<li>run python nosnmp_responder (default in port 1161)<br>
<li>iptables -I OUTPUT -j DNAT -t nat -d *****YOURDEVICE IP******* --to-destination 127.0.0.1 -p udp --dport 1161<br>
<li>/opt/observium/add_device.php *****YOURDEVICE IP******* public v1 1161 udp   OR add it from browser <br>  

<h3>Future</h3>
<li>



  
