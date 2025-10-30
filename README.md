# CCNA-IPV6-DHCP

In the router 

\>en

\#conf t

fig#ipv6 unicast-rout

fig#int g#/#

if#ip address 2001::1/64

if#ex

-now that ipv6 routing is enabled on the router and the inter face have been assigned an ipv6 let us configure the ipv6 pool-

fig#ipv6 dhcp pool <name>

dhcpv6#address pref 2001::2/64

## Now the server is set assign it to the interface/port

fig#int g#/#

if# ipv6 nd managed-config-flag (I usually use it ipv6 nd mana)

if# ipv6 dhcp server <name>  ( make sure the nme is correct it's case senstive and you must use the name that you assigned to the pool)


---------------------

## for troubleshooting

ping <ipv6>

show ipv6 dhcp pool

show ipv6 dhcp int

show ipv6 dhcp binding 



