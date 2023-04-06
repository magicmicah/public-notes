
Load Balancer achieves high availability and scalability. The LB will reverse proxy traffic to backend servers. LBs include advanced features like TLS termination. 

## Layer 7 Load Balancer
Understands HTTP/S and includes several specific capabilities. 

### Flexible Shape
Flexible shapes (deprecating in May 2023) allows a minimum and maximum range of traffic.

### Dynamic Shape
Bandwidth is predefined - micro, small, medium, large. LB does not have to be warmed up, the LB will automatically scale to the traffic. 

### Public vs Private

LBs can be public or private depending on your needs.

## Network Load Balancer

Operates at Layer 4 (TCP/UDP/ICMP). Supports public or private options. Highly availbale, highly scalable. 


## NLB vs layer 7
NLB is lower latency and faster, so its more performant. Layer 7 does packet inspection and gather intelligence and create routing decisions for you. 