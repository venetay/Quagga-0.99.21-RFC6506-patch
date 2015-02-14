# Quagga-0.99.21 RFC6506-patch

The RFC6506 patch is applied to the code 

Steps to test/run the developed patch file on quagga-0.99.21 : 
As per RFC, implementation is done by TCS in order to provide 
authentication support on both interface and area. 
Commands to be used are as follows: 
For an interface(under interface <i/f name>)- 
ipv6 ospf6 sha-256-authentication [command to set AT-bit 
on interface] 
ipv6 ospf6 sha-256-key <key-id> sha-256 <password> 
[command to attach key-id and password to the packets] 
For an area (under router ospf6)- 
area <area-id> sha-256-authentication [command to set 
AT-bit on area] 
In order to authenticate OSPFv3 packets, please provide combination of 
both AT bit on an interface/area and key-id with sha-256 password. 

Tata Consultancy Services (TCS) providing the implementation code for RFC-6506, developed and tested on 
quagga-0.99.21 version. 

http://www.gossamer-threads.com/lists/quagga/dev/24965

http://tools.ietf.org/html/rfc6506

http://tools.ietf.org/html/rfc7166
