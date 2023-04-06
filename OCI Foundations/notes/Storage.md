Storage Requirements should be consdered first before deciding. Things such as:

persistent vs non persistent
Waht type of data? dbs, videos, audio, photos, text?
What performance? IOPS? Capacity? Throughput?
Durability?
Connectivity - local, network and how data is accessed
Protocol - Block, File, HTTP

![[storage-options.png]]
## Local NVMe
locally attached storage - NVMe SSDs. Performance sensitive applications.

## Block Volume
Locally attached storage is moved to a remote service called a block volume. 

## File Storage
Exists in the same AD, but its a shared file storage for two instances. File systems are mounted and shared.

#