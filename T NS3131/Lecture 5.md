# Electronic Mail Security

### Pretty Good Privacy (PGP)

+ Popular program used primarily to **encrypt and decrypt email** over the Internet, 

![](./img/lecture5-pgp-authentication.jpg)

As shown in the figure above, the **hash function *H* will calculate the hash value of the message using ***SHA-1*** (where it generate a 160-bit hash value). Then, using the sender's private key ***KR<sub>a</sub>*** the hash code will be encrypted and it is called **Digital Signature**. After that, message will be appended to the signature. All the process that happened till now, is known as signing the message. And to reduce the overhead during transmission, the message will undergo compression before sending over to the receiver.

At the receiver end, the data is decompressed ***Z<sup>-1</sup>***, and the original message ***M*** and signature ***S*** are obtained. The signature is then decrypted using the sender's public key ***KU<sub>a</sub>***

### Secure/Multipurpose Internet Mail Extension (S/MIME)



