

Region - localized geographic region containining one or more availability domains

  

availability domains - one or more fault tolerant data centers within a region

  

ADs are connected together by low latency high bandwidth networks

  

Fault Domains - Logical datacenters within datacenter. Anti-affinity

  

Multi cloud, hybrid cloud with Azure.

  

Regions should b e chosen for your requirements - promixity to users, compliance, data residency. New services are made available based on regional demand, compliance, etc. 

  

ADs are isolated from each other, fault tolerant and unlikely to fail together. They do not share power, cooling or network.

  

Each AD has three fault domains. Resources are placed in different FDs and they won't share single points of failure such as same racks or networking gear.