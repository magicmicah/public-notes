
Internet scale high performance storage platform. Data is managed as objects. Ideal for unstructured data - photos, videos, log files, text files. 
Regional, public service. Multipe storage tiers. Private access from OCI resources and advanced capabilities available.

Any object stored in Object Storage is stored as key value pairs. Objects will have metadata and can be customized too. Objects are sorted in buckets. Buckets are unique in tenancy and have a flat hierarchy. Also must have a globally unique namespace. 

![[object-storage-resources.png]]

### Standard storage tier
* Fast, immediate and frequent access
* most recent copy of data
* instantaneous retrieval
* Can't be downgraded.

### Infrequent access storage tier
* Ideal for data that you access infrequently
* Minimum retention requirement - 31 days. 
* Storage costs lower than standard tier - 60% cheaper
* Retrieval fees. 

### Archive Storage Tier

* Seldom or rarely accessed - tape storage in the cloud
* Minimum retention - 90 days
* Objects need to be restored before download
	* Restore time: 1 hour
	* Download time: 24 hours. 

### Auto-Tiering

Allows automatic tiering of data depending on how often you access data. 


### Lifecycle Management

Hot tier vs cool tier. Allows moving of data automatically for you.

### Versioning

Allows versioning data as you use it. 

### Data Encryption
Data is automatically encrypted. you can let Oracle store the encryption keys or bring your own keys. 