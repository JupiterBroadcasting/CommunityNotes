# Ansible Install 

## Pre Req 
In order to install Ansibe, you must configure the EPEL (Extra Packages for Enterprise Linux) repository on your system. 

The EPEL repository is managed by the EPEL group which is a special intrest group within the Fedora Project. 

* RHEL/CentOS6: 

` yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-6.noarch.rpm`

* RHEL/CentOS 7

yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm



## Install

### Via DNF or YUM

` sudo yum install ansible` 

or 

` sudo dnf install ansible`

### Latest via Apt 

```
$ sudo apt-get update
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository --yes --update ppa:ansible/ansible
$ sudo apt-get install ansible
```

Note: On older Ubuntu distributions, “software-properties-common” is called “python-software-properties”.

### Install Documentation 

https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html


## Git install

It is advisable also to install source control. Although this is not required it is beneficial. 

`sudo yum install git` 

## Config file

/etc/ansible/ansible.cfg is the primary Ansible configuration file.

/etc/ansible/hosts is the default Ansible inventory file.

Ansible also looks `ansible.cfg` from current directory before failing back to the default one. Inventory file, as well as many other settings, can be defined inside the config file and kept easily in git repo so that any changes are easily tracked.

Documentation of all the configuration file settins can be found from:

https://ansible-manual.readthedocs.io/en/latest/intro_configuration.html
