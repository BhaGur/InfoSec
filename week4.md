# Week 4 assignment (Hash)
This file consists of the tasks regarding week 4 assignment. The topics below consists of summary of two chapters about One-way function and One-way hash function.
the file also contains steps about installing Hashcat and using it to crack a provided code.

## Applied Cryptography Chapter 2
### 2.3 One-way functions
* One-way function is an important element to public-key cryptography.
* Though it is easy to compute, but to reverse will be an uphill task.
* Even though many functions look and feels like one-way function, but there is no evidence that one-way function exists.
* Using one-way function is not useful as it will be hard to decrypt it.
* Trapdoor one-way function consists of a secret trapdoor which have some information that can help to compute the one-way functions.
* For example, it is easy to disassemble a watch into hundreds of parts but it is hard to put it back together. However, with assembly instructions it is somewhat easier to put the pieces together.

### 2.4 One-way hash functions
* One-way hash function is also known as compression function, contraction function, fingerprint and some more names.
* Hash function takes a variable-length input string called a pre-image and converts it to a fixed-length output string called a hash value.
* The point is to produce a value that indicates whether a candidate pre-image is likely to be similar to the real-image.
* One-way hash function works in one direction, so it is easy to compute a hash value from pre-image but not the other way around.
* Generating two pre-images with the same hash value is difficult.
* As hash function is public there is no secrecy to the process.
* For example, if you want to make sure that somebody has a particular file, you can ask for the hash value. Normally the hash function is without a key but a secret key can be created and only the person with the key can verify the hash value.

## References
* Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.
