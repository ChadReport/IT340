

Stateful FIrewall:
Tracks network connections based on the connection state using active sessions base off of state tables.

Stateless [[Firewall]]:
Filtering packets without tracking connection state, purely by pre-defined basic rulesets. IP addresses, ports, and protocols.

Packet inspection:

Examining of network packet headers as well as their payloads for enhanced security rules
additional security layer.



[[DMZ]]"Screened Subnet" (Firewall):`

A network segment that separates publicly accessible servers from internal networks, providing a barrier and 



Internet:


[[Netflow]]: 

Network Protocol developed by cisco for monitoring and collecting network performance 

standard [[ACL]]:

Access control lists that filter traffic based solely on the ip address

Extended [[ACL]]:

More advanced access control list that allows filtering based on packet information such as IP address, protocols, and ports.

5 tuples:

Source and Destnation IP, source and dest port, and protocol

Example of ^

Source IP address: 192.168.1.11 -> Dest IP Address: 10.0.1.11, SRC port: 53,371, Dest port: 53, procol DNS


Intranet:

A private network. Only accessible to an organisation's internal users, typically designed for secure internal connectivity and resource sharing

Extranet:

An extension of a private network allowing controlled access to external parties, such as contractors or customers.

Internet:


Explain how to trouble shoot routing issues:

Turning it on & off again. Firing the product owner of Packet Tracer.

Double check your routing tables.

Double check your network settings.

Explain end to end connectivity tests:

Use [[ICMP]]

Ping it!

How to examine [[Netflow]]:

We can use a protocol analyzer Like Wireshark to help us analyze [[Netflow]].

Define IN Bound rule Placement:
A ruleset that applies to packets recieved by an interface


Define out bound rule placment:

A ruleset that applies to going outside of a network


how do you determine which way to place an [[ACL]]:

Determine whether it'll be a standard [[ACL]] or extended [[ACL]]. Identify the information source or destination bound traffic. if it is closer to it's original source or further away.


Where to place a Standard [[ACL]]:
Closest to the destination. It's less defined, broader scope. Limiting web surfing. Top Down Policy enforcement. Breaking up the network. Major traffic shaping.

Where to place an Extended [[ACL]]:
Closest to the source. Complex rulesets. To prevent overloading of an internal network. Denying access to a specific application or service. 

Traffic shaping:
Traditionally it is defined as bandwidth management and Quality of service, allowing some applications or traffic types priority over others. in network security traffic shaping is the control and flow of a network communication over a network as a whole