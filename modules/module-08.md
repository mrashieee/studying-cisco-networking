# The Internet Protocol

## Purpose of an IPv4 Address

Every device needs an IPv4 address to participate on the internet and
almost all LANs today. It must be properly configured and should be
unique, for communication. This is how a host is able to communicate
with other devices on the network/internet.

The address lives on the network interface, usually the NIC in the
device. Workstations, servers, printers, IP phones all have one. A
server can have more than one NIC and each of them will have their own
IPv4 address. Router interfaces have them too, one per connection.

Every packet crossing the internet has a source address and a
destination address. Network devices read them to deliver the
packet. Replies use the same pair in reverse to find their way back.

### Octets and Dotted-Decimal Notation

IPv4 addresses are 32 bits in length. Here is an IPv4 address in
binary:

11010001101001011100100000000001

Because of the difficulty to read, the 32 bits are grouped into four
8-bit groups called octets:

11010001.10100101.11001000.00000001

It's still difficult to read so we convert it to decimal value:

209.165.200.1

### IPv4 Address Structure

Every address splits into two parts. The front part names the network,
the back part names the host inside it. Your router uses the network
part to get the packet to the right LAN, then the host part to find
the exact device. Where the split falls is decided by the subnet mask:
mask 255.255.255.0 means the first three octets are network and the
last one is host. Same address, different mask, different split.
This network-then-host split is called hierarchical addressing.
Hierarchy exists so routers only learn networks, not every host
on earth. Same idea as phone numbers: country and area codes
find the region, the last digits find the person.

Common masks:

- /8 (255.0.0.0) - first octet is network. Huge networks.
- /16 (255.255.0.0) - first two octets are network. Around 65,000
  hosts.
- /24 (255.255.255.0) - first three octets are network. 254 hosts.
  This is the home LAN shape.

## Assessment Questions

1. What criterion must be followed in the design of an IPv4 addressing
   scheme for end devices?  
   Ans: Each IP address must be unique within the local network.

2. How many octets exist in an IPv4 address?  
   Ans: 4

3. Which two parts are the components of an IPv4 address?  
   Ans: Host portion and network portion.

4. What is the purpose of the subnet mask in conjunction with an IP
   address?  
   Ans: To determine the subnet to which the host belongs.

5. Which statement describes the relationship of a physical network
   and logical IPv4 addressed networks?  
   Ans: A physical network can connect multiple devices of different
   IPv4 logical networks.

6. How large are IPv4 addresses?  
   Ans: 32 bits

7. What is the network number for an IPv4 address 172.16.34.10 with
   the subnet mask of 255.255.255.0?  
   Ans: 172.16.34.0

8. What are two features of IPv4 addresses?  
   Ans: An IPv4 addressing scheme is hierarchical and it is a logical
   addressing scheme.
