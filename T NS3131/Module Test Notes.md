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

	> such as a username / password combination, a secret key, or perhaps bio metric data (fingerprints, for example) -- that serves as unambiguous identification credentials.

	+ The AAA server compares the user-supplied authentication data with the user-associated data stored in its database, and if the credentials match, the user is granted with the network access.

+ Authorization

	+ defines what rights and services that the end user is allowed to have once network access is granted.

	+ this might include providing an IP address, invoking a filter to determine which applications or protocols are supported, and so on.

	+ Authentication and authorization are usually performed together in an AAA-managed environment.

+ Accounting

	+ provides the methodology for collecting information about the end user's resource consumption, which can then be processed for billing, auditing, and capacity-planning purposes.

### AAA Processing

- End user connects to the point-of-entry device and requests access to the network.
- NAS (Network Access Server) AAA client function collects and forwards the end user's credentials to the AAA server.
- AAA server processes the data and returns an accept or reject response and other relevant data to the AA client.
- AAA client on the NAS (Network Access Server) notifies the end user that access is granted or denied for the specified resources.

![AAA Framework](https://download.huawei.com/mdl/image/download?uuid=73578bb25fee4af69890b3c4d9af2b89)

> AAA Framework shown by [Huawei](https://info.support.huawei.com/info-finder/encyclopedia/en/AAA.html)

As shown in the preceding figure, the basic AAA implementation process is as follows:

-  The user established a connection with the `AAA client` before accessing the `network`.

- The `AAA client` sends the user's authentication credential to the `AAA server`.

- The `AAA server` authenticates and authorizes the user based on the user's authentication credentials and returns the authentication and authorization results to the `AAA client`.

- The `AAA client` determines whether to allow the user to access the network based on the received authentication and authorization results.

In the **AAA framework**:

- The `AAA client` runs on a `network access server (NAS)` , which can be a router or switch that provides network access services for `users`.

- The `AAA server` is responsible for `user authentication`, `authorization`, and `accounting`, as well as **centralized user information management**. Depending on the communication protocols used in `AAA`, `AAA servers` are classified into `Remote Authentication Dial-in Service (RADIUS)` server and `Terminal Access Controller Access Control System (TACACS)` server.


![Overview of AAA and User Management](https://download.huawei.com/mdl/image/download?uuid=672a9a06fb9c419eb02f1ce483be90fb)

> Overview of AAA and User Management illustrated by [Huawei](https://info.support.huawei.com/info-finder/encyclopedia/en/AAA.html)

---

### RADIUS (REMOTE ACCESS DIAL-In USER SERVICE)

- Best-known and most widely deployed AAA protocol

- Developed in the mid-1990s by `Livingston Enterprises` (since acquired by Lucent) to provide `authentication` and `accounting` services to their `NAS (Network Access Server)` devices.

- RFC 2138, RFC 2139, RFC 2865, 2866 and 2869

![RADIUS Process ](https://github.com/ngzhekai/obsidian-note-sync/blob/main/T%20NS3131/img/moduleTest-radius-diagram.png?raw=true)

#### The process used in centralized authentication:

1. The remote access server (Network Access Server) queries the users for credentials.

2.  The client sends its authentication information.

3. The remote access server (NAS) forwards the authentication information to a central authentication server (AAA Server).

4. The central authentication server (AAA Server) checks the user's credentials against a user account database, such as the `Active Directory` directory service, `Novell NetWare eDirectory`, or `UNIX NIS`.

5. The authentication server returns the success or failure of the authentication to the remote access server (NAS).

6. If the authentication succeeded, the remote access server (NAS) allows the client to access the network.