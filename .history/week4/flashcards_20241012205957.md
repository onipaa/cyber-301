




## Module 6 cryptography
---
### Flashcard Set: Cryptography Concepts

1. **Q:** Which of these provides cryptographic services and is external to the device?  
   **A:** Hardware Security Module (HSM)

2. **Q:** Cryptography can prevent an individual from fraudulently reneging on an action. What is this known as?  
   **A:** Nonrepudiation

3. **Q:** What type of attack forces the system to abandon a higher cryptographic security mode of operation and fall back to a less secure one?  
   **A:** Downgrade attack

4. **Q:** Which of the following is not to be decrypted but is only used for comparison purposes?  
   **A:** Digest

A **digest** is the result of a cryptographic hash function, which takes an input (or message) and returns a fixed-length string of characters, typically a hexadecimal number. The digest is unique to the input, meaning that even a small change in the input will produce a vastly different digest. A digest is not meant to be decrypted because it doesn't contain the original data—it's a one-way function.

**Purpose of a Digest**:
- **Verification**: It's used to compare and verify that a message or file hasn't been altered. When you hash the same data again, the resulting digest will be the same if the data is unchanged.
- **Integrity Check**: For example, when downloading files, the digest (often referred to as a checksum) is provided so that users can verify the file's integrity after download by comparing the computed digest of the file with the original one.

In this case, the correct answer to the question is **Digest**, as it is not meant to be decrypted but is used for comparison purposes, like verifying integrity.

5. **Q:** Which of the following is NOT a characteristic of the Trusted Platform Module (TPM)?  
   **A:** It can easily be transported to another computer.

6. **Q:** Which characteristic of cryptography makes information obscure or unclear, making the original information impossible to be determined?  
   **A:** Obfuscation

7. **Q:** Which encryption chip on the motherboard provides cryptographic services?  
   **A:** Trusted Platform Module (TPM)

8. **Q:** Which principle can be used to verify a manager's claim of sharing a list of employees and later denying it?  
   **A:** Nonrepudiation

**Nonrepudiation** is a concept in cryptography and information security that ensures a party involved in a communication or transaction cannot deny the authenticity of their signature or the validity of the message sent. It provides proof of the origin and integrity of the data, and this proof can be verified by any third party.

In the context of cryptography, nonrepudiation is typically achieved through the use of digital signatures or other cryptographic techniques that link a message to the sender in a way that cannot be later disputed. It is crucial for ensuring trust in electronic transactions, legal communications, and secure messaging systems.

9. **Q:** What type of cryptographic algorithm uses two keys, one public and one private?  
   **A:** Asymmetric cryptographic

10. **Q:** Which of the following uses hardware encryption technology to secure stored data and ensures SEDs' inseparability among vendors?  
   **A:** Opal
   
Opal refers to a security standard developed by the Trusted Computing Group (TCG) for **self-encrypting drives (SEDs)**. These drives use hardware-based encryption to secure data at rest. Opal-compliant drives ensure that encryption is done at the hardware level, meaning that the encryption keys never leave the drive itself, which enhances security.

Key aspects of Opal include:
- **Data Security**: Encryption is transparent to the user, as all data written to the disk is automatically encrypted.
- **Interoperability**: Opal ensures that self-encrypting drives can work across different platforms and vendors, making them portable and standardized.
- **Management**: Opal-compliant drives often come with features for management, such as locking the drive with passwords or other authentication methods.

In summary, Opal is a standard that ensures secure and vendor-independent self-encrypting drives.


11. **Q:** Which cryptographic function takes a string of any length as input and returns a string of any requested variable length?  
   **A:** Sponge

12. **Q:** Which of the following devices can perform cryptographic erase?  
   **A:** Self-encrypting hard disk drives (SED)

13. **Q:** Which attack involves determining the hash function's input strings that produce the same hash result?  
   **A:** Collision attack

14. **Q:** Which cryptographic method is used to create a sequence of numbers that closely resemble random numbers?  
   **A:** Pseudorandom number generator (PRNG)

15. **Q:** Which feature of cryptography is used to prove a user's identity and prevent an individual from fraudulently reneging on an action?  
   **A:** Nonrepudiation
---