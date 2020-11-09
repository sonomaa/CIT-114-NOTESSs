# Notes 5: Networking & Content Delivery

### What is a Network?
- a computer network is just two or more client machines that are connected together, using a network device, to share resources. 
### Computer Network
-  interconnection of multiple devices, generally termed as Hosts connected using multiple paths for the purpose of sending/receiving data or media.
### Amazon VPC
- Amazon VPC lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define.
- You have complete control over your virtual networking environment. 
- Create an Amazon VPC on AWS's scalable infrastructure and specify its private IP address range from any range you choose.
### VPCs and Subnets
- After creating a VPC, you can add one or more subnets in each Availability Zone. You can optionally add subnets in a Local Zone, which is an AWS infrastructure deployment that places compute, storage, database, and other select services closer to your end users. 
###  IP Addressing in your VPC
- IP addresses enable resources in your VPC to communicate with each other, and with resources over the Internet.
- By default, Amazon EC2 and Amazon VPC use the IPv4 addressing protocol. When you create a VPC, you must assign it an IPv4 CIDR block. 
### Elastic Network Interfaces
- virtual network interface that can include the following attributes:a primary private IPv4 address,secondary private IPv4 addresses, one Elastic IP address per private IPv4 address, one public IPv4 address, which can be auto-assigned to the network interface for eth0 when you launch an instance, one or more IPv6 addresses
one or more security groups, a MAC address, a source/destination check flag, a description. 
### VPC Route Tables
- A route table contains a set of rules, called routes, that are used to determine where network traffic from your subnet or gateway is directed. Each route specifies a destination and a target.
- Main route table - The route table that automatically comes with your VPC. It controls the routing for all subnets that are not explicitly associated with any other route table.
### Internet Gateway
- horizontally scaled, redundant, and highly available VPC component that allows communication between your VPC and the internet. An internet gateway serves two purposes: to provide a target in your VPC route tables for internet-routable traffic, and to perform network address translation (NAT) for instances that have been assigned public IPv4 addresses.
### Network Address Translation (NAT)
- You can use a NAT device to enable instances in a private subnet to connect to the internet (for example, for software updates) or other AWS services, but prevent the internet from initiating connections with the instances. A NAT device forwards traffic from the instances in the private subnet to the internet or other AWS services, and then sends the response back to the instances. 
### Working with shared VPCs
- VPC sharing offers several benefits: Separation of duties, Ownership , Security groups 
### VPC Peering
- A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them privately. Instances in either VPC can communicate with each other as if they are within the same network. 
### VPN's
- Allows a user to connect one remote private network to a seperate remote private network through a secure virtual tunnel over the public internet. Many companies use this technology to connect seperate locations in order to grant employees the ability to access company resources anywhere in the world.


### TWO QUOTES: 
- "One of the challenges of network communication is network performance. Performance can be negatively affected if your data center is located far away from your AWS Region." 
- VPC sharing enables you to decouple accounts and networks. You have fewer, larger, centrally managed VPCs. Highly interconnected applications automatically benefit from this approach.

### NEW FACTS
- Companies use VPNs to allow employees to work in different countries. A VPN allows for the employee to have the same computing visual as they would on the job site. 
- NAT gateways provide better availability and bandwidth over NAT instances.

### QUESTIONS: 
