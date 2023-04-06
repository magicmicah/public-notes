Managed service that manages encryption keys and credentials. Keys like ssh keys, crdential files, passwords, etc. 

Two levels of protection - software and hardware modules. Hardware meets FIPS 140-2 standards. The master key for a hardware security machine is stored on the HSM. All cryptography occurs on the HSM.

Software store in server, can be exported, operations allowed on clients. 

Algorithms - Vault supports AES, RSA and ECDSA keys. 

AES - the same key encrypts and decrypts data
RSA - asymmetric encryption with a public and private key
ECDSA - used in digital signing but cannot be used to encrypt or decrypt

Keys are integrated with other OCI services. Master key rotation is possible.

Vault is regional and has a public API endpoint available. 

Vault works with envelop encryption - a two tier hierarchy. The data encryption keys encrypt the customer data and the master encryption keys actually encrypt the data keys. 

IAM policies can set who is allowed to access master keys and audit logs to monitor all key related activity. 

Benefits - limited blast radius, easier to manage, doesnt generate a complete data re-encryption.

If master key is deleted, no way to recover data. Keys are soft deleted with a seven day gap and backups should be taken often. Vault cannot be immediately deleted and it will schedule to delete 7-30 days later. 

![[vault-encryption.png]]