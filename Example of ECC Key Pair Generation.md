**W05 Discussion: Module 7 NIST CT (Security for Life)**

The National Institute of Standards and Technology (NIST) is a non-regulatory agency of the United States Department of Commerce whose mission is to promote innovation and industrial competitiveness. NIST is heavily involved in cryptographic technologies.

For this “Security for Life” activity you will read and summarize information from the NIST Cryptographic Technology website ([ csrc.nist.gov/Groups/Computer-Security-Division/Cryptographic-Technology ](https://csrc.nist.gov/Groups/Computer-Security-Division/Cryptographic-Technology)). The posting that you select must be unique and not one that another learner has already posted about for this class. 

- [x] First, read through all previous postings by other learners and make note of those documents that have already been researched.
- [x] Then, go to the NIST Cryptographic Technology website ([ https://csrc.nist.gov/Groups/Computer-Security-Division/Cryptographic-Technology ](https://csrc.nist.gov/Groups/Computer-Security-Division/Cryptographic-Technology)) and select a category (a project) of interest.
- [x] Read the information about this topic.
- [x] Post your summary (minimum of 100 words). Include your opinion of the value of this information and assign it a grade (1–10) regarding its value and how you could use this information.
- [ ] Finally, post a reply to another learner’s initial posting (minimum of 50 words).





***Article:  Recommendations for Discrete Logarithm-Based Cryptography: Elliptic Curve Domain Parameters***

***Authors:*** Lily Chen (NIST), Dustin Moody (NIST), Andrew Regenscheid (NIST), Karen Randall (Randall Consulting)

***Site:*** https://csrc.nist.gov/pubs/sp/800/186/ipd

***Difficulty:*** 10/10



So, the Post Quantum topic looked real fun and talked about Star Trekky stuff like Dilithium Crystals. But, alas, Michael got to that topic before I could, dang it. I'll choose Eliptic Curve Cryptography. Firstly, this method involves some hefty mathematical Kung Fu. It is extremely difficult to derive the private key (d) from an eliptical curve formed from the formula `y^2 = x^3 + 2x + 3` even if you know the public key (Q).

### **Example of ECC Key Pair Generation**

Let's walk through a simplified ECC key pair generation example using a curve like `y^2 = x^3 + 2x + 3` over a small finite field modulo 5. (In practice, much larger fields are used for real security.)

1. **Choose a base point (P)** on the curve. Let’s say `P = (2, 4)` is a point on the elliptic curve defined by the equation above.
2. **Private Key (d)**: Select a random number as your private key. For example, let `d = 3`.
3. **Public Key (Q)**: Multiply the base point `P` by the private key `d` to get the public key `Q`. This involves performing elliptic curve point addition. After calculating, you get `Q = 3 * P = (resulting point)`.

In reality, the calculations are far more complex, and the finite field size is much larger (e.g., 256-bit integers).

### **Why ECC?**

- **Smaller Keys**: ECC offers the same level of security as RSA but with much smaller key sizes. For instance, a 256-bit key in ECC is as secure as a 3072-bit key in RSA.
- **Efficiency**: Smaller keys lead to faster computations and lower power consumption, which is important for mobile devices and other constrained environments.

### Example of Real-World Use: Bitcoin

In Bitcoin, ECC is used for signing transactions. The Bitcoin network uses the curve **secp256k1**, and each user has a private key (used to sign transactions) and a public key (used to verify them).

#### Eliptic Point Addition

Imagine a doughnut shaped elipse with an infinite number of points describing it's curvilinear edge. Now, pick a point on the curve as shown above like (2, 4). Your Public key would be another resulting point on the curve where Q = 3 * p. You "add" or double a point when you create new tangental lines through the same elipse. This activity creates a mathematically difficult problem that happens to have enough density that starting with an ECC-256 bit point is adequate and provides a much faster calculation than its sibling RSA-3072 bit key. Unfortunately, 100 words is no where near enough space to cover what's going on; however, you can go to the following sites for more information. I am also punting because I am not the mathematician I should be to adequately discuss what happens. Maybe I could do it in 100 pages instead of 100 words. But then, I would have a PhD title beside my name had have friends like Lily Chen and Dustin Moody.

### **Further Reading and References**

- **NIST ECC Recommendations**: [NIST SP 800-186](https://csrc.nist.gov/publications/detail/sp/800-186/draft)
- **Introduction to Elliptic Curve Cryptography**: Certicom ECC Tutorial
- **RFC 6090**: Basic Elliptic Curve Cryptography (ECC) Algorithms: RFC 6090

Elliptic Curve Cryptography offers a highly efficient and secure method for encryption, making it a cornerstone in modern cryptography, especially for resource-constrained environments like mobile and IoT devices.