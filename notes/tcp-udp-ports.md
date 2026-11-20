
# TCP, UDP and Common Network Ports

## 1. What Is the Transport Layer?

The Transport Layer is Layer 4 of the OSI model.

It is responsible for communication between applications running on different devices.

Two important transport layer protocols are TCP and UDP.

## 2. What Is TCP?

TCP (Transmission Control Protocol) is a connection-oriented protocol that provides reliable data transmission.

Its main characteristics include:

- Reliable data delivery
- Packets are delivered in the correct order
- Lost data can be retransmitted
- Flow control helps prevent overwhelming the receiver
- Establishes a connection before transmitting data

TCP is commonly used for web browsing, file transfers and remote administration.

### TCP Three-Way Handshake

TCP establishes a connection using a three-step process:

1. **SYN:** The client requests a connection.
2. **SYN-ACK:** The server acknowledges the request.
3. **ACK:** The client acknowledges the server.

After these steps, the connection is established.

## 3. What Is UDP?

UDP (User Datagram Protocol) is a connectionless protocol that sends data without establishing a connection first.

Its main characteristics include:

- Lower overhead than TCP
- No built-in guarantee of delivery
- No built-in guarantee that packets arrive in order
- No built-in retransmission of lost data
- Suitable for applications that prioritize low latency

UDP is commonly used for voice calls, video streaming, online gaming and DNS queries.

## 4. TCP vs UDP

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Reliable delivery | No delivery guarantee |
| Packet ordering | Maintains order | No ordering guarantee |
| Retransmission | Supported | Not built in |
| Overhead | Higher | Lower |
| Common uses | Web browsing, file transfers | Voice calls, gaming, DNS |

## 5. Common Network Ports

A port identifies a specific application or service running on a device.

Some commonly used network ports include:

| Port | Protocol | Service |
|---|---|---|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 143 | TCP | IMAP |
| 443 | TCP | HTTPS |
| 3389 | TCP/UDP | RDP |

## 6. ICMP and Ping

ICMP (Internet Control Message Protocol) is used for network diagnostics and error reporting.

The `ping` command uses ICMP to test whether another device is reachable over an IP network.

Unlike TCP and UDP, ICMP does not use port numbers.

## 7. Key Takeaways

- TCP and UDP operate at Layer 4 of the OSI model.
- TCP provides reliable and ordered data transmission.
- UDP has lower overhead and does not guarantee delivery or ordering.
- TCP uses a three-way handshake to establish connections.
- Port numbers identify specific services and applications.
- Common ports include 22 (SSH), 53 (DNS), 80 (HTTP) and 443 (HTTPS).
- Ping uses ICMP, not TCP or UDP.
