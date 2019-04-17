# Network Intrusion Detection and Prevention 

## IDS
 
 Intrusion detection system detects, logs and alerts to unauthorized host or network use. Alerts based.


## IPS 

Intrusion prevention system. Shares all the characteristics of IPS but adds in functionality that allows the system to respond without the need for operator intervention 

- Passive monitoring has a copy of the traffic sent to the IPS and an alert is sent if "bad" behavior is detected. 
    - The IPS can be set up to send an **out of band** response that *TCP reset* which resents the connections however this does not work with other types of traffic. 

- In line monitoring- the IPS sits between devices and the IPS makes a decision if the communication is allowed. Any suspicious traffic will be dropped. 

**Decisions are made by:** 

- Signature-based is a form of blacklisting and tend to be difficult as constant updates and a longer an longer list. 

- Anomaly based 

- Behavior based rely on established baseline of known "good" behaviors. It generates a high number of false positives because new behaviors can be labled as suspicious. 

- Heuristics - use artificial intelligence to identify potential threats. 
    - Algorithms are used to help it understand if an activity is malicious or not. 
    - These algorithms will have to be updated and tweaked as secuirty professionals define acceptable and malicious conditions. 


### Acronyms 

NIDS or NIPS ---> network based 
HIPS or HIDS ---> host based  


## Components of IDS

Traffic collector - sometimes referred to as a **sensor** it captures activities and events for the IDS. 
   - In the HIDS  the audit logs and the traffic logs for a host
    - In the NIDS it will sensor act as a sniffer and makes copies of the network traffic or the network link. 
    - In off-site storage, the IDS can inspect and monitor the data without causing performance issues across the network.

Signature Database - a collection of known patterns and definitions of malicious activity. An IDS/IPS should receive periodic updates to this data ase as new attack patterns are identified regularly. 

Analysis engine- analysis engine is the component responsible for examining traffic and comparing that against the signature database to find malicious behaviors if presents 