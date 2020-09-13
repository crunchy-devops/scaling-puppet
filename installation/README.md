# Installation
## Hardware required
For managing 1500 nodes, puppetmaster host should have 16 Gb and 8 cores. 
50 Gb should be allocated to /opt and /var with log retnention should be defined at 25 Gb

## Setup Bolt 
```shell script
sudo rpm -Uvh https://yum.puppet.com/puppet-tools-release-el-7.noarch.rpm
sudo yum install puppet-bolt
```