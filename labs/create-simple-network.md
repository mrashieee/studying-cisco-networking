# Create a Simple Network ([create-simple-network.pka](./create-simple-network.pka))

First lab: one PC, one laptop, wired up and interacting.

| Device | IPv4 Address       | Subnet Mask   | Default Gateway |
|--------|--------------------|---------------|-----------------|
| PC     | 192.168.0.2 (DHCP) | 255.255.255.0 | 192.168.0.1     |
| Laptop | 192.168.0.3        | 255.255.255.0 | 192.168.0.1     |

Who gets .2 and who gets .3 depends on which device connects first -
DHCP hands them out in order, so they are not fixed numbers. Same network,
same mask, same gateway, that's what makes them able to reach each
other.
