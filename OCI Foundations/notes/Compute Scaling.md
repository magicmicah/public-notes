
## Horizontal Scaling
Also known as autoscaling. Adds more VMs of the same shape that allows scaleout deployment. Provides high availability and allows adding/removing VMs based on traffic. 

### How do?
Must create a template of your image which includes OS image, metadata, stamp, etc - a stamp of the image. That stamp is added into something called a instance pool. Then you take that pool and create autoscaling rules with a desired size, thresholds and maximum size. 


## Vertical Scaling

SCale upwards - memory, cpu, disk. Downtime is required for scaling up as hosts are reconfigured and may be migrated. 

