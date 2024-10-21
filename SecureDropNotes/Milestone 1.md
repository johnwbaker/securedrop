**User Registration**

```
When implementing this module, consider the following:
1. Database implementation is not required; simple files, YAML, or JSON structures suffice.
2. Initially, implement the module without security controls. After verifying its correctness, introduce security measures to protect against traditional password cracking attacks.
3. Emphasize code reusability. The password protections can be reused in the User Login milestone.
4. Utilize third-party APIs; the Python crypt module is valuable for implementing salted hashes for password security.
5. Generate and store information during registration for mutual authentication in future milestones. Assuming a CA (Certificate Authority) is present and trusted on all clients can facilitate the use of digital certificates.
```

Key Notes:

Very very similar to Activity 1, can most likely be reused/modified slightly and then reused. Without security, will pretty much be entering name, email, password x2, and storing to JSON files, being able to access files to check if user exists later

Security to be added: 

Password obfuscation, password hashes, (tbf)