# Implementaion-Of-SNMP-Manager
Although some RS­232 connectors still cling desperately to audio hardware products around the world, for years Ethernet and the Internet Protocol (IP) have been replacing older serial communication formats as the connection of choice for monitoring and controlling audio as well as video, networking, and industrial equipment. Since the childhood of computer networking, network designers envisioned a world where a person’s audio system, video system, HVAC system, and toaster all connect to the same network. To that end, computer scientists developed a protocol capable of managing any network device. The result was SNMP, which stands for Simple Network Management Protocol. SNMP was introduced in 1988 and now includes three distinct versions SNMPv1, SNMPv2, and SNMPv3. Due to the maturity of SNMP, many device manufacturers include support for this protocol in their products, and many SNMP management solutions exist off­the­shelf for common operating systems and programming languages. However, SNMP man­ agement capabilities are still lacking for today’s control system platforms, requiring control system programmers to write their own SNMP management code.
Of course, writing an SNMP manager should be simple, right? After all, it is the Simple Network Management Protocol. Unfortunately, “Simple” means “easy for computer scientists who spend eight hours a day thinking about designing network protocols.” When making the leap from constructing text strings to constructing SNMP messages, the word “Simple” is a cruel joke that leaves control system programmers shouting “Just tell me the bytes to send!”
In answer to that plea, this RaneNote provides a technical overview of SNMPv1, along with the terminology necessary to understand the SNMP message, describe the message format, and show exactly (byte­ by­byte) how to construct the SNMP message.

Types of Server
There are two types of servers you can have −
Iterative Server − This is the simplest form of server where a server process serves one client and after completing the first request, it takes request from another client. Meanwhile, another client keeps waiting.
Concurrent Servers − This type of server runs multiple concurrent processes to serve many requests at a time because one process may take longer and another client cannot wait for so long. The simplest way to write a concurrent server under Unix is to fork a child process to handle each client separately.

How to Make Client
The system calls for establishing a connection are somewhat different for the client and the server, but both involve the basic construct of a socket. Both the processes establish their own sockets.
The steps involved in establishing a socket on the client side are as follows −
Create a socket with the socket() system call.
Connect the socket to the address of the server using the connect() system call.
Send and receive data. There are a number of ways to do this, but the simplest way is to use the read() and write() system calls.


The complete document can be found in the below mentioned google drive link 
https://drive.google.com/file/d/1gWBfzbvtal9Mp_Y8LAWFtfhBzh3qKJxY/view?usp=sharing
