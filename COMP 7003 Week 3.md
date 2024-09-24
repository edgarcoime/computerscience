## Ports
1. Purpose of Ports
	1. Ports uniquely identify 
2. Structure of ports
	1. Ports are represented by 16-bit unsigned integers
	2. Well known ports (0-1023)
		1. These ports are reserved for commonly used services and protocols such as http, ftp, dns, and ssh
	3. Registered ports (1024-49151)
		1. These ports are ysed by user applicatinos and services less universally defined by well-known ports
	4. Dynamic/private Ports (49152-65535)
		1. when you make a connection it might just give you one of these ports
3. How ports work
	1. Sending and receiving from the same port 
	2. The transport layer (tcp or udp) headers 
## UDP
1. Simple protocol that is light weight and fast
2. Online gaming
	1. games require low-latency communication b etween player and games 
## TCP
1. Has a sequence number which keeps track of how the packets should numbered