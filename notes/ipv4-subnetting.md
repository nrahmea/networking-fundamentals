# IPv4 Addressing and Subnetting

## 1. What is an IPv4 address?

An IPv4 address is a 32-bit numerical address assigned to a network interface. It is used to identify devices on an IP network and allows them to communicate with each other.

IPv4 addresses are divided into public and private addresses. Public addresses are used for communication across the internet, while private addresses are used within local networks.

## 2. What is a subnet mask?

A subnet mask determines which portion of an IPv4 address identifies the network and which portion identifies the host.

For example:
- 255.255.255.0 (/24) provides 254 usable host addresses.
- 255.255.0.0 (/16) provides 65,534 usable host addresses.

Subnetting allows larger networks to be divided into smaller, more manageable networks.

## 3. What does /24 mean?

/24 is CIDR (Classless Inter-Domain Routing) notation. It indicates that the first 24 bits of an IPv4 address identify the network, leaving 8 bits for host addresses.

The equivalent subnet mask is 255.255.255.0, which provides 256 total addresses, of which 254 are conventionally usable by hosts.

## 4. What is a default gateway?

A default gateway is the IP address of the router interface that a device uses to reach destinations outside its local network.

It forwards traffic towards other networks, including the internet.

## 5. Key takeaways

- IPv4 addresses consist of 32 bits.
- Subnet masks separate network bits from host bits.
- CIDR notation specifies the network prefix length.
- Subnetting divides networks into smaller subnetworks.
- Default gateways allow communication with external networks.
