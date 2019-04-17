## Terms:

* **Black box testing**- Pentester has little to no knowledge of the system it's self. 

* **White box testing**- all the functionalities of the system are known to the pen tester. 

* **Steganography** 
    - Steganos: "covered, concealed or protected."
    - Graphein: " Writing." 

- **Honeypot** is a server designed to look and act like a real server but rather than having real data the data within it is fake.
	- legal concerns of the use of a honeypot is entratment.
    
- **System sprawl**- is what happens when the systems expand over time and exceed documentation and knowledge of your security professional leading to *undocumented assets.*

- Mac - Media Access Control 

- **Segmentation fault** - Prevents access to a restricted area of memory

- **High-end cryptographic hardware** (HSM)  allows back up key secure storage or allow for an SSL endpoint to offload that CPU overhead from other devices. 
- Media gateways - converts between Public Switched Telephone Network (PSTN) and VoIP by allowing ISDN trunk on one side and Ethernet with VoIP on the other. 

- **Exploitation Frameworks** are tools that attackers use to find vulnerabilities in a system (Metasploit)

- **BlueJacking** - sending of unsolicited messages to another device via blue tooth. This should even request to add data to your device. (Generally a deprecated attack) 

- **Bluesnarfing** - is the theft of information from a wireless device through a Bluetooth connection. 

- **Basic Packet Filtering** - firewall will only use packet headers to make the decision on to allow or block.

- **Implicit deny**  - blocks anything not implicitly allowe
## Command Line Security Tools 

- Ping test reachability 
- NetStat (Networtk statistics) 
    - netstat - a shows all active connections (Linux) 
- Traceroute - Determine the route a packet takes to a destination 
    - Windows (tracert)
- nslookup and dig look up infomration from DNS servers 
- tcpdump - capture packets from the command line. 



## Security protocols  

- Secure real time transport protocol (SRTP) Adds security features to RTP to keep conversation private and uses AES to encrypt the voice and video flow. 
  - Encryption, message authentication, and replay protection. 

- NTP Sec - secure network time protocol began development in June 2015. 

- S/MIME Secure multipurpose Internet mail extensions, public key encryption and digital signing of mail content. It requires a PKI or similar organization of keys.

- Secure POP and Secure IMAP Use STARTTLS extension to encrypt 

- FTPS- File Transfer Protocol over SSL. Remember this differs from *SFTP* which is ssh file transfer protocol 

- DNSSec - Domain Name System Security Extension, uses public key cryptography. 
   - DNS records are signed so that DNSSEC responses are authenticated. 
   - Althought they are signed they are not encrypted alloweing for network security devices to inerpret the data contained inside the packets.
   - DNS traffic usually over **UDP** port 53 but this limited in size to 512 bytes. Since DNSSEC packets can be larger it uses **TCP** port 53.

- SNMPv3 - Simple Network Management Protocol version 3 
Encrypted communication and authenticates the source the information is coming from.
is the standard developed for management of devices on IP-based networks. Uses port 161 and TRAPS which are the alerts sent to central SNMP manager are sent via 162. 

- DHCP does not offer a secure version thus we face the issue of Rogue DHCP servers. Microsoft addresses this by having DHCP to authorize with AD. 
    
- DHCP client DoS - starvation attack. spoofs MAC address to exhaust the DHCP pool. Switches can be configured to limit the number of MAC addresses per interface. 

- LDAPS uses port 636 . LDAPS has now been replaced with SASL. 