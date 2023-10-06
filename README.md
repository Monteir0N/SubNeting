# SubNeting
Easy SubNeting using Html/Js

This Page will alow you to insert a network ipv4 address and a subnetmask either 
in dotted decimal or the corresponding CIDR and calculate the subnet details.

For those newer to this subject, also alows to input the number of hosts that you 
need on that subnet and automatically determine the smallest subnet mask that will 
meet your requirements.

if you're trying to create several subnets, you can start by inputing in the 
Ip Address field the ip to your network and the submask (or number of hosts
needed) for your first subnet, press calculate. After in the Ip Address Field
input the next free ip available (the one after the "Network Broadcast IP in 
Decimal") of the previous calculated subnet.

ex: starting with the network 192.168.1.0
    needing 40 hosts

    press calculate.
    You'll get the following output

IP Address in Binary:	11000110.10101000.00000001.00000000
Subnet Mask in Binary:	11111111.11111111.11111111.11000000
Network IP in Binary:	11000110.10101000.00000001.00000000
====================================	=================================
Network IP in Decimal:	198.168.1.0
Subnet Mask :	255.255.255.192
First Available Host IP in Decimal:	198.168.1.1
Last Available Host IP in Decimal:	198.168.1.62
Network Broadcast IP in Decimal:	198.168.1.63
Total Number of hosts bits:	6
Total Number of IPs Available for Assignment:	62

    then input on the ip address field 192.168.1.64 wich is the next available Ipv4
        (the previous subnet Network Broadcast IP in Decimal was	198.168.1.63 so 
        the next free ip is 198.168.1.64)
    needing 20 hosts

    Press calculate.
    You'll get the following out put appended to the previous output

IP Address in Binary:	11000110.10101000.00000001.01000001
Subnet Mask in Binary:	11111111.11111111.11111111.11100000
Network IP in Binary:	11000110.10101000.00000001.01000000
====================================	=================================
Network IP in Decimal:	198.168.1.64
Subnet Mask :	255.255.255.224
First Available Host IP in Decimal:	198.168.1.65
Last Available Host IP in Decimal:	198.168.1.94
Network Broadcast IP in Decimal:	198.168.1.95
Total Number of hosts bits:	5
Total Number of IPs Available for Assignment:	30

    After you're done press print to get a printed copy of your calculations
    
