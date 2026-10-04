# Build a Home Network

## Home Network Basics

Home network routers typically come with:
- **Ethernet Port**: routers have an internal switch portion with
  ports to connect devices over wires. This port is used for
  connecting the router to the local network.

- **Internet Port**: this port connects the router to another
  network. It plugs into the modem's Ethernet port, and through
  the modem reaches the internet.

- **Radio antenna** and **wireless access point** are built in routers
  for devices that cannot be physically plugged into the router, they
  connect over Wi-Fi instead. The devices on the wireless network will
  also be in the same local network as the devices that are physically
  plugged into the Ethernet ports. Internet port is the only port that
  connects router to a different network.

## Network Technologies in the Home

### Wireless Frequencies

The technologies used in home networks are in the unlicensed 2.4 GHz
and 5 GHz frequency ranges. Bluetooth uses the 2.4 GHz band. It is
limited to low-speed and short-range communication, but it can talk
to many devices at the same time. This is why Bluetooth is used for
connecting peripherals and accessories.

Modern Wi-Fi follows the IEEE 802.11 standards, which also use the
2.4 GHz and 5 GHz bands. Unlike Bluetooth, 802.11 devices transmit
at much higher power, so they reach farther and move data faster.
Both bands are unlicensed, meaning anyone can use them without a
permit.

### Wired Network Technologies

Even with Wi-Fi everywhere, some devices do better on a wired
connection that nobody shares with them.

- **Ethernet**: the most common wired protocol. A set of rules that
  lets devices talk over a wired LAN, using many kinds of wiring.

- **Unshielded twisted pair and RJ-45**: home Ethernet runs on
  unshielded twisted pair (UTP) cable, usually Cat5e or better. RJ-45
  is the clear plastic plug on the end. Patch cables come ready-made
  in many lengths. Newer homes have Ethernet wall jacks wired in
  already.

- **Powerline**: for homes with no network wiring. Adapters send
  the signal through the electrical outlets instead.

- **Coaxial**: the thick cable-TV wire. Carries TV plus internet to
  the modem on the same line.

- **Fiber optic**: thin glass strands carrying light instead of
  electricity. Fastest option, used for the backbone and in some
  homes (fiber to the home).

### Wireless Standards

Standards for wireless devices are made by many organizations, main
organization is IEEE (Institute of Electrical and Electronics
Engineers). IEEE handles the 802.11 standards and rules. The Wi-Fi
Alliance tests wireless LAN devices from different manufacturers.
Devices that pass get the Wi-Fi logo, which is given by the Wi-Fi
Alliance and means the device should work with other Wi-Fi gear.
Standards keep improving, so stay aware of new ones since makers put
them in new devices fast.

### Wireless Settings

Wireless routers using the 802.11 standards have multiple settings to
configure:

- **Network mode**: determines the generation of technology that must
  be supported.
  - **802.11b**: 2.4 GHz, up to 11 Mbps. Oldest generation, only
    keeps ancient devices online.
  - **802.11g**: 2.4 GHz, up to 54 Mbps. Old systems (~15 years),
    faster than b but still slow.
  - **802.11n**: 2.4 + 5 GHz, up to ~600 Mbps. First fast one,
    what most devices use.
  - **Mixed mode**: speed will depend on the oldest system on the
    network.

(Side note by rashieee: b/g/n are Wi-Fi 4 and older. Modern routers
use ac (Wi-Fi 5), ax (Wi-Fi 6), be (Wi-Fi 7) instead.)

- **Network Name (Service Set Identifier)**: the name of the wireless
  network (WLAN). Case-sensitive, up to 32 characters, sent in every
  frame header. Devices must know it to join.

- **SSID Broadcast**: the router sends its name out so it shows in
  scans. Turning it off hides the network, but you can still join by
  typing the SSID and password. Hiding is not security, always use the
  strongest encryption available.

## Assessment Questions

1. Which type of wireless communication is based on 802.11 standards?  
   Ans: Wi-Fi

2. What wireless router configuration would stop outsiders from using
   your home network?  
   Ans: Encryption

3. What type of device is commonly connected to the Ethernet switch
   ports on a home wireless router?  
   Ans: LAN device

4. Which type of network technology is used for low-speed
   communication between peripheral devices?  
   Ans: Bluetooth

5. What can be used to allow visitor mobile devices to connect to a
   wireless network and restrict access of those devices to only the
   internet?  
   Ans: Guest SSID

6. What purpose would a home user have for implementing Wi-Fi?  
   Ans: To create a wireless network usable by other devices.

7. What is another term for the internet port of a wireless router?  
   Ans: WAN port

8. Which type of network cable consists of 4 pairs of twisted wire?  
   Ans: Cat 5e

9. What is the default SSID Broadcast setting on a wireless router?  
   Ans: Enabled

10. What is a characteristic of network SSID?  
    Ans: It is case sensitive.
