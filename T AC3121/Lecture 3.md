# Chapter 3: Classical Ciphers

#### 2 Main Categories of Classical Ciphers:

| No. | Term | Definition |
| :--- | :--- | :--- |
|||
| 1. | **Substitution** | Letters are replaced by other letters, categorized as mono-alphabetic or poly-alphabetic |
|||
| 2. | **Transposition** | Letters are arranged in a different order |
|||

Comparison between *Mono-alphabetic* and *Poly-alphabetic* Substitution Ciphers:

| | **Monoalphabetic Cipher** | **Polyalphabetic Cipher** |
| :--- | :--- | :--- |
| Definition |Monoalphabetic cipher is one where each symbol in plain text is mapped to a fixed symbol in cipher text. | Polyalphabetic cipher is any cipher based on *substitution*, using multiple substitution alphabets.|
| Relationship (Plaintext to Ciphertext) |One-to-One | One-to-Many |
| Mapping | Onto a unique alphabetic character of a cipher text | Onto 'm' alphabetic characters of a cipher text |
| Examples are | additive, Caesar-shift cipher and monoalphabetic substitution cipher.| Autokey, Playfair, Vigenere, Hill, one-time pad, etc.|
|||
| Simple? | It is a simple substitution cipher. | It is multiple substitutions cipher. |
| Strength? |  Monoalphabetic ciphers are not that strong as compared to polyalphabetic cipher. | Polyalphabetic ciphers are much stronger. |
|||
| Dependency | A stream cipher is a monoalphabetic cipher if the value of key does not depend on the position of the plain text character in the plain text stream. | A stream cipher is a polyalphabetic cipher if the value of key does depend on the position of the plain text character in the plain text stream. |
|||

Source from [here](https://www.geeksforgeeks.org/difference-between-monoalphabetic-cipher-and-polyalphabetic-cipher/#:~:text=Monoalphabetic%20cipher%20is%20one%20where,substitution%2C%20using%20multiple%20substitution%20alphabets.&text=The%20relationship%20between%20a%20character,is%20one%2Dto%2Done.)
 
List of *Classical Ciphers*:

+ Caesar Cipher
+ Playfair Cipher
+ Hill Cipher
+ Vigenere Cipher (multiple Caesar Ciphers)
+ Autokey Cipher
+ Vernam Cipher
+ One-Time Pad
+ Transposition Ciphers (Permutation Ciphers)
+ Rail Fence Cipher
+ ROW Transposition Ciphers
+ BLOCK / COLUMNAR Transposition Ciphers
+ Product Ciphers

### Monoalphabetic Substitution Cipher
+ Caesar Cipher
+ Playfair Cipher
+ Hill Cipher


#### Caesar Cipher
+ Only have 25 possible ciphers (A maps to B, ..., Z)
+ Could simply try each in turn (brute force search / exhaustive key search)
+ Encryption:
	+ *C* = E<sub>k</sub>(*P*) = *P* + *k* (mod 26)

+ Decryption:
	+ *P* = D<sub>k</sub>(*C*) = *C* + *k* (mod 26)

> `C` stands for Ciphertext, `P` stands for Plaintext, `k` stands for key

#### Playfair Cipher
+ Encrypt multiple letters
+ Security much improved over monoalphabetic
+ Playfair Key Matrix
	+ A `5 x 5`  matrix of letters based on a keyword
	+ Fill in letters of keyword (minus duplicates)
	+ Fill rest of matrix with other letters
	+ E.g. using the keyword MONARCHY

| | | | | |
|---|---|---|---|---|
| **M** | **O** | **N** | **A** | **R** |
| **C** | **H** | **Y** | B | D |
| E | F | G | I/J | K |
| L | P | Q | S | T |
| U | V | W | X | Z |
|||
> Playfair Key Matrix (5 x 5)


### Polyalphabetic Substitution Cipher
+ Vigenère Cipher
+ Autokey Cipher
+ Vernam Cipher
+ One-Time Pad

#### The Vigenère Tableu

![Image.](https://pages.mtu.edu/~shene/NSF-4/Tutorial/VIG/FIG-VIG-Table.jpg)

### Transposition Cipher
+ Considers as classical transposition or permutation ciphers.
+ Hide the plaintext by rearranging the letter order, without having to alter the actual letters used

#### Examples of Transposition Cipher (Permutation)
+ Geometric Figure
+ Rail Fence Cipher
+ ROW Transposition Cipher
+ BLOCK /COLUMNAR Transposition Cipher