### Introduction
1. In computer networks, data is transmitted in small, manageable units called packets
2. Packets carry data and control information needed for successful delivery
### Packet Structure Overview
1. Packet Header
	1. Contains essential controller information for data transmission
2. Packet Payload
	1. Core content of the packet, containing actual data that needs to be transmitted 
3. Packet Trailer
	1. Packett railer plays a crucial role in maintaining data integrity during transmission
### How packets travel through network
1. Bandwidth:
	1. The capacity of VALID data that is able to be sent through the network
## Routing
1. Introduction
	1. Process of directing a packet from source to destination across one or more networks
	2. Routers are responsible for this usually a physical router device or it can be embedded in hardware 
		1. ie. a computer with router software
2. How routing works
	1. Looking at a destination address and deciding the best next step, or hop, for packet 
	2. ttl: time to live shows how much the packet will try to send until it won't send anymore
### Types of routing
1. Static routing
	1. Network administrators manually configure routes for data tot ravel across a network
	2. Once routes are made they are usually fixed
2. Dynamic routing
	1. Leverages routing protocols that automatically adjust paths based onr eal-time network conditions
	2. These protocols continuously monitor the network and can dynamically reroute traffic
### Routing challenges
1. Network congestion
	1. Occurs when congestion is present in the network
2. Network failures
## MAC address
1. Introduction
	1. Every physical device has a mac address
	2. A mac address is permanently embedded into the device's hardware
	3. MAC adresses are spoofable
	4. Every device that is connected to a network has a macaddress
2. Structure of a mac address
	1. An example of a mac address
		1. 00:1A:2b:3c:4d:5E
		2. usually make and network cards
3. MAC address functionality in Networking
	1. They help ensure that data is sent to the correct device 
	2. when data is transmitted the device creates a frame that includes both the source MAC address and the destination MAC address
4. Mac addresses and Data transmission
	1. Sending Data
	2. Frame Broadcast
	3. Destination identification
	4. Data reception
5. Types of MAC addresses
	1. Unicast MAC addresses
	2. Multicast  MAC address
	3. Broadcast MAC address
## MAC address filtering
1. Filtering allowing only specific mac addresses but remember that you can spoof mac addresses so it doesn't even matter
## MAC address spoofing



## Ethernet
1. Introduction
	1. operates by sending frames across the network
2. What is ethernet
3. Ethernet frame structure
	1. Preamble:
		1. a 7-byte sequence that helps synchronize these ndera nd receiver
	2. Start Frame Delimiter (SFD):
		1. a 1-byte field that indicates the start of the frame
	3. Destination MAC address:
		1. The mac address of the receiving device
	4. Source MAC address
		1. The mac address of the source device
	5. Ethertype:
		1. A field that indicates the type of payload being transmitted
	6. Payload:
		1. The actual data being transmitted can range from 46 to 1500
	7. Frame Check Sequence FCS:
		1. A 4-byte field for error checking to ensure data integrity
4. Data transmission in ethernet
	1. When a device wants to send data, it encapsulates it in an ethernet frame and broadcasts it onto the network
5. Collision Detection and CSMA/CS
	1. In older or unswitched ethernet networks, devices could transmit data simultaneously leading to collisions
	2. Carrier Sense
	3. Multiple Access
	4. Collision Detection
	5. Collision Resolution
## Addressing
1. Introduction
	1. Two types of addressing are essential are MAC and IP addresses
	2. Allows us to communicate locally and remotely
2. Why do we need addressing
	1. IP addresses are easy to remember
3. What is an IP address
	1. An IP (internet protocol) is a logical identifier for communication across different networks
4. IPv4 vs IPv6: Why do they coexist?
	1. To upgrade from 4 to 6 EVERY hardware network needs to be replaced
	2. This would cost a monumental amount of money 
	3. If it broke don't fix it mentality so they needed to keep legacy 
5. Key differences between IPv4 and IPv6 
	1. Much larger address scope 
	2. No need for NAT to translate local machines that share the same ip ad the router
6. How addressing enables Data transmission
## MAC-IP Addresses
1. Introduction
	1. IP packet gets embedded into the ethernet packet
2. The role of MAC and IP addresses in Data Transmission
	1. for devices to communicate effectively, especially whens ending data across different networks, the system must resolve the recipient's IP address to a MAC address
3. ARP: Mapping IP to MAC in IPv4 Networks
	1. ARP Request
	2. ARP Reply
	3. Update ARP Cache
	4. Transmission
4. NDP: Address Mapping in IPv6 Networks