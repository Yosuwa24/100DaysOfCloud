

# DDos, SSL & TLS - A Course on Learn Cantrill by Adrian Cantrill



## Cloud Research

**Distributed Denial of Service (DDoS)**

Definition

- Attack designed to overload websites
- Compete against legitimate connections
- Distributed - hard to block individual IPs/Ranges
- often involve large armies of compromised machines (botnets)


Types of DDoS Attack:

Application layer - HTTP flood

Protocol Attack - SYN Flood

Volumetric - DNS Amplification

**SSL and TLS**

Privacy and Data Integrity between client and server

Privacy -  communications are encrypted

Secure Sockect Layer (SSL)

1. Web browser, send a message to web server for connecting a SSL website
2. Web browser request the web server to identify itself
3. Web server will respond it, by sending a copy of its SSL certificate
4. Web browser will authenticate this certificate, send message back to server
5. Web server acknowledge back to browser and encrypted data exchanged between computer and web server

Transport layer security (TLS)

TLS is recent security system

TLS ensures the security and privacy of data

TLS is designed to provide encryption, authentication and data integrity

TLS is formed of two layers:

- Record protocol : this part of the communications can be used with or without encryption
- Handshake protocol : to authenticate each other and to make use of encryption algorithms

Used for : 

- online credit card transactions
- any sensitive information exchanged online
- web based email
- virtual private networks


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1526833387834847232)
