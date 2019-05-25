# Networking 

## Switch

The backbone of a LAN as it connects devices together on a single network by using packet switching to forward data to the destination device. The difference between a router and a switch is that a router can forward communication from one network to another while a switch is limited to node-to-node communication on the same network.

### Port security
 the capability provided by a switch that controls what devices are allowed to connect to each port on that switch. This is accomplished through the use of the end devices MAC address. 

- Static Learning: Specific Mac addresses are assigned to specific ports

- Dynamic Learning- the switch learns which mac addresses should be used as they connect. 

- Sticky learning - allows multiple devices to particular port mainting those setting in memory even through reboots. This helps prevent in attacks that force the switch to reboot 

- Loop prevention- One of the problems with layer 2 switches is that there is no inherited mechanism in place to kill or drop packets that get caught in loops or otherwise paths cannot be resolved. To counter this a few mechanisms have been put in place to provide loop protection.

- OSPF - open shortage path first which is a robust link-state interior gateway which creates a logical point to point topology that prevents looping

- STP - spanning tree protocol it acts by trimming connections that are not part of the spanning tree connecting all nodes  

- IEEE 802.1X Port-Based (Network Access Control NAC) 
You don't get access unless you authenticate to a physical interface. 

## Load Balancer 

- Round Robin 
	- Weighted round robin prioritize the server using
	- dynamic round robin monitors the server load and distributes to the server with the lowest use (Active/active load balancing) 

- Affinity a kindship or likeness meaning the application requires communication to the same instance. Each user uses the same server based on IP address or session IDS (Source affinity& Active/active  )

- Active/ passive load balancing means some servers are active while others are on standby working as fault tolerance 


## Demilitarized Zone (DMZ) 

Exist between the internet and trusted internal network. Has firewalls on both sides, from both the external and internal zone. The idea is to force outsiders to make at least one hop into the DMZ before they can access the internal network. 
	- Servers that should be in the DMZ are any servers that external entities can supply information to and retrieve information from (web servers, ftp servers) Rat servers that can force authentication into the trusted internal network, 

- Network Segregation is used to control access to resources. 
	- physical segregation refers to separate hardware and cabling.

- Logical segregation refers to dividing a network into subnets based on functionality, using firewalls or routers to separate and facilitate communication between the logical networks.

- Virtualization provides logical server isolation while still allowing physical hosting. 