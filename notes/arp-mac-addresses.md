
# ARP and MAC Addresses

## 1. What is a MAC address?

A MAC (Media Access Control) address is a hardware address assigned to a network interface controller (NIC). It is 48 bits long and is usually represented using hexadecimal notation.

It identifies a network interface for communication on a local network.

For example, a laptop can have an Ethernet port and a Wi-Fi adapter. Since both are separate network interfaces, they normally have different MAC addresses.

## 2. What is ARP?

ARP (Address Resolution Protocol) is a communication protocol used to discover the MAC address associated with a particular IPv4 address on a local network.

It resolves 32-bit IPv4 addresses into their corresponding 48-bit MAC addresses.

## 3. How does ARP work?

When Host A wants to communicate with Host B on the same local network, but doesn't know Host B's MAC address, it sends an ARP Request.

The ARP Request is sent as a broadcast using the destination MAC address:

FF:FF:FF:FF:FF:FF

This broadcast reaches all devices on the local network.

Each device checks whether the requested IPv4 address belongs to it. If Host B recognises its own IPv4 address in the request, it responds with an ARP Reply containing its MAC address.

Host A receives the reply and can now communicate with Host B using its MAC address.

## 4. What is an ARP cache?

An ARP cache is a table stored by a device that contains previously learned mappings between IPv4 addresses and their corresponding MAC addresses.

It reduces unnecessary ARP requests because devices can reuse previously learned mappings.

## 5. Key takeaways

- MAC addresses are 48-bit hardware addresses.
- Network interfaces normally have their own MAC addresses.
- ARP resolves IPv4 addresses into MAC addresses.
- ARP Requests are broadcast across the local network.
- ARP Replies provide the requested MAC address.
- ARP caches store previously learned IP-to-MAC mappings.
