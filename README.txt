
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







































