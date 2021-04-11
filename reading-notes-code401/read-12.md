# Read-12, Code 401, 11 April 2021

## Review and Discussion

1. What is the benefit of transforming data into packets?

   Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully.

2. UDP is often refereed to as a connectionless protocol. Why is this?

   because No connection needs to be established between the source and destination before you transmit data.

3. Can a socket server application have multiple socket connections?

   A socket that has been established as a server can accept connection requests from multiple clients

4. Can a socket connection application be connected to multiple socket servers?

   If your program is a client to multiple servers, use one socket per server.

5. Can an application be both a socket server and a socket connection?

   Yes! You can do that if you're willing to use two different ports.

## Vocabulary Terms

- Observer Pattern: Observer is a behavioral pattern which means that is concerned about communication between objects.

- Listener: EventEmitter is a class that helps us create a publisher-subscriber pattern in NodeJS.

- Event handlers can be used to handle and verify user input, user actions, and browser actions: Things that should be done every time a page loads.

- Event-Driven Programming is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads.

- Event Loop: is a programming construct or design pattern that waits for and dispatches events or messages in a program

- Event Queue is a repository where events from an application are held prior to being processed by a receiving program or system.

- Call Stack: is a stack data structure that stores information about the active subroutines of a computer program.

- Emit/Raise/Trigger: Emit send a message with payload, that trigger a response and raise the events.

- Subscribe: waiting for the events to take a place in the event loop cycle.

- A Database: is a data structure that stores organized information.

## Preview

1. Stack & Queue, Events in node.js, Socket io
2. React, more about Socket io, connecting two server with socket io.
3. TCP, in-message queue.

### OSI model

Open Systems Interconnection model, describes seven layers that computer systems use to communicate over a network.
OSI layers: - Application - Presentation - Session, - Transport - Netwrok - Data Link - Physical

![layers](https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/02/OSI-7-layers.jpg)

### TCP Three-Way handshake

TCP is a reliable and connection-oriented transport protocol. with this data can delivered successfully and accurately.

- Connection step three-way handshake
  - syn: Client sends a SYN segment to the server, asking for synchronization "simply, server please open the connectin for me". the server reply with...
  - SYN-ACK: synchronization and acknowledgement now you are connected.
  - Then two way connection established.

![tcp](https://media.geeksforgeeks.org/wp-content/uploads/TCP-connection-1.png)

### Socket io

[Tutorial](https://www.tutorialspoint.com/socket.io/)

Socket IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket IO is built on top of the WebSockets API (Client side) and Node.js.

#### Socket io vs WebSocket

![Sokect](https://cdn.educba.com/academy/wp-content/uploads/2018/11/WebSockets-vs-Socket-1.jpg.webp)

[GitHub-Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-12)
