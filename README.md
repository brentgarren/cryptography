# cryptography
Terminology
Symmetric encryption, such as AES<br>
Asymmetric encryption, such as RSA<br>
Diffie-Hellman Key Exchange<br>
Hashing<br>
PKI - an arrangement that binds public keys with respective identities of entities (like people and organizations).<br>
Cryptographic Algorithm or Cipher - This algorithm defines the encryption and decryption processes.<br>
Key - The cryptographic algorithm needs a key to convert the plaintext into ciphertext and vice versa.
plaintext - is the original message that we want to encrypt<br>
ciphertext - is the message in its encrypted form<br>

--------------

One of the simplest form of cryptography is the caeser cipher. Wherein you shift every letter either further or backwards an "X" amount of spaces.

The caeser cipher is considered a substition cipher as each letter is substitued with another letter.<br>
![cypher1](https://user-images.githubusercontent.com/105601437/217408704-e69a8bf9-042d-4b12-aef8-80e2c91f7829.png)
<br>

--------------

Transpositional Cipher which mixes the order of the letters while still substituting each letter for another "X" spaces away To figure out the order of letters we would need a key for instance 12345 which would write the alphabet vertically and then using a key 5 substition to find the message. <br>

![cypher](https://user-images.githubusercontent.com/105601437/217408822-68fd7207-bc04-4600-a676-8578b9a6436c.png)
<br>

https://www.quipqiup.com/ can be used to solve simple encryption

--------------


Symmetric Encryption

A symmetric encryption algorithm uses the same key for encryption and decryption. Consequently, the communicating parties need to agree on a secret key before being able to exchange any messages.

Sender -> Plaintext -> [Encrypt(KEY)] -> CipherText -> [Decrypt(KEY)] -> Plaintext -> Recipient

During the process the Sender provides the encryption process

During the process the recipient provides the decrypt process

note that both share the same key and the key is usually transferred over a secure channel between both parties.


--------------
The Block Cipher symmetric encryption "shown below" 
<br>A block cipher algorithm converts the input (plaintext) into blocks and encrypts each block. A block is usually 128 bits. In the figure below, we want to encrypt the plaintext “TANGO HOTEL MIKE”, a total of 16 characters. The first step is to represent it in binary. If we use ASCII, “T” is 0x54 in hexadecimal format, “A” is 0x41, and so on. Every two hexadecimal digits constitute 8 bits and represent one byte. A block of 128 bits is practically 16 bytes and is represented in a 4 by 4 array. The 128-bit block is fed as one unit to the encryption method.<br>
![cypher3](https://user-images.githubusercontent.com/105601437/217410785-c51a1954-ec1d-4b24-8f38-7622184c1511.png)<br>

--------------

The other type of symmetric encryption algorithm is stream ciphers, which encrypt the plaintext byte by byte. Consider the case where we want to encrypt the message “TANGO HOTEL MIKE”; each character needs to be converted to its binary representation. If we use ASCII, “T” is 0x54 in hexadecimal, while “A” is 0x41, and so on. The encryption method will process one byte at a time. This is represented in the figure below.<br>
![cypher4](https://user-images.githubusercontent.com/105601437/217410816-2af8806b-b450-4f5d-b544-d9b866bdfbd7.png)<br>


--------------

One of the biggest problems with symetricall encryption is scalability for instance if we had 3 users who needed to share information Bob Tom and Max.
We would need a Bob -> Tom Tom -> Max and Bob -> Max 
With more users for instance 100 users would require 5000 keys with each paring requiring a unique key with every other person.
With the added issue being if one system is compromised you have the regenerate another 5000 keys for every user again

--------------


