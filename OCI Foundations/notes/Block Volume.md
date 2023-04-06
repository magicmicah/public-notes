Provides persistent and durable storage to compute instance. 

Can create, delete, attach, detach. The block volume even persists after the instance is terminated. Multiple copies can be made.

## Tiers
### Basic
large sequential I/O workloads
### Balanced
Balanced choice for random I/O
### Higher Performance
most demanding
### ultra higher performance
Highest demanding

### Auto tune performance
Will automatically change your tiering based on your needs. 

Encrypytion is automatically turned on by default. You can bring your own keys. Encryption is setup automatically between instance and block volume storage service. 

### Read/Write Shareable

Allows multiple VMs to read and write to the same volume.

### Online resizing
Keepy instance online and resize while block volume is in use.

### Replication 

Replicate block volumes across regions for DR, Migration and Business Expansion.

### Volume Groups
Group volumes together to simplify the process of creating consistent backups of running applications. 