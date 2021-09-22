---
layout: default
course_number: CS330
title: "Programming Lab - Introduction to Sockets"
---

# Programming Lab - Introduction to Socket   

### Download and compile _individually_ the following files:
  - [tcp_client.c](files/tcp_client.java)
  - [udp_client.c](files/udp_client.java)
  - [tcp_server.c](files/tcp_server.java)
  - [udp_server.c](files/udp_server.java)

### We use the following simple client/server applications do demonstrate UDP and TCP socket programming.
  - A client reads a line from its standard input and sends the line out its socket to the server.
  - The server reads a line from its socket.
  - The server converts the line to uppercase.
  - The server sends the modified line out its socket to the client.
  - The client reads the modified line through its socket and prints the line on its standard output.

###  Run the applications and answer the following questions:
  - Suppose you run tcp_client before you run tcp_server.
    - What happens?
    - Why?
  - Suppose you run udp_client before you run udp_server.
    - What happens?
    - Why?
  - What happens if you use different port numbers for the UDP client and UDP server sides?
  - What happens if you use different port numbers for the TCP client and TCP server sides?
  - Run udp_server and udp_client – send a message. Run udp_client again (while udp_server is still running), but this time with a shorter message.
    - What happens?
    - Why?
    - Extra Credit: Can if you fix it?    
  - Update tcp_client, udp_client, tcp_server and udp_server to accept the **client and server** port numbers as a _user_ input.
  - Change the _receiveData_ in udp_client to allocate 1 byte instead of 1024. Run the udp_client and the udp_server – send a message with length more than 1.
    - What happens?
    - Why?
  - Change the allocation size of _sendData_ in udp_client to 1 and rerun the client.
    - What do you expect will happen?
    - What happens?  
    - Why?
    - Is this a bug?
 - _Extra Credit_ Experiment with the code, surprise me.
    - Do not be afraid to explore and brake it. Learn form it.  

### References
  - [Linux socket interface](https://linux.die.net/man/7/socket)
  - [Beej's Guide to Network Programming](https://beej.us/guide/bgnet/html/#structs)

### Testing
  - [Netcat](http://netcat.sourceforge.net/) is a command line tool that connects to an arbitrary TCP or UDP port and allows you to send and receive data.

### Grading
Post your report including source in [Marmoset](https://cs.ycp.edu/marmoset) by the scheduled due date in the syllabus.
