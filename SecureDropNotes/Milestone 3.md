**Contact Adding**

```
This module is relatively simple and can be implemented quickly. Key points to consider include:
1. Database implementation is unnecessary; simple files, YAML, or JSON structures suffice. Assume that each user will have a limited number of contacts.
2. Explore ways to use information generated in Milestone 2 to ensure the confidentiality and integrity of contact information. Prevent unauthorized access or tampering by malicious actors.
```

Key Notes:

Without looking too much in detail to this, first assumption would be to make another JSON file for contact information, potentially using the initial login information to check if user exists before adding

Security to be added:

Need to ensure no information can be gathered by adding someone (i.e. password hash)