# TCP Servers

## Event Queues

Much of the NodeJS architecture is built around the use of events. All objects that emit events in NodeJS are instances of the EventEmitter constructor

## OSI Model (Open Systems Interconnection)

 (OSI model) was developed as a seven layer model. This seven layer OSI model has continued to accurately describe the different processes in computer networking, and is still widely used as a point of reference while working in networked systems today.
 
 > Not every computer network solution uses all seven layers , for example HTTP skips the Presentation and Session layers and lives directly on top of the Transport layer.

## OSI Layers

 1. Physical >> bit, transmission and reception of raw data streams over a physical medium , USB, Bluetooth, Ethernet physical layer, SMB, Telephone network modem
 2. Data Link >> Frame , Reliable transmission of frames between to physical layer nodes, Ethernet and IEEE 802.11 wireless LAN
 3. Network >> Packet, Managing the network through addressing, routing, and traffic control, IP and ICMP
 4. Transport >> Segment/Datagram, Reliable transmission of data between points on a network, TCP and UDP
 5. Session >> Data, Manages a session though passing data back and fourth, NetBios and Remote Procedure Protocol (RPC)
 6. Presentation >> Data, 	Data translating, including encryption, character encoding, and compression , Strings encoded with null terminated strings vs Strings defined by an Integer Length
 7. Application >> Data, Height Level APIs, HTTP, IMAP, POP, SSH

## Internet Protocol Suite

The Internet Protocol Suite is the conceptual model for the protocols used by the internet. It is often referred to as TCP/IP because the IP and TCP were the original protocols in the suite.

> The Internet Protocol Suite is described using four layers - Link(Used to move packets between two different hosts), Internet(Maintains computer addressing and identification and manages packet routing), Transport(Provides process to process data exchange), and Application(Provides high level data exchange for use in user application development). 

## TCP (Transmission Control Protocol )
used by application layer protocols in the Internet Protocol Suite. 