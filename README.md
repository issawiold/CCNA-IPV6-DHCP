# CCNA-IPV6-DHCP

In the router 

\>en

\#conf t

fig#ipv6 unicast-rout

fig#int g#/#

if#ip address 2001::1/64

if#ex

fig#ipv6 dhcp pool <name>

dhcpv6#address pref 2001::2/64

##Now the server is set assign it to the interface/port

fig#int g#/#

if# ipv6 nd managed-config-flag (I usually use it ipv6 nd mana)

if# ipv6 dhcp server <name>  
