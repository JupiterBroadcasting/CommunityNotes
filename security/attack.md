# Attacks

`Etter cap is a free and open source network security tool for man in the middle attacks on LAN. It works by putting the network interface into promiscuous mode and by Arp poisoning the target machine. This allows it to act as a man in the middle. `
 
## Arp Poison (Spoofing type)

ARP spoofing is a type of attack that is meant to falsify the address resolution protocol message over a local area network. This results in the linking of an attackers MAC address with the IP address of a legitimate computer or server on the network. A victim would send traffic to the attacker (man in the middle) thinking that the attacker was the real endpoint. 

- One way to prevent this is to use the arp command to put a static entry into your ARP table. 

## Man in the browser 

MIB attacks use a proxy on your local machine that allows capture of encrypted traffic before its encrypted. MIB installs malware on a computer system to watch activity when you visit a certain site. It will issue instructions such as when X bill is paid transfer funds to the attacker. 

## Replay Attack: 

Captures communication and replays it at a later time. Usually attempting to circumvent authentication. Usually capturing and reusing certificates or tokens. 

* Easier to carry out on a wireless system because traffic is easier to capture.

### Pass the hash (Variant of replay attack) 

attackers capture a password hash and reinsert it into the system as authentication 

## Initialization Vector (IV):

used in wireless as the randomization element at the beginning of a connection. Attackers aim to determine the iv so that they will be able to repeat it (much like a replay attack) and make the connection as well. 

## Buffer overflow 

memory spills over beyond the expected/allocated area. If they can exploit it and replicate it they will own it. 

 - Code injection is enabled by bad coding that will allow for things like SQL injections. 

- SQL injections use database calls to look for your own request instead of those intended.

- XML extensible markup language set of rules for data transfer and storage

## DOS -  denial of service attack makes use of a known vulnerability target 
   - DDOS -  distributed denial of service attack. carries out multiple attacks on a system often makes use of a botnet.

## Driver manipulation

Changes the drives thus changing the behaviors of a system. drivers are generally less secure than the OS that they are connected to leaving a security gap that can be attacked. Shimming- putting code between the OS and drivers. (This can have legitimate uses) 


## Cross-site scripting (XSS) 
 Originally named as it allowed info to be sent between sites when more than one tab was open. It takes advantage of inherent trust an application has. 

1) Theft of authentication from a web app
2) session hijacking
3) Deploying hostile content
4) Impersonation of user

- Non-persistent (Reflect) XSS attack a website by allowing scripts to run in through user input. For example inside of a search box.

- Persistent (Stored) XSS attacks will include a malicious payload with no specific target these are popular on social media.

- DOM-based XSS attacks are executed in the browser via the Document object model (DOM) process as opposed to the web server. 

** To protect do not click on links, some say to disable javascript but this could cause issues inv isiting may websites. In the end, keep your apps updated.


## Cross-Site request forgery

  ``` an example of this attack is you are checking your bank balance when you receive an email with hotlink in an email about "X" you click on the link and a request is sent to your bank session for transfers to be sent to the attacker. ``` 

One click attack, session riding XSRF, CSRF (sea surfing) 

Takes advantage of the trust that a web application has for the user. Encryption can usually be used as prevention. 

## DNS Poisoning 

 modifys the client host file and send a fake response to a valid DNS request

## Domain highjacking 

allows access to be gained to the domain registration and this will enable you to control where traffic is sent. 

## Other

- Clickjacking- overlay trick that has user click on a malicious link 

- Session Jacking allows attackers to circumvent authentication as they take over an active connection (Stealing session ID) 

    - Cookie high jacking can be used to steal info needed. 

- Refactoring the process of restructuring code without changing the external behavior. 

-  Spoofing making data look like it's coming for somewhere else. 
    - Such as mac or IP spoofing. 

    - Smurf attack - attacker spoofs a packer to all systems on a  particular network and forges the from address so that target host gets all the replies


- Evil Twin and Rouge - Attackers set up their own access point and users will connect allowing the attacker to become a MIM 

- Wireless jamming - term to remember here is fox hunting and this is when you are hunting to find out what is causing the issue at a minimum you will need the use of a directional antenna. 

- BlueJacking- sending of unsolicited messages to another device via blue tooth. This should even request to add data to your device. (Generally a deprecated attack) 

- Bluesnarfing is the theft of information from a wireless device through a Bluetooth connection. 