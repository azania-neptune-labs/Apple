
Active Directory)
AD DS (Active Directory Domain Services)
API (application programming interface)
application layer backbone bus topology
CAN (campus area network) change management client
client-server application client-server network model connectionless protocol connection-oriented protocol data link layer datagram
DBMS (database management system)
decapsulation
DNS (Domain Name System) domain
encapsulation
ESD (electrostatic discharge) fail close fail open
fire suppression system firewall firmware
fragmentation frame
FTP (File Transfer Protocol) grounding header host
HTTP (Hypertext Transfer Protocol) HTTPS (HTTP Secure) hub
review Questions
1. In the client-server model, what is the primary secure protocol used for communication between a browser and web server? a. HTTPS b. TLS c. HTTP d. SSL
2. Which two encryption protocols might be used to provide secure transmissions for email services? a. HTTP and HTTPS b. SSL and TLS c. FTP and SFTP d. SSH and RDP
Copyright 2022 Cengage Learning. All Rights Reserved. May not be copied, scanned, or duplicated, in whole or in part. Due to electronic rights, some third party content may be suppressed from the eBook and/or eChapter(s). Editorial review has deemed that any suppressed content does not materially affect the overall learning experience. Cengage Learning reserves the right to remove additional content at any time if subsequent rights restrictions require it.
hub-and-spoke topology hybrid topology
IMAP4 (Internet Message Access Protocol, version 4) IP (Internet Protocol) IP address
ISP (Internet service provider) knowledge base
LAN (local area network) logical topology
MAC (Media Access Control) address
MAN (metropolitan area network) mesh topology Microsoft SQL Server MySQL network
network layer network service
NIC (network interface card) node
NOS (network operating system) open source Oracle Database
OSHA (Occupational Safety and Health Administration) OSI (Open Systems
Interconnection) reference model P2P (peer-to-peer) network model packet
PAN (personal area network) password manager payload
physical layer physical topology
POP3 (Post Office Protocol, version 3)
port
PPE (personal protective equipment)
presentation layer protocol
RDP (Remote Desktop Protocol) ring topology router
SAN (storage area network) scalable
SDS (safety data sheet) segment server
server operating system session layer
SFTP (Secure File Transfer Protocol) SMTP (Simple Mail Transfer Protocol)
SNMP (Simple Network Management Protocol) SOHO (small office-home office) network
SQL (Structured Query Language)


1)A
2)A
3)c
4)A
5)B
6)A
7)D
8)A
9)B
10)C
11)C
12)B
13)A
14)C
15)B
16)A
17)C
18)A
19)D
20)A


services Description
The Internet can be described as an infrastructure that provides services to applications. These applications (Web, social networks, VoIP...) are said to be distributed since they involve multiple end systems that exchange data with each other. Internet applications run on end systems, not in the packet switches or routers, packet switches facilitate the exchange of data, but they are not concerned with the application that is the source or sink of data.

End systems attached to the Internet provide and Application Programming Interface (API) that specifies how a program running on one end system asks the Internet infrastructure to deliver data to a specific destination program running on another end system.

1.1.3 What Is a Protocol?
All the activity in the Internet that involves two or more communicating remote entities is governed by a protocol.

A protocol defines the format and the order of messages exchanged between two or more communicating entities, as weel as the actions taken on the trasmission and/or receipt of a message or other event

1.2 The Network Edge
Computers and other devices connected to the Internet are often referred to as end systems as they sit at the edge of the Internet. They are also called hosts as they host, run, applications programs such as a Web Browser or an email client.

Hosts are sometimes further divided into two categories: clients and servers. The former being desktop, mobile pcs, smartphones, the latter being powerful machines that store and distribute Web pages, streams... Nowadays most of the servers reside in large data centers

1.2.1 Access Networks
They are the networks that physically connect end systems to the first router on a path from the end system to any other distant end system. Examples: mobile network, national or global ISP, local or regional ISP, home networks enterprise networks.

Home Access: DSL, Cable, FITH, Dial-Up and Satellite
Today, the two most prevalent types of broadband residential access are digital subscriber line (DSL) and cable.

A residence typically obtains DSL access from the telephone company (telco) that provides its wired local phone access. The customer's telco is therefore its ISP. DSL modem use the existing telephone lines to exchange data with DSLAMs (digital subscriber line access multiplexer) located in the telco local central office. The DSL modem takes digital data and translates it to high-frequency tones for transmission over telephone wires, these analog signals from many houses are translated back into digital format at the DSLAM. The use of different frequencies allows the phone line to carry a high-speed downstream channel, a medium-speed upstream channel and an ordinary two-way telephone channel. Hundreds or even thousands of households connect to a single DSLAM.

DSL: 24 Mbps downstream and 2.5 Mbps upstream (MAX VALUES). Because of the difference between these two values, the access is said to be asymmetric.

Cable Internet access makes use of the cable television company's existing cable television infrastructure. Cable modems connect to CMTS (Cablem Modem Termination System) which does the same job the DSLAM does for phone lines. The access is typically asymmetric. CABLE: 42.8 Mbps downstream and 30.7 Mbps upstream (MAX VALUES). Cable Internet access is a shared broadcast medium: each packet travels downstream on every link to every home and viceversa. For this, if several users are simultaneously using the downstream channel, the actual rate will be significantly lower.

Another up-and-coming technology that promises very high speeds is fiber to the home (FTTH). The concept is simple: provide an optical fiber path from the Central Office (CO)

Access in the Enterprise and the Home: Ethernet and WiFi
On corporate and university campuses, and increasingly in home settings, a Local Area Network (LAN) is used to connect an end system to the edge router. Ethernet is by far the most prevalent access technology is corporate, university and home networks. Ethernet uses twisted-pair copper wire to connect to an Ethernet switch which is connected into the larger Internet. The Internet is increasingly accessed wirelessly: wireless users transmit/receive packets to/from an access point connected into the enterprise's network which in turn is connected to the wired Internet.

Wide-Area Wireless Access: 3G and LTE
Smartphones and Tablets employ the same wireless infrastructure used for cellular telephony to send/receive packets through a base station operated by the cellular network provider. Third generation (3G) wireless and fourth generation (4G) of wide-area network are being deployed. LTE ("Long-Term Evolution") has its root in 3G and can potentially achieve rates in excess of 10 Mbps.

1.2.2 Physical Media
The book talks about it in detail but we haven't talked about it in class

A bit, when traveling from source to destination, passes through a series of transmitter-receiver pairs, for each pair, the bit is sent by propagating electromagnetic waves or optical pulses across a physical medium. This can take many shapes and forms and doesn't have to be of the same type for each transmitter-receiver pair along the path. Physical media fall into two categories:

guided media: the waves are guided along a solid medium (fiber-optic cable, twisted-pair copper wire, coaxial cable)
unguided media: the waves propagate in the atmosphere and in outer space (wireless LAN, digital satellite channel)
1.3 The Network Core
1.3.1 Packet Switching
In a network application, end systems exchange messages with each other. To send a message from a source end system to a destination end system, the source breaks long messages into smaller chunks of data known as packets. Between source and destination, each packet travels through communication links and packet switches (for which there are two predominant types, routers and link-layer switches). Packets are transmitted over each communication link at a rate equal to the full transmission rate of the link. So, if a source end system or a packet switch is send a packet of L bits over a link with transmission rate R bits/sec, then the time to transmit the packet is L/R seconds.

Store-and-forward Transmission
Most packet switches use store-and-forward transmission at the inputs to the links. Store-and-forward transmission means that the packet switch must receive the entire packet before it can begin to transmit the first bit of the packet onto the outbound link. The link must buffer ("store") the packet's bits and only after the router has received all of the packet's bits can it begin to transmit ("forward") the packet onto the outbound link.

