# Introduction

### What is Cryptography?

*"**Crypto algorithms** are the equivalent of locks, seals, security stamps and identification documents on the Internet. They are essential to protect our on-line bank transactions, credit cards, and personal information and to support e-commerce and e-government"*

| Term | Definition |
| :---- | :--------- |
| Cryptology | The field of both cryptography and cryptanalysis. |
| Cryptography | The study of encryption (including decryption) principles/methods that allows only the sender and intended recipient of a message to view its contents.|
| Cryptanalysis | The study of principles/methods of decrypting cipher text without knowing the key (often used by the attacker) |
|||
| Intelligible  | can be known as meaningful or capable of being understood | 

### Basic Terminology
| Term | Description |
| :--- | :---------- |
| Plaintext | original message |
| Ciphertext | encrypted message |
| Cipher / Cryptographic System | pair of algorithms for transforming plaintext to ciphertext and ciphertext back to plaintext. |
| Key | info used in cipher that are known only to `Sender/Receiver` |
| Encrypt | the process of converting plaintext to ciphertext |
| Decrypt | the process of recovering plaintext from ciphertext |

### Cryptanalytic Attacks

| Term | Description |
| :--- | :---------- |
|  Ciphertext only (COA) | Only know algorithm & ciphertext, is statistical, know or can identify plaintext |
| Known plaintext (KPA) | Know/suspect plaintext & ciphertext to attack cipher based on some plaintext-ciphertext combinations have been known in the past. |
| Chosen plaintext (CPA) | Select plaintext and obtain ciphertext to attack cipher. The attacker has access to the encryption machine. |
| Chosen ciphertext | Select ciphertext and obtain plaintext to attack cipher. The attacker has access to decryption machine. |
| Chosen text | Select plaintext or ciphertext to en/decrypt to attack cipher |

## Kerckhoffs' Principle
![](./img/TAC3121-Lec1-kerchoff-principles.jpg)
> Everything can be made public (including the algorithms) except the `private key`.

---
### Cryptography is broadly classified into two categories:
1. Symmetric / Private-Key Cryptography
2. Asymmetric Key Cryptography / Public-Key Cryptography

#### Symmetric Cryptography (Private-Key)
- both the `Sender` and `Recipient` share a common key, `private key`
- rely on one key to both `encrypt` and `decrypt`
- think of it like a traditional house door key, to unlock/lock it requires the common key.

### Private-Key Encryption Model
![](./img/TAC3121-Lec1-private-key-encryption-diagram-2.png)

#### Asymmetric Cryptography (Public-Key)
- Involves the use of two keys:
	- public-key - the recipient public key can be known by anyone and is used to encrypt the messages by the sender, and verify signatures.
	- private-key - only known to the recipient, and is used to decrypt the ciphertext and sign signature.
- Therefore the `Sender` who encrypt messages or verify signatures **cannot** decrypt messages or create signatures.

### Public-Key Encryption Model
![](./img/TAC3121-Lec1-public-key-encryption-diagram.png)

### Authentication using Public-Key System (Digital Signature) 
![](./img/TAC3121-Lec1-authentication-using-public-key-system-diagram.png)

### Unconditional Secure Cipher
> Even having unlimited computer power and time, the secure ciphertext still cannot be broken (decrypt); Since the ciphertext itself does not provide sufficient information to uniquely determine the corresponding plaintext.

### Computational Secure Cipher
> Given that the current computing resources (which are limited), the ciphertext cannot be broken due to the time needed to decrypt the ciphertext outweigh the content of the message.

#### Brute Force Search
+ Try every possible key on a piece of ciphertext until an intelligible translation into plaintext is obtained.
+ On average, half of all possible keys must be tried to achieve success.
	+ Always possible to simple try every key
	+ Most basic attack, proportional to key size
	+ Assume either know/recognize plaintext

![](./img/TAC3121-Lec1-brute-force-search.png)