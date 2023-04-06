
## Security Lists
Like firewall rules associated with a subnet and all the instances inside the subnet.

![[security-lists.png]]

## Network Security Group

Similar to security lists but these apply only to virtual NICs. Another difference is NSGs can be the source or destination in rules. 

Inthis example, the egress traffic, the source is NSG B. So that's the NSG which is attached to my database. Similarly for the second network security group, you can see that the source is the first network security group. That's NSG A.
![[network-security-groups.png]]