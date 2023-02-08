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

note that both share the same key and the key is usually transferred over a secure channel between both parties.


--------------
