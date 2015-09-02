# noip-hack-observium

Hack to enable snmp incapable devices to observium

requirements 
  
  python
  iptables
  pysnmp
  
login to your observium box
run python noip_responder (default in port 1161)
iptables -I OUTPUT -j DNAT -t nat -d *****YOURDEVICE IP******* --to-destination 127.0.0.1 -p udp --dport 1161
/opt/observium/add_device.php *****YOURDEVICE IP******* public v1 1161 udp



  
