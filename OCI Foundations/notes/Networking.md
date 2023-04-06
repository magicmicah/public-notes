  
## VCN

Private software defined network for use in OCI.

VCN has an address space given in CIDR notation. 10.0.0.0/16

Subnets are broken down into public and private subnets.

### Internet Gateway

Public services are server through an internet gateway

### NAT Gateway

Enables outbound communication from private subnet to internet but not back in. 


### Service Gateway

Lets resources in VCN access public OCI services such as object storage but not through NAT or Internet gateway. 

### Dynamic Routing Gateway

Virtual router that provides a path for private traffic between VCN and destinations other than internet. 


### Routing

VCNs route traffic to internet, on premise, other VCNs, etc.

Route rules with destination CIDR and route target - route target is the next hop. Traffic within VCN does not need to be routed.

### Peering![[local-peering-vs-remote-peering.png]]
If networks are in same OCI region, they can communicatve via local peering. 

If two networks are in different OCI regions, they can communicate via remote peering. Remote peering uses Dynamic Routing Gateways.

As more VCNs are created, complexity arises. Dynamic Routing Gateway v2 no longer requires a local peering gateway and VCNs allow scalability up to 300 DRGs. Additional networks can be peered through Remote peering connection
