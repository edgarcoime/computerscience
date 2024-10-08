# Packet Processing 16
1. Validate packets using mac addresses 
# Packet capturing 17
1. See every single packet coming in through the machine because it is the network stack and it hasn't hit the firewall yet
2. We can troubleshoot network issues through packet capturing which allows us to save packets to analyze at a later time
3. Protocol analysis
4. Raw Sockets
	1. Construct everything in the socket 
# Packet Capturing Process 18
1. Filtering Packets 
# Berkeley packet filter 19
1. 
# Packet capturing with Scapy 20
1. Scapy library in python
```python
from scapy.all import sniff
# Function to handle each captured packet
def packet_callback(packet):
	raw_data = bytes(packet)
	hex_data = raw_data.hex()

	# Process the ethernet header
	print(f"Captured the Packet (Hex): {hex_data}")
	parse_ethernet_header(hex_data)

# Capture packets on a specified interface using a custom filter
filter
def capture_packets(interface, capture_filter, packet_count):
	print(f"Starting packet capture on {interface} with filter: {capture_filter})
	sniff(iface=interface, filter=capture_filter, prn=packet_callback, count=packet_count)

	# Example usage 
	capture_packets('eth0', 'txp and port 80', 5)
```