# Directadmin-1.60.4-Nulled
Directadmin 1.60.4 Nulled + Working License File ( Unlimited Account, Unlimited Domains )


yum -y install nano wget perl

wget https://raw.githubusercontent.com/cuibapvh/DA-1.60.4-Nulled/master/setup.sh

chmod +x setup.sh

./setup.sh

Client ID (uid):  9192
License ID (lid): 919233

firewall-cmd --zone=public --add-port=21/tcp --permanent

firewall-cmd --zone=public --add-port=22/tcp --permanent

firewall-cmd --zone=public --add-port=25/tcp --permanent

firewall-cmd --zone=public --add-port=80/tcp --permanent

firewall-cmd --zone=public --add-port=443/tcp --permanent

firewall-cmd --zone=public --add-port=465/tcp --permanent

firewall-cmd --zone=public --add-port=2222/tcp --permanent

firewall-cmd --reload

systemctl restart directadmin

cd /usr/local/directadmin/conf/

systemctl stop directadmin

rm -rf /usr/local/directadmin/conf/license.key

wget -O /usr/local/directadmin/conf/license.key https://raw.githubusercontent.com/cuibapvh/DA-1.60.4-Nulled/master/license.key

chmod 600 /usr/local/directadmin/conf/license.key

chown diradmin:diradmin /usr/local/directadmin/conf/license.key

ifconfig eth0:92 37.97.247.189 netmask 255.255.255.0 up

echo 'DEVICE=eth0:92' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

echo 'IPADDR=37.97.247.189' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

echo 'NETMASK=255.255.255.0' >> /etc/sysconfig/network-scripts/ifcfg-eth0:92

systemctl restart network

/usr/bin/perl -pi -e 's/^ethernet_dev=.*/ethernet_dev=eth0:92/' /usr/local/directadmin/conf/directadmin.conf

systemctl start directadmin

Done:)