Queuing Delays and Packet Loss
Each packet switch has multiple links attached to it. For each attached link, the packet switch has an output buffer (or output queue) which stores packets that the router is about to send into that link. If an arriving packet needs to be transmitted onto a link but finds the link busy with the transmission of another packet, the arriving packet must wait in the output buffer. Thus, packets suffer output buffer queuing delays which are variable and depend on the level of congestion in the network. Since the amount of buffer space is finite, an arriving packet may find the buffer completely full. In this case, packet loss will occur, either the arriving packet or one of the already queued packets will be dropped.

Forwarding tables and routing protocols
In the Internet, every end system has an address called an IP address. When a source end system wants to send a packet to a destination end system, the source includes the destination's IP address in the packet's header. Each router has a forwarding table that maps destination addresses (or portions of the destination addresses) to that router's outbound links. When a packet arrives at the router, the router examines the address and searches its forwarding table, using this destination address, to find the appropriate outbound link. A number of special routing protocols are used to automatically set the forwarding tables.

1.3.2 Circuit Switching
In circuit-switched networks, the resources needed along a path(buffers, link transmission rate) to provide for communication between the end systems are reserved for the duration of the communication sessions. When two hosts want to communicate, the network establishes a dedicated end-to-end connection between them.

Multiplexing in Circuit-Switched Networks
A circuit in a link is implemented with either frequency-division multiplexing (FDM) or time-division multiplexing (TDM). With FDM, the frequency spectrum of a link is divided up among the connections established across the link. The width of the band is called the bandwidth. For a TDM link, time is divided into frames of fixed duration, and each frame is divided into a fixed number of time slots.

Packet Switching Versus Circuit Switching
Packet switching is more flexible, uses resources efficiently and is simpler to implement (even if it requires congestion control). Circuit switching offers performance guarantees but uses resources inefficiently

1.3.3 A Network of Networks
To create the Internet, ISPs must be interconnected, thus creating a network of networks. Much of the evolution of the structure of the Internet is driven by economics and national policy, rather than by performance consideration.

Today's Internet is complex, consisting of a dozen or so tier-1 ISPs and hundreds of thousands of lower-tier ISPs. The ISPs are diverse in their coverage, with some spanning multiple continents and oceans, and others limited to narrow geographic regions. The lower-tier ISPs connect to the higher-tier ISPs and the higher-tier ISPs interconnect with one another. Users and content providers are customers of lower-tier ISPs and lower-tier ISPs are customers of higher-tier ISPs. Recently, major content providers (Google) have also created their own networks and connect directly into lower-tier ISPs where possible.

Alt text

1.4 Delay, Loss and Throughput in Packet-Switched Networks
Computer networks necessarily constrain throughput (the amount of data per second that can be transferred) between end system, introduce delays between end systems and can actually lose packets.

1.4.1 Overview of Delay in Packet-Switched networks
As a packet travels from one node (host or router) to the subsequent host along his path, it suffers from several types of delays at each node along the path.

Types of Delay
Alt text

Processing Delay
The processing delay consists of the time required to examine the packet's header and determine where to direct the packet. It may also include other factors, such as the time needed to check for bit-level errors occurred during transmission. They typically are of the order of microseconds or less. After processing the packet is sent to the queue preceding the link to the next router

Queuing Delay
At the queue, the packet experiences a queuing delay as it waits to be transmitted onto the link. It depends on the number of earlier-arriving packets, therefore if the queue is empty, then the packet's queuing delay will be 0. Typically of the order of microseconds or milliseconds.

Transmission delays
If the length of the packet is L bits, and the transmission rate of the link is R bits/sec, then the transmission delay is L/R. This is the amount of time required to push (transmit) all of the packet's bits into the link. Typically on the order of microseconds to milliseconds.

Propagation Delay
The time required to propagate a bit from the beginning of the link to the next router is the propagation delay. The bit propagates at the propagation speed of the link, which depends on the physical medium of the link. The propagation delay is the distance between two routers divided by the propagation speed of the link.

Total nodal delay
it is the summation of the previous delays

1.4.2 Queuing Delay and Packet Loss
The queuing delay depends can vary from packet to packet, therefore when characterizing queuing delay, one typically uses statistical measures, such as average queuing delay, variance of queuing delay, and the probability that the queuing delay exceeds some specified value