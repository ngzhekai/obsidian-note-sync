### Overview of Cryptography

#### Two type of operation used for transforming plain text to cipher text

+ Substitution 

> replacing the letter with another letter

+ Transposition 

 > changing the sequence of the letter, while the frequency of the letter appearance is still the same
 
#### Type of key used in cryptography

1. Symmetric

> Sender and Receiver shares the same key (refer private-key encryption

2. Asymmetric 

> Sender and Receiver uses two different keys to do the encryption and decryption (refer public-key encryption)

#### Two ways which the plain text is processed

1. Block cipher

2. Stream cipher

### Five ingredients of the encryption scheme

1. Plain text
2. Encryption algorithm
3. Secret Key
4. Cipher text
5. Decryption algorithm

---

### Public-Key uses can be classify into these 3 categories:

1. Encryption/decryption (provide secrecy)
2. Digital signatures (provide authentication)
3. Key exchange (of session keys)

### Different ways of distributing public keys

1. Public announcement
2. Public available directory
3. Public-key authority
4. Public-key certificates

---

### AAA (Authentication, Authorization and Accounting)

+ Authentication
	+ involves validating the end users' identity prior to permitting them network access.
	+ this process key on the notion that the end-user possesses a unique piece of information

	> a username / password combination, a secret key, or perhaps bio metric data (fingerprints, for example) -- that serves as unambiguous identification credentials.

	+ The AAA server compares the user-supplied authentication data with the user-associated data stored in its database, and if the credentials match, the user is granted with the network access.
+ Authorization
	+ defines what rights and services that the end user is allowed to have once network access is granted.
+ Accounting
	+ provides the methodology for collecting information about the end user's resource consumption, which can then be processed for billing, auditing, and capacity-planning purposes.