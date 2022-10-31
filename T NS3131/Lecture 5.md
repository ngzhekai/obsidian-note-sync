# Chapter 5: Electronic Mail Security

### Pretty Good Privacy (PGP)

+ popular program and open source
+ to provide confidentiality and authentication services for electronic mail and file storage
+ used primarily to **encrypt and decrypt email** over the Internet
+ designed by *Phil Zimmermann* in 1991

The following services offered by PGP:
1. Authentication
2. Confidentiality
3. Compression
4. Email Compatibility
5. Segmentation

![PGP Operation - Authentication](./img/lecture5-pgp-authentication.jpg)

As shown in the figure above, the **hash function *H* will calculate the hash value of the message using ***SHA-1*** (where it generate a 160-bit hash value). Then, using the sender's private key ***KR<sub>a</sub>*** the hash code will be encrypted and it is called **Digital Signature**. After that, message will be appended to the signature. All the process that happened till now, is known as signing the message. And to reduce the overhead during transmission, the message will undergo compression before sending over to the receiver.

At the receiver end, the data is decompressed ***Z<sup> -1</sup>***, and the original message ***M*** and signature ***S*** are obtained. The signature is then decrypted using the sender's public key ***KU<sub>a</sub>*** and the hash value is obtained. The message is again passed to the **hash function *H***, and its hash value is calculated and obtained.

Both the values, one from signature and another from the recent output of hash function are compared. If both are the same, it conclude that the email is actually sent from a known one and is legit. Else, not a legit one.

### Secure/Multipurpose Internet Mail Extension (S/MIME)



