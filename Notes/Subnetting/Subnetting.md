# Subnetting

An IP Address is 32 bits long and consists of two components - **Network Bits** and **Host Bits**

The network id is used to identify the network and is common to all devices on the network while the host id is used to identify a particular device on a network.



**Subnetting** is the concept of dividing the network into smaller portions called 'subnets'.



Typically, the first IP address available is the **Network ID** and the last address if the **Broadcast ID**.

<br>


Things to Remember:
> * Hosts double each increment of a CIDR
> * Always Subtract 2 from host total: <br>* Network ID - First Address <br>* Broadcast ID - Last Address


<br>

Helpful online tool - [IP Address Guide](https://ipaddressguide.com/cidr)

<br>

<div align="center">

![Subnetting Cheat Sheet](SubnettingCheatSheet.png "Subnetting Cheat Sheet")

<br>
<br>



|Address        |Subnet         |Hosts (excluding network and broadcast)|Network ID  |Broadcast ID |Useable Addresses        |
|---------------|---------------|:-------------------------------------:|------------|-------------|-------------------------|
|192.168.1.0/24 |255.255.255.0  |254                                    |192.168.1.0 |192.168.1.255|192.168.1.1-192.168.1.254|
|192.168.1.0/28 |255.255.255.240|14                                     |192.168.1.0 |192.168.1.15 |192.168.1.1-192.168.1.14 |
|192.168.1.16/28|255.255.255.240|14                                     |192.168.1.16|192.168.1.31 |192.168.1.17-192.168.1.30|
|192.168.0.0/23 |255.255.254.0  |510                                    |192.168.0.0 |192.168.1.255|192.168.0.1-192.168.1.254|
|192.168.2.0/23 |255.255.254.0  |510                                    |192.168.2.0 |192.168.3.255|192.168.2.1-192.168.3.254|
|192.168.0.0/22 |255.255.252.0  |1022                                   |192.168.0.0 |192.168.3.255|192.168.0.1-192.168.3.254|
|192.168.1.0/26 |255.255.255.192|62                                     |192.168.1.0 |192.168.1.63 |192.168.1.1-192.168.1.62 |
|192.168.1.0/27 |255.255.255.224|30                                     |192.168.1.0 |192.168.1.31 |192.168.1.1-192.168.1.30 |

</div>