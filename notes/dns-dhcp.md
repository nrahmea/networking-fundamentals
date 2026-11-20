
# DNS and DHCP

## 1. What is DNS?

DNS (Domain Name System) translates human-readable domain names into IP addresses.

For example, when a user visits `google.com`, DNS helps the device find the IP address associated with that domain.

This allows users to access websites without having to remember their IP addresses.

## 2. Common DNS Records

DNS uses different record types to store information about domains.

| Record | Purpose |
|---|---|
| A | Maps a domain name to an IPv4 address |
| AAAA | Maps a domain name to an IPv6 address |
| CNAME | Creates an alias for another domain name |
| MX | Specifies mail servers for a domain |
| NS | Identifies the authoritative name servers for a domain |
| PTR | Maps an IP address back to a domain name |

## 3. How Does DNS Work?

1. A user enters a domain name into a browser.
2. The device checks whether the DNS result is already cached.
3. If necessary, it sends a query to a DNS resolver.
4. The resolver finds the IP address associated with the domain.
5. The IP address is returned to the device.
6. The device can now connect to the destination server.

DNS commonly uses **UDP port 53**, but it can also use **TCP port 53**.

## 4. What Is DHCP?

DHCP (Dynamic Host Configuration Protocol) automatically provides network configuration to devices.

Instead of manually configuring every device, DHCP can assign:

- IPv4 address
- Subnet mask
- Default gateway
- DNS server

This makes network administration easier and reduces manual configuration errors.

## 5. How Does DHCP Work? (DORA)

DHCP uses a four-step process known as DORA:

1. **Discover:** The client broadcasts a request to find a DHCP server.
2. **Offer:** The DHCP server offers an available IP address and configuration.
3. **Request:** The client requests the offered configuration.
4. **Acknowledgement:** The server confirms the assignment.

DHCP uses UDP ports **67 (server)** and **68 (client)**.

## 6. Key Takeaways

- DNS translates domain names into IP addresses.
- DNS uses different record types, such as A, AAAA, CNAME and MX.
- DNS commonly uses UDP port 53, but can also use TCP port 53.
- DHCP automatically assigns network configuration to devices.
- DHCP provides IP addresses, subnet masks, gateways and DNS server settings.
- DHCP uses the DORA process: Discover, Offer, Request and Acknowledgement.
- DHCP uses UDP ports 67 and 68.
