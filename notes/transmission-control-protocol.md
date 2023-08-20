# Transmission Control Protocol / Internent Protocol (TCP/IP)

## Transmission Control Protocol (TCP)

### Basics
> The **Transmission Control Protocol** is one of the main protocols in the **Internet protocol suite**. It is the successor of the **Internet Protocol**, so it's commonly referred as **TCP/IP**. The World Wide Web, file transfer, email and remote administration all use TCP. TCP provides a reliable and error-checked delivery of a stream of octects (8 bytes). **TLS** often runs on top of TCP.

### TCP Layers
> The **TCP/IP Model** has 4 layers:
>+ **Application Layer**
>+ **Transport Layer**
>+ **Internet Layer**
>+ **Network Interface Layer**
> Each layer has its own protocols and functions to make TCP/IP work.
>+ **Application Layer**: This is the highest layer, and interacts with the application program. This layer allows users to interact with software applications. This layer interacts with applications by creating a communication component. Examples of the application layer in applications is file transfer, email, remote login, etc.
>+ **Transport Layer**: This layer builds on the network layer to allow data transfer from a source machine to a destination machine. This layer determines how much data will be sent at what rate and where. This layer adds to the messages received from the application layer to ensure they're sent error-free and in sequence.
>+ **Internet Layer**: This layers function is to send packets from a source network or computer and ensure they reach the destination computer or network irrespective of their route. This layer offers the functionality of transferring packets from one node to another with the help of various networks (internetworking).
>+ **Network Interface Layer**: This is the lowest and final layer on the TCP/IP Model. This layer is responsible for the transmission of data between two computers on the same network. This layer helps to define details as to how data should be sent using the network. It also defines how the data should be sent physically through the network.

### Handshake
> Before creating a connection to a server, the server must be first listening for connections on an open port. This is called **passive open**. Once the server is passive open, a client can initiate a 3-step **handshake** to connect to the server. The handshakes goes as follows:
>+ **SYN**: The client sends a SYN, or synchronize, packet to the server. Client sets the packets segment of numbers to a random value A.
>+ **SYN-ACK**: The server sends back SYN-ACK, or an acknowledgement packet, telling the client the SYN packet was received. The server sets the ACK packets segment of numbers to A+1 and sends the SYN packets segment of numbers as random value B.
>+ **ACK**: The client sends back an ACK packet with the packets segment of numbers as B+1.
