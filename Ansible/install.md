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

### Install via Python Pip (cross distribution installation method)

Install pip (available in most package managers as pip or python-pip)

https://pip.pypa.io/en/stable/installing/ 

Install ansible via pip

```
$ pip install --user ansible
```

### Install Documentation 

https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html


## Git install

It is advisable also to install source control. Although this is not required it is beneficial. 

`sudo yum install git` 

## Config file

/etc/ansible/ansible.cfg is the primary Ansible configuration file. 

/etc/ansible/hosts is the default Ansible inventory file.

You can also override these settings by placing ansible.cfg in your home directory, see here for the full list of locations:
https://docs.ansible.com/ansible/latest/reference_appendices/config.html#ansible-configuration-settings-locations

