## Types of Threat Actors

1) Script kiddies
2) Hactivist
3) Organized crime
4) Nation States 

## Vulnerabilties 

are the source of almost all security concerns 

* Improper input handling or input validation are the number one cause of software vulnerabilities. 
    - The following attacks take advbantage of missing input validation checks:
        - Buffer overflow
        - Cross site scripting (XSS)
        - Cross site request forgery (XSRF)
        - Injection attacks ( such as SQL Injection )

* **Race conditions** – the order of the input does not occur in the way that it was intended or expected creating a race condition. The idea is that multiple inputs are racing each other in an attempt to influence the output. The most commin impact of a race condition is system failure in the form of a crash. This can also cause unexpected output, perhaps output not given in the format we were expecting.
    - **Counter measure and prevention.**  
        - *Reference counters* - Structures in the kernel that detail whether a particular resource is in use.
        - *Locking the kernal* - if two programs grab the same portion of the kernel, modify it and then write back to memory the expected output should be four new outputs, however since they over write we are left with three. We combat this by enabling kernel locking however this can lead to performance degradation.
        - *Thread synchronization*  – save on performance issues and prevents threads from accessing the shared data at the same time.  


### Vulnerability Scanners

* Network vulnerability scanner
* Host vulnerability scanner
* Application vulnerability scanners 
* Configuration compliance scanner- security content automation protocol (SCAP) was developed for automating config checks. These scanners are used to inform admins when their configuration does not meet their defined requirements. They check for
    - os versions
    - installed programs and apps
    - settings  of the network
    - presence and settings of anti-virus

### Vulnerability scanning results
* Plan of Action
    - what measures are taken when the results are found and how do we shore up and put controls in place to address vulnerabilities found. 


## Tech types

### RFID 
Data capture with MIM type. Jam signal or spoof your own reader. There are many decryption keys for sale online.

### NFC 

possible issues: Relay and Reply, Man In the Middle, jamming and lost devices. 

### 802.11 wirless 

no authentication, encryption by default but even with encryption sone of the info can be in the clear. 