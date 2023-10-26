## Hash Tables
- WHY:
Imagine you work at a busy mail sorting office, and your job is to efficiently sort thousands of letters. To make this task easier, you need a systematic way to quickly find and place each letter. This is where hashing comes in.

- WHAT:
Hashing:

Hashing is like converting the addresses on letters into a simple code, making it easier to find their destination.
It's similar to changing complex keys (like addresses) into unique numbers (the codes).
Hash Function:

A hash function is like a magic formula that takes an address (key) and turns it into a code (hash).
Think of it as a unique transformation that makes each letter's code special.
Hash Table:

A hash table is like a set of mail slots with labels (buckets).
Each slot is assigned a code, and letters with the same code go to the same slot.

- HOW:
Here's how it works at the mail sorting office:
- Hashing:
WHY: To simplify the process of finding destinations for thousands of letters.
WHAT: Converting addresses into unique codes (hashes).
HOW: Use a special formula (hash function) to create codes from addresses.

- Hash Function:
WHY: To make each letter's code unique.
WHAT: A magic formula that transforms addresses into codes.
HOW: Apply the formula to each address to get a unique code.

- Hash Table:
WHY: To efficiently sort letters with the same code.
WHAT: A set of labeled slots where letters with the same code go.
HOW: Place letters in the correct slot based on their code.

- Let's see an example:
You receive a letter with the address "123 Main St, City." You need to hash it.
Apply the hash function: Add the ASCII values of each character (123+Main+St+City).
The result is 5477. So, you place the letter in slot 5477.

Quiz:
1.  What is hashing?
A. Sorting letters in a post office.
B. Converting keys into unique codes.
C. Sending letters to different cities.

2. What is a hash function?
A. A magic formula to transform addresses.
B. A list of mail slots.
C. A type of envelope.

3. What's the purpose of a hash table?
A. Storing letters.
B. Quickly finding letters with the same code.
C. Delivering letters to the wrong address.

Answers:
1. B
2. A
3. B


