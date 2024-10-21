**Secure File Transfer**

```
The complexity of this milestone depends on previous milestones. Key considerations include:
1. Efficiently transmit large files while maintaining file confidentiality and integrity. The received file must match the transmitted one before notifying the user of a successful transfer.
2. Mitigate replay attacks by using sequence numbers, starting with a random seed on each client.
```

Key Notes:

Assuming every previous milestone has been done correctly and securely, this milestone should not be too strenuous. Some important things to take away are using PGP encryption for the transmission of large files, and also hashing and comparing the hashes of files to ensure no information has been modified.

Security to be added: 

PGP encryption, file hashing and comparation, proper and unbreakable random seeds, look into replay attacks

