# Virtual-switches
建立於虛擬平台上，透過軟體模擬出網路交換器的功能，其提供管理員能夠不依賴於實體網路和硬體，動態地重新配置虛擬環境中的網路架構。也由於其變動性較小，因此可減少網路和虛擬平台管理人員的負擔。 

![Virtual-switches](http://www.govmlab.com/wp-content/uploads/2016/02/vNetworking-vSwitch-768x576.jpg)

# TYPE OF COMMUNICATIONS SUPPORTED BY VIRTUAL SWITCH
- Virtual Machine Communications running on same ESXi Host
- Virtual Machine Communications running on different Hosts via Physical Network
- VMkernel Network Traffic
- vMotion Network Traffic across hosts
- IP Storage Traffic ( NFS & iSCSI)
- ESXi Management Traffic
- Fault Tolerance Traffic between Hosts

# KEY FUNCTIONALITIES OF VIRTUAL SWITCH 
It’s a core Layer-2 Forwarding Engine which forwards traffic based on MAC Layer Addresses.
It maintains MAC address and Port Forwarding Table.
It does Forwarding and Filtering of Ethernet Frames like Physical Switch & avoid unnecessary broadcast ( in other words, it is not a hub)
Similar to Physical Switch, when a frame is received on an Interface, the switch looks at the destination hardware address and finds the exit interface in the MAC Table. The Frame is only forwarded to Specified Destination Port. It does Unicast Communication.
It also supports VLAN segmentation at the port level and supports Access and Trunk Mode.
It enables many VMs to share same Physical NIC and Communicate directly with each other.

![Virtual-switches](http://www.govmlab.com/wp-content/uploads/2016/02/Obj2.1_vSwitch01.gif)


