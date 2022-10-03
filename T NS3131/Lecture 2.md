# Chapter 2: Conventional Encryption & Message Confidentiality

## Transforming Plaintext to Ciphertext

1. **Substitution Technique** - involves the replacement of the letters by other letters or symbols. In more detailed, the characters of plaintext are replaced, and other substitute characters, numbers and symbols are used at their place. 
> Replacing current *Char* with another *Char* in a another (e.g. shift five characters to the right, such as letter `a` will be substitute with letter `f`). Turning intelligible message into meaningless text.

2. **Transposition Technique** - Transform original messages (Plaintext) by mixing them up in random sequence. Scrambles the positions of characters to create the ciphertext.
> Example: "`come down`" will be transpose into ''`cmdwoeon`''

## Basic Terminology

| Term | Description |
| :--- | :---------- |
| Plaintext | original message |
| Ciphertext | encrypted message |
| Cipher / Cryptographic System | pair of algorithms for transforming plaintext to ciphertext and ciphertext back to plaintext. |
| Key | info used in cipher that are known only to `Sender/Receiver` |
| Encrypt | the process of converting plaintext to ciphertext |
| Decrypt | the process of recovering plaintext from ciphertext |
| Cryptography | The study of encryption (including decryption) principles/methods that allows only the sender and intended recipient of a message to view its contents.|
| Cryptanalysis | The study of principles/methods of decrypting cipher text without knowing the key (often used by the attacker) |

### Unconditional Secure Cipher

 Even having unlimited computer power and time, the secure ciphertext still cannot be broken (decrypt); Since the ciphertext itself does not provide sufficient information to uniquely determine the corresponding plaintext.
 > As redundancy in data gives extra information to break the encryption algorithms.

### Computational Secure Cipher

 Given that the current computing resources (which are limited), the ciphertext cannot be broken due to the time needed to decrypt the ciphertext outweigh the content of the message.

## Feistel Cipher Structure

