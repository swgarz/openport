
https://ping.eu/port-chk/ (para saber mi ip del router)

nmap -PNO -sV 177.247.113.5 -p 80

sudo gedit /etc/apache2/ports.conf (aparece habilitado LISTEN 80)

sudo ufw status

sudo ufw enable

sudo ufw allow 80/tcp

sudo iptables -A INPUT -p tcp --dport 80 -j ACCEPT

sudo apt-get install iptables-persistent (no me deja abierto el puerto)

