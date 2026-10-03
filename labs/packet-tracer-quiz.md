# Packet Tracer Quiz ([packet-tracer-quiz.pka](./packet-tracer-quiz.pka))

Final exam for the intro course. Scored 100% on the first try in
about 2 minutes.

## Questions

1. What is the IP address of the Laptop?  
   Ans: 172.16.0.252

2. What is the default gateway for the PC?  
   Ans: 172.16.0.254

3. What is the subnet mask for the PC?  
   Ans: 255.255.255.0

4. From the PC or Laptop, open a web browser, go to cisco.srv, and open the link called A small page. What does it say?  
   Ans: Hello, world!

5. What device connects to the wireless router wirelessly?  
   Ans: Laptop

## Findings

Everything sits on 172.16.0.x with mask 255.255.255.0, so PC,

laptop, and gateway are all on the same subnet. That's why the

answers hang together: .252 and .254 only make sense next to each

other.

## What a default gateway actually is

The gateway is the router's own address on your network - the door

out. When your PC wants an address outside its subnet, it doesn't

try to find it directly. It hands the packet to the gateway and the

router takes it from there.

That's also why no device ever gets the gateway's address. It's

already taken - it belongs to the router's interface on that LAN.

Give it to a PC and you get two machines claiming one IP, which

breaks both (same as any duplicate IP). DHCP knows this too, which

is why the pool it hands out skips the gateway (usually .1 or .254

is reserved for it).
