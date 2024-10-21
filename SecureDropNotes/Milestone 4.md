**Listing Contacts**

```
This milestone presents a complex challenge, demanding meticulous design and implementation. It marks the initial phase where the application communicates over a network, expanding its attack surface. When working on this module, consider the following key points:
1. Display contact information only if certain conditions are met: the user has added the contact, the contact has reciprocated, and the contact is online on the same network.
2. Initially, implement the module without security controls, and later add security measures. Utilize TCP or UDP for communication, and consider using Python’s socket module for transport layer protocols.
3. Strive to create reusable code, especially for cryptographic functions. Leveraging Python’s pycryptodome and cryptography modules can greatly assist in the implementation of diverse cryptographic tasks. These implementations can be valuable for later use in the Secure File Transfer milestone.
4. Encrypt identities of communicating entities to safeguard against packet sniffing. Compromise of contact information can lead to spam and targeted attacks.
5. Mitigate impersonation attacks; implement a protocol for mutual authentication between entities.
6. Consider exchanging unique and protected information between entities to enhance security without requiring reauthentication in subsequent steps. Ensure this information remains confidential.
```

Key Notes:

This will be the hardest milestone of the project, demanding the most time and work. This will work best if it is broken up before attempted. We should, as the notes suggest, first implement without security and add security as we go as to not overcomplicate things.

Networking as a topic is the most important topic to understand for this task. We'll need to establish and detect the connection a user makes when logging in, yet we will need to do this in a secure way to defend against compromise from traffic analysis.

Security to be added:

A lot; encryption of identities, encryption of login information over a network, safeguard against impersonation, eventual PGP encryption of data to be transmitted (tbf)