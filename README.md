##ZTP Setup on Centos6

###CentOS Setup
* boot image in vcenter
  * skip media test or vDisc will eject
* follow prompts to start install of image
* select "basic server" for install type
* logging with root/"password setup in boot"
* setup network in /etc/sysconfig/network-scripts/ifcfg-eth0
 ``` vi ifcfg-eth0 ```
 ```
 DEVICE="eth0"
 BOOTPROTO="static"
 HWADDR="00:0C:29:5F:44:3A"
 ONBOOT="yes"
 TYPE="Ethernet"
 IPADDR="192.168.5.180"
 NETMASK="255.255.255.0"
 DNS1="8.8.8.8"
 DNS1="4.2.2.2"
 ```
 
#####restart the nic
``` service network restart ```
#####ping the gateway to verify it's online
``` ping 192.168.5.1 ```
 














``` example ```
* example
* "example_01", "example_02"


##example
