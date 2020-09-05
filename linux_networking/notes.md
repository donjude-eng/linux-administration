## TCP?IP
 1. Used for network communications
 2. TCP = Tranmission Contron Protocol
 3. Ip = Internet Protocol

* TCP -control data exchane
* Ip -sends data from one device to another

## Communication needs the below details.
 ![Linux Directories](communication.PNG?raw=true "Title")

# DNS hostname

![Linux Directories](subnet.PNG?raw=true "Title")
8 FQDN = fully qualified domain anme
 1. webprod01.mycompany.com

* TLD
 1. .com., .net, .org,etc

* Domains
1. below (to the left of) TLD

* sub domain
 1. elow (to the leftof) the domain
 2. webprod01.ny.us.mycompany.com

## To get the ip address
* ip addr
* ifconfig

# hostnames
* human readable name for an IP address
 1. webprod01 = 10.109.155.174

# Network Port
* Port identifies the services on a host.
* Port 1 - 1023 are well known ports.
  1. 22 -SSH
  2. 25 -SMTP
  3. 80 -HTTP
  4. 143 - IMAP
  5. 389 - LDAP
  6. 443 - HTTPS

* webserver recive traffic on 443 port.

## DHCP
![Linux Directories](dhcpconfigure.PNG?raw=true "Title")

# Network troubleshooting
* Ping > Ping a host icmp packet to the host and wait for the reply
* ping -c 3 google.com
