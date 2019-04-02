# Ansible Install 

## Pre Req 
In order to install Ansibe, you must configure the EPEL (Extra Packages for Enterprise Linux) repository on your system. 

The EPEL repository is managed by the EPEL group which is a special intrest group within the Fedora Project. 

* RHEL/CentOS6: 

` yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-6.noarch.rpm`

* RHEL/CentOS 7

yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm



## Install

` sudo yum install ansible` 

## Git install

It is advisable also to install source control. Although this is not required it is beneficial. 

`sudo yum install git` 

## Config file

/etc/ansible/ansible.cfg is the primary Ansible configuration file.

/etc/ansible/hosts is the default Ansible inventory file.

