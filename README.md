##ZTP Setup on Centos6

###CentOS Setup
1. boot image in vcenter
  * skip media test or vDisc will eject
* follow prompts to start install of image
* select "basic server" for install type
* logging with root/"password setup in boot"
2. setup network in /etc/sysconfig/network-scripts/ifcfg-eth0
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
 
3. restart the nic
``` service network restart ```
4. ping the gateway to verify it's online
``` ping 192.168.5.1 ```
5. you should now be able to ssh to the vm
6. ```
   ssh root@192.168.5.180
   password: 
   ``````
 
7. The rest of your work can now be done while sshd into your vm rather than from the console window in vmware


 














``` example ```
* example
* "example_01", "example_02"


##example
