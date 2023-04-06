Provides virtual machines.

## Flexible Shapes
Choose your own cores, CPU type, memory. AMD, Intel and Ampere ARM based processors are available. 

## Virtual Machine

Shared, multi tenant. Strong security isolation. 

## Bare Metal

## Dedicated Host

No other customers on there. 


## Costs

Preemptible VMs allow reduced costs with short lived VMs for batch processing. 

## Instance Basics

An instance is a compute host. A region is composed of multiple Availability Domains. A vitual network card is attached to the host and placed inside the subnet. 
The compute host also depends on boot volumes and block volumes. The image determines the operating system where the host boots off a network disk. There is also data disks that combine for a block volume. 

### Live Migration

If one of the compute hosts go down, the virtual machine will be live migrated between hosts without rebooting. This is an opt-in feature. 