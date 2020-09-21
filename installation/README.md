# Installation
## Hardware required
For managing 1500 nodes, puppetmaster host should have 16 Gb and 8 cores.   
50 Gb should be allocated to /opt and /var with log retention should be defined at 25 Gb

## Setup Bolt 
```shell script
sudo rpm -Uvh https://yum.puppet.com/puppet-tools-release-el-7.noarch.rpm
sudo yum install puppet-bolt
```

## Setup Puppetserver
For CentOS go to ```https://yum.puppetlabs.com/```  
Select ```https://yum.puppetlabs.com/puppet5/puppet5-release-el-7.noarch.rpm``` for CentOS 7
Hit
```shell script
yum install -y https://yum.puppetlabs.com/puppet5/puppet5-release-el-7.noarch.rpm
yum install -y puppetserver
``` 
Log out , log in again for the change takes effect

Change memory settings for puppetserver JVM 
```shell script
vi /etc/sysconfig/puppetserver
Modifier the memory footprint for the puppetserver
```
Modify the hosts def to reflect your DNS name as Fully Qualified Domain Name

### Install the CA
```shell script
puppet cert list -a 
```  


