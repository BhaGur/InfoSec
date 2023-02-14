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

## Hashcat
### Installing Hashcat
I installed Hashcat according to steps given in Karvinen 2022: Cracking Passwords with Hashcat
*	I installed the hashcat using the following code
  <img src="https://github.com/BhaGur/InfoSec/blob/main/hashcat1.png" width="600" height="200"> 

*	After that I created a directory and downloaded a database with password.
  <img src="https://github.com/BhaGur/InfoSec/blob/main/hashcat2.png" width="600" height="150"> 

*	I tried to get the first 10 words of the file
  <img src="https://github.com/BhaGur/InfoSec/blob/main/hashcat3.png" width="600" height="200"> 


### Cracking the code
*	To crack the given code, I used the following code as shown in the picture
  <img src="https://github.com/BhaGur/InfoSec/blob/main/hashcat4.png" width="600" height="150"> 

*	Once the code was entered, the session started and once the code was cracked the status changed to ‘Cracked’.
  <img src="https://github.com/BhaGur/InfoSec/blob/main/hashcat5.png" width="600" height="200"> 

*	Then I input the code ‘ cat solved’ and the answer was shown along with the hash
*	The answer was february.

## John The Ripper
### Installing John The Ripper
*	First I installed the re-requisites as follows
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper1.png" width="600" height="200"> 

*	Then, I downloaded or cloned john the Ripper version with the help of the following command as shown in the picture
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper2.png" width="600" height="200"> 

*	Then I had to configure the file 
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper3.png" width="600" height="200"> 

*	Then after the configuration, a correct make command is printed in the end which I copied and run to compile John
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper4.png" width="600" height="200"> 

*	Finally John The Ripper was downloaded and I could see the version downloaded by running the following command
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper6.png" width="600" height="200"> 

### Cracking zip file
*	The zip file was downloaded using the following commands from TeroKarvinen.com
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper7.png" width="600" height="200"> 

*	I tried to unzip the file but was not successful
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper8.png" width="600" height="200"> 

*	I then followed next step to extract the hash into a new file
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper8.png" width="600" height="200"> 

*	Next I used command to let John attack the hash.
   <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper9.png" width="600" height="200"> 

*	The attack resulted in printing the password as a key line (in brown colour)
*	The password is ‘butterfly’ which I used to unzip the file
  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper10.png" width="600" height="200"> 


* The SECRET file contained a message as follows

  <img src="https://github.com/BhaGur/InfoSec/blob/main/johnripper11.png" width="600" height="200"> 


## References
* Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.
* https://terokarvinen.com/2022/cracking-passwords-with-hashcat/
* https://terokarvinen.com/2023/crack-file-password-with-john/
