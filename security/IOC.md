## IOCs

Indicators of Compromise are indicators or signs that unauthorized activity has compromised information system. IOCs act as breadcrumbs for incident response investigators allowing them to put together the clues to what has occurred.

### Commonly observed IOCs

Before understanding IOCs you will need to understand the baseline of your system.

* Unusual outbound network traffic - this would be centered around stealing data
* Anomalies in privileged user account activity
*Account login red flags 
* Geographical irregularities in network traffic - if your account admin lives in Keller why are they logging in from China? 
* Increase in database read volumes
* HTML response size increase
* Large numbers of Requests for the same files
* Mismatched port application traffic, including encrypted over plain ports.
* Suspicious registry or system file changes. 
* Unusual DNS requests most command and control malware masks its self as DNS request, so if you see large numbers of these request this might warrant more investigation.
* Unexpectedly patched - some attackers will patch a system to ensure they are the only one who has access to this system. If other attackers are able to access it this lowers the profit they can make on your information.
* Bybdkes if data in the wrong place(s) - if you start seeing data from an isolated server on one with outbound access.
* Web traffic with non-human behavior, for example, large calls to one or more multiple IPs in nanoseconds.
* Signs of DDos Attempts, even if it's temporary.

## Frameworks for sharing IOCs

* OpenIoc
  * Created by mandiant to facilitate sharing IOC data.
  * Open Source

* STIX/TAXII/CybOx
  - Structured Threat Information Expression (STIX) 
  - Trusted Automated Exchange of Indicator Information (TAXII)
  - Cyber Observable Expression (CybOX) 



