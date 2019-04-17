# Technologies and Tools 

## FireWalls

 Application-aware securitgy devices require that every packet be analyzed and categorized
 
 Can also be called
 - Application layer gateway
 - Stateful multilayer inspection
 - Deep Packet inspection 


## VPN 

- Full tunnel - all traffic will go through the tunnel 

- Split tunnel- all traffic to X goes through the tunnel, traffic to Y does not 

- Site to Site VPN

 Often firewalls will act as vpns concentrators. Often IPsec (Internet Protocol Security) is used offering OSI layer three security. IPSec is a standardized protocol that provides integrity checks. 
    - IPSec has two core protocols Authentication Header (AH) and Encapsulation Security Payload (ESP)
    -IPSec has two different modes for communication. 
 Transport mode which places an IPsec header and a IPsec trailer around the data to encrypt but the original ipheader is left.
Tunnel mode the Ip header and data are encrypted and a whole new IP header is added

## High-end cryptographic hardware (HSM)  

allows back up key secure storage or allow for an SSL endpoint to offload that CPU overhead from other devices. 

##  Media gateways 

 converts between Public Switched Telephone Network (PSTN) and VoIP by allowing ISDN trunk on one side and Ethernet with VoIP on the other. 

## Security Tools: 

###  Passive tools- listen to gain info

* *Protocol analyzer* - capturing network traffic to be able to view traffic patterns and have them displayed in plain text. (ie wire shark)
    - Can be used on wired or wireless to view traffic patterns and identify unknown or unverified traffic and verify network tools. 

### Active tools - send traffic to the target to gain information 

 - Can be used on wired or wireless to view traffic patterns and identify unknown or unverified traffic and verify network tools. 

* *Network Scanner*- a tool designed to probe a network or system for open ports. You can have it scan a specific IP or a range of IP addresses. (Nmap and Zenmap, Angry IP Scanner)

* *Wireless scanners* - there are specially crafted tools to perform wireless scanning because of these differences many organizations often neglect to ensure compliance of their wireless network.
  - Cracking find a wirless network key - Aircrack-ng, FERN
  - password cracking - john the ripper

### Data Sanitization 

- Overwrite the data once and its gone
    - one and done 
    - multiple for piece of mind
-Whole drive - Darik's Boot and Nuke (DBAN)

### Explotation frame works 
- BeFF - The Browser Exploitation Framework Project
- Metasploit