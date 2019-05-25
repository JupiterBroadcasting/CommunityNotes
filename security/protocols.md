
## Security protocols  

- **Secure real time transport protocol** (SRTP) Adds security features to RTP to keep conversation private and uses AES to encrypt the voice and video flow. 
  - Encryption, message authentication, and replay protection. 

- **NTP Sec** - secure network time protocol began development in June 2015. 

- **S/MIME** Secure multipurpose Internet mail extensions, public key encryption and digital signing of mail content. It requires a PKI or similar organization of keys.

- Secure POP and Secure IMAP Use STARTTLS extension to encrypt 

- **FTPS**- File Transfer Protocol over SSL. Remember this differs from *SFTP* which is ssh file transfer protocol 

- **DNSSec** - Domain Name System Security Extension, uses public key cryptography. 
   - DNS records are signed so that DNSSEC responses are authenticated. 
   - Althought they are signed they are not encrypted alloweing for network security devices to inerpret the data contained inside the packets.
   - DNS traffic usually over **UDP** port 53 but this limited in size to 512 bytes. Since DNSSEC packets can be larger it uses **TCP** port 53.

- **SNMPv3** - Simple Network Management Protocol version 3 
Encrypted communication and authenticates the source the information is coming from and is the standard developed for management of devices on IP-based networks. Uses port 161 and TRAPS which are the alerts sent to central SNMP manager are sent via 162. 

- **DHCP** does not offer a secure version thus we face the issue of Rogue DHCP servers. Microsoft addresses this by having DHCP to authorize with AD. 
    
    -  DHCP client DoS - starvation attack. spoofs MAC address to exhaust the DHCP pool. Switches can be configured to limit the number of MAC addresses per interface. 

- **LDAPS** uses port 636 . LDAPS has now been replaced with SASL. 