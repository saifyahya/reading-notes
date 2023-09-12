## Password Hashing
- Hashing is a process in computing and cryptography where data, like a password, is transformed into a fixed-length string of characters, which looks like a random jumble of letters and numbers. This transformation is done in a way that makes it extremely difficult to reverse and figure out the original data from the hash.

- Imagine a hash function is like a magic blender for passwords. You put your password in, and it comes out looking like a bunch of random letters and numbers. But the cool thing is, you can't turn it back into your original password. It's like turning your secret recipe into a bunch of colorful jigsaw puzzle pieces – easy to make, really hard to unmake. This helps keep your password safe from bad guys who might try to steal it.

## bcrypt overview
- 'Salting' a password means adding a unique and random string of bytes to the password before applying a hashing algorithm. This added string, known as the 'salt,' increases the complexity of the hash and enhances password security.

- To find the 'salt' string for passwords, a hacker would typically need access to the source code or storage where the 'salt' is stored for each user. Without access to this information, it becomes much more challenging for the hacker to crack the passwords.

## jBCrypt 
- The Blowfish block cipher, as implemented in jBCrypt, handles the increased computation speed of new computers by allowing the computation cost of the algorithm to be parametized. This means that the cost, or work factor, of the hashing algorithm can be adjusted to increase with the speed of computers. As computers become faster, the work factor can be increased, making password hashing more computationally intensive and time-consuming, thereby frustrating fast hardware implementations and raising the cost of offline password cracking.

- The issues with the two most common password hashes for Java, "Java password hash" and "Java password encryption," are as follows:
1. "Java password hash" often uses unsalted hashes, which are vulnerable to reverse dictionary attacks. Unsalted hashes do not incorporate a unique and random 'salt' value for each password, making it easier for attackers to precompute hash values for common passwords and look them up in a table.
2. "Java password encryption" recommends reversible encryption, which means that the original passwords can be decrypted back from the stored values. Reversible encryption is rarely needed for securely storing passwords and should only be used as a last resort because it exposes passwords to potential decryption if the encryption key is compromised. It's generally recommended to use irreversible hashing (like bcrypt) with salts for password storage instead.