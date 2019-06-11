# Don't be Famous Study Group

## Part 1: Introduction:
Famous breaches 
Tesla Cloud Resources Are Hacked To Run Cryptocurrency Mining Malware    
https://arstechnica.com/information-technology/2018/02/tesla-cloud-resources-are-hacked-to-run-cryptocurrency-mining-malware/
Shopify     
https://www.eweek.com/security/how-shopify-avoided-a-data-breach-thanks-to-a-bug-bounty
Legacy Security         
Physical Access    
Network Perimeter
Updated Machines         
Workload Isolation             
Could be Dev,     Staging and production. Could also be separating production environments.
         
## Part 2: Security through Architecture
https://kubernetes.io/blog/2018/07/18/11-ways-not-to-get-hacked/#1-tls-everything
Everywhere that can be TLS should be TLS inside the cluster.         
Worker nodes should never have access to etcd for any reason.             
Even Better, Etcd should be completely separate from the controls and         firewall-ed.         
Upgrades
Upgrade in place    
Lower     infrastructure cost            
More “dangerous”                         
Configuration     Drift    
External Access is Easier
Stand up a new cluster
Higher     infrastructure cost                 
Less     “dangerous”                 
Immutable Clusters
External Access is harder.             
Command to know:
https://kubernetes.io/docs/tasks/administer-cluster/safely-drain-node/
kubectl cordon        
kubectl drain         
     
Projects to know:
Velero (arc) –     backups and restores for k8s objects     

## Part 3: RBAC
RBAC relies on a series of well defined and standard concepts that are commonly     found in all implementations.
     
Subjects – A     person, agent or group
Roles- A role     is made of a set of permissions (an approval of a mode of access to a resource)         
Assignments – Role assignment grants a subject right to execute a transaction by         assigning to the subject an active role    
Kubernetes has Role and Cluster Roles
Using RBAC Authorizaiton 
https://kubernetes.io/docs/reference/access-authn-authz/rbac/
Authorization Overview 
https://kubernetes.io/docs/reference/access-authn-authz/authorization/
Roles are defined at the Kubernetes namespace level.         
Batteries Included        
Cluster-Admin             
Admin             
Edit                          
View                      
Role Sprawl Insanity         
Use groups                     
Tools that help :                     
Dex    
https://github.com/dexidp/dex/blob/master/Documentation/kubernetes.md
https://github.com/dexidp/dex        
Gangway 
https://github.com/heptiolabs/gangway

## Part 4: “Policies”
Network Policy     
Default is ALLOW ALL ANYWHERE        
Remember network plugins             
http://github.com/ahmetb/kubernetes-network-policy-recipes     
Pod Security Policy     
Runs on the cluster as an admission controller.                 
Linked to RBAC roles
RBAC defines     what policies users have access to.    
Permissive vs     Restricted    
Default        
Kube-System     
Networking
     

## Part 5: Audit Everything
https://kubernetes.io/docs/tasks/debug-application-cluster/audit/
API Server will log ALL REQUEST for auditing purpose
Audit logs can be VERY NOISY, so you only log what you need.     
Stages of a Request to the API server     
RequestReceived
ResponseStated    
ResponseComplete
Panic         
Audit log levels
None    
Metadata    
Requests
RequestResponse         


## Closing:
Previous Study groups     
[History of Linux](https://youtu.be/qJ1CrzLS7Ak)    
[Ansible](https://youtu.be/0WfYpWl01VQ)
[Command Line Threat Hunting](https://youtu.be/jy9SAUHEWdU)         
[Feedback form](https://forms.gle/oXAa1VYjsJJBsZD78)    
[Free k8s courses](https://linuxacademy.com/blog/linux-academy/freemay2019/)    
[Hearts twitter](@hhover)
