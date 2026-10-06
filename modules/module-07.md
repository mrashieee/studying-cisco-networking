# The Access Layer

## The Fields of the Ethernet Frame

Ethernet is a technology commonly used in local area networks. Devices
access the Ethernet LAN using an Ethernet Interface Card (NIC). Each
Ethernet NIC has a unique address permanently embedded on the card
known as a Media Access Control (MAC) address. The MAC address for
both the source and destination are fields in an Ethernet frame.

Fields are:

- **Preamble (7 bytes)**: the throat-clear. Repeating 1-0 pattern
  so the receiver locks onto the rhythm before real data starts.

- **Start Frame Delimiter (1 byte)**: the starting gun. Breaks the
  preamble pattern to say data begins with the next bit.

- **Destination MAC Address (6 bytes)**: who the frame is for.
  Switches read this to decide which port it leaves by.

- **Source MAC Address (6 bytes)**: who sent it. Switches learn
  from this which port each device lives on.

- **Length/Type (2 bytes)**: says how long the data is, or which
  upper-layer protocol it carries.

- **Data (46-1500)**: the actual payload - the packet from above,
  padded if too short, capped if too long.

- **Frame Check Sequence (4 bytes)**: checksum of the frame. The
  receiver recomputes it - mismatch means the frame got damaged
  and gets dropped.

## Encapsulation

The process of placing one message format inside another message
format is called encapsulation. De-encapsulation occurs when the
process is reversed by the recipient. Each computer message is
encapsulated in a specific format, called a frame. A frame acts like
an envelope, it provides the address of the destination and address of
the source host. The format and contents of a frame are determined by
the type of message being sent and the channel over which it is
communicated. Messages that are not correctly formatted are not
successfully delivered to or processed by the destination host.

## Assessment Questions

1. What will a layer 2 switch do when the destination MAC address of a
   received frame is not in the MAC table?  
   Ans: It forwards the frame
   out of all ports except for the port at which the frame was
   received.

2. Which network device has the primary function to send data to a
   specific destination based on the information found in the MAC
   address table?  
   Ans: Switch

3. What addressing information is recorded by a switch to build its
   MAC address table?  
   Ans: The source layer 2 address of incoming frames

4. What is the purpose of FCS field in a frame?  
   Ans: To determine if errors occurred in the transmission and
   reception. (this is done with help of Cyclic Redundancy Check
   (CRC))

5. What is one function of a layer 2 switch?  
   Ans: Determines which interface is used to forward a frame based on
   the destination MAC address.

6. Which information does a switch use to keep the MAC address table
   information current?  
   Ans: The source MAC address and the incoming port.

7. What process is used to place one message inside another message
   for transfer from the source to the destination?  
   Ans: Encapsulation

8. Which three fields are found in an 802.3 Ethernet frame?  
   Ans: Destination physical address, source physical address, and
   frame check sequence.  
   (also preamble, length/type, and data)

9. What will a host on an Ethernet network do if it receives a frame
   with a unicast destination MAC address that does not match its own
   MAC address?  
   Ans: Discard the frame

10. Which statement is correct about Ethernet switch frame forwarding
    decisions?  
	Ans: Frame forwarding decisions are based on MAC address and port
    mappings in the MAC Address table.

