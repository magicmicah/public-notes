
Also referred to fine grained access control or Role Based Access Control.

  

AuthN - Who are you?

AuthZ - What are you permissioned to?

  

OCI Identity Concepts

  

Identity Domains  - represents a user population in OCI and associated configurations and security settings.

  

Identity Domains get created with Users and Groups which are assigned to Policies and with each Compartment (a logical isolation) they are assigned resources.

  

Anything you create in the cloud is a resource. Resources are all have unique identifiers - Oralce Cloud ID (OCID)

  

Ex. ocid1.<resource type>.<realm>.[Region][.futurue use].<unique id>

  

Compartments are  logical seperation of resources for isolation and control of access.

  

Root Compartment - created when the tenant is created. All OCI resources can be installed in the root compartment but best practice is to put resources in the logical compartments.

  

EAch resource belongs to a compartment. They can interact with other compartments easily. Resources can be moved between compartments.

  

Compartments are global constructs - resources from multiple regions can be in the same compartment. Policies can be created to restrict access.

Compartments  can be nested up to six levels. 

Compartments can have quotes and budgets set individually on them.

  

Principal are IAM entities that are allowed to interact with OCI resources.

  

IAM Users - an example principal, these are the users who are using the cloud resources

Resources - another example of principals, they can make API calls against other services

Groups - Collection of Users that have shared access to similar resources.

  

Authentication - Who are you?

Username/Password

API Signing Keys - public/private RSA key pair

Tokens - Oracle generated token strings. Useful for authenticating third party APIs

  

Authorization - What are you allowed to do?

IAM Policies - human readable statements to define granular permissions

  

Allow group group_name to verb resource-type in tenancy/compartment

Allow group_name to verb resource-type in location where condition

  

  

Tenancy setup - create individual compartments for everything. don't use the tenancy admin account for day to day

Enforce MFA.