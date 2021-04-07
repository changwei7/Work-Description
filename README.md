# Work-Description
This is about the work experience of TenJin Data Center network construction

# Quickly understanding
In this project, we basically worked with the server departments to set up a network of data centers in the Tenjin Data Center
Mainly including the use of routing protocols to make firewalls and Layer 3 and Layer 2 switches, routers and servers communicate with each other。
And through the fortigate combing and testing the policy to control traffic.

# Organization structure
Firstly, design network of data center according to the informations and requirements. Here network topology means it will be analyzed and established according to this form. 

Then, based on confirm the machine after discussion,we prepared those documents to learn and understand the function and port information and the supported protocols

🔸Route

[Cisco 891](https://www.cisco.com/c/ja_jp/support/routers/891-integrated-services-router-isr/model.html)

🔸Switch

[HPE5710 Switch](https://www.hpe.com/jp/ja/product-catalog/networking/networking-switches/pip.hpe-flexfabric-5710-switch-series.1010868971.html)

[HPE5130 Switch](https://www.hpe.com/jp/ja/product-catalog/networking/networking-switches/pip.hpe-flexnetwork-5130-hi-switch-series.1008605458.html)


🔸Firewall

[Fortigate 100E](https://www.fortinet.com/resources-content/fortinet/assets/data-sheets/ja_jp/file/FGT100ESeriesDS)

[Palo alto 850](https://www.paloaltonetworks.jp/apps/pan/public/downloadResource?pagePath=/content/pan/ja_JP/resources/datasheets/pa-800-series-datasheet)

🔸Server load balance

[Big-ip F5 i2600](https://www.networld.co.jp/product/f5/pro_info/bigip/)

Next, we analyzed these documents and to start machine initialization and do the settings with lots of command by using protocols.Makesure the network system can determine the communication path.

Finally,improve the network by combining experiments

![image](https://github.com/changwei7/Work-Description/blob/main/network%20organization%20structure.png)


# Network Topology

In this project，there are 4 networking groups inlude lots of segment.And we use the firewall to control the traffics by the lag port.And all the machine do the stack setting，in the normal times，the primary device will be used.When the port linkdown，the secondary device will be used.So the datacenter network runs all the time.And we used the network protocol such like VLAN,VRRP,BGP,OSPF,PBR IPsec and static routes to make sure the same segment servers as DB and storage will connect between each others.

![image](https://github.com/changwei7/Work-Description/blob/main/Network%20Topology.png)
