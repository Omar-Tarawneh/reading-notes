# Read-13, Code 401, 12 April 2021

## Review and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?
   This mean that the connection is directly between the client and the server use TCP no HTTP. Bcause you don't need to handle every request from client you just use events

2. What happens when a client emits an event?
   The server take that emit message and the paylod and resopond with and action or another emit message.

3. What happens when a server emits an event?
   The client take this emit and respond to it with an action or another emit messages.

4. What happens if a client “misses” an event?
   nothing actually that mean the event never been triggered the app will still functions the right way.

5. How can we mitigate this??
   you can avoid missing events by having a handler for each event that take an action.

6. Does socket.io use HTTP? Why?
   No, it use a TCP connection. Because the TCP allow for direct connection between the client and the server on the other hand HTTP deal with request and resoponse which will not useful for events.

## Vocabulary

- Socket: is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

- Websocket: WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

- Client: A Web client typically refers to the Web browser in the user's machine or mobile device.

- Server: It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users

- OSI Model: The Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network.

- TCP/IP: stands for Transmission Control Protocol/ Internet Protocol. It is specifically designed as a model to offer highly reliable and end-to-end byte stream over an unreliable internetwork..

- TCP: Transmission Control Protocol (TCP) is a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.

- UDP: User Datagram Protocol (UDP) – a communications protocol that facilitates the exchange of messages between computing devices in a network. It's an alternative to the transmission control protocol (TCP).

- Packet: is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred.

## Preview

1. Queue with Stacks, socket io, websocket.
2. React, more about socket io.
3. The socket io with our project this week.

## Socket io Cheatsheet

### Server-side

```javascript
io.on('connection', (socket) => {
  // basic emit
  socket.emit(/* ... */);

  // to all clients in the current namespace except the sender
  socket.broadcast.emit(/* ... */);

  // to all clients in room1 except the sender
  socket.to('room1').emit(/* ... */);

  // to all clients in room1 and/or room2 except the sender
  socket.to('room1').to('room2').emit(/* ... */);

  // to all clients in room1
  io.in('room1').emit(/* ... */);

  // to all clients in namespace "myNamespace"
  io.of('myNamespace').emit(/* ... */);

  // to all clients in room1 in namespace "myNamespace"
  io.of('myNamespace').to('room1').emit(/* ... */);

  // to individual socketid (private message)
  io.to(socketId).emit(/* ... */);

  // to all clients on this node (when using multiple nodes)
  io.local.emit(/* ... */);

  // to all connected clients
  io.emit(/* ... */);

  // WARNING: `socket.to(socket.id).emit()` will NOT work, as it will send to everyone in the room
  // named `socket.id` but the sender. Please use the classic `socket.emit()` instead.

  // with acknowledgement
  socket.emit('question', (answer) => {
    // ...
  });

  // without compression
  socket.compress(false).emit(/* ... */);

  // a message that might be dropped if the low-level transport is not writable
  socket.volatile.emit(/* ... */);
});
```

### Client-side

```javascript
// basic emit
socket.emit(/* ... */);

// with acknowledgement
socket.emit('question', (answer) => {
  // ...
});

// without compression
socket.compress(false).emit(/* ... */);

// a message that might be dropped if the low-level transport is not writable
socket.volatile.emit(/* ... */);
```

### Reversed Events

- connect
- connect_error
- disconnect
- disconnecting
- newListener
- removeListener

## Rooms and namespaces

Rooms are part of namespaces where each namespace can be divided into several rooms and a very room handles a certain type of sockets (Join & Leave) it basically works by a socket (user) sends a join request to one of the available rooms and the server joins it in the room (it could need authentication or invitation depending on your application).

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-13)
