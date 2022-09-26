## TCP/IP ARCHITECTURE
![Difference Between OSI and TCP/IP  Layers](./img/TTP3121-Lec1-TCP&IP-Architecture1.jpg)

|    | TCP/IP Layers                | OSI Model Layers (Equivalent to) |
| -- | :-----                       | :-----                           |
| 1. | Application Layer            | Application Layer                |
|    |                              | Presentation Layer               |
|    |                              | Session Layer                    |
|    |                              |                                  |
| 2. | Host-to-Host Transport Layer | Transport Layer                  |
|    |                              |                                  |
| 3. | Internet Layer               | Network Layer                    |
|    |                              |                                  |
| 4. | Network Interface Layer      | Data-Link Layer                  |
|    |                              | Physical Layer                   | 

---

![TCP/IP Layer](./img/TTP3121-Lec1-TCP&IP-Architecture.png)

---

## TCP (Transmission Control Protocol)
>1.  **Connection Oriented** transport protocol. Includes features such as **acknowledgements**, **timeouts**, **re-transmissions**, **end-to-end flow control**, etc.
>
>2. **TCP** is a guaranteed method of transferring data (aka packets), where no data loss will be tolerated, the 3-Way Handshake mechanism take action between the Client and the Server.
>
>3.  **TCP** and **IP** are used together so often, in short the responsibility of IP protocol was to make sure that the packet reaches the right destination, and while the TCP protocol make sure that packets (or data) are not lost when transferring from the sender to the receiver.


## UDP (User Datagram Protocol)
>1. **Connection-less** transport protocol. **UDP** lack all TCP features (acknowledgement, timeouts, re-transmissions, end-to-end flow control, etc) therefore it does not guarantee packet delivery.
>
>2. **UDP** is a method of transferring data which allows partially of the data to be lost, for example,  Live Stream on YouTube


---


