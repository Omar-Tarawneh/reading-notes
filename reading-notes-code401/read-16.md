# Read-16, Code 401, 18 April 2021

## AWS: Cloud Servers

### Discussion

1. What’s the difference between a FIFO and a standard queue?

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers

2. How can the server be assured a message was properly received?
   The most common approach is to use a hash function that combines all the bytes in the message with a secret key and produces a message digest that is difficult to reverse.

3. What classic design pattern is best represented by event driven programming?
   The observer pattern

4. How do you test an event driven system?
   There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application.

### Vocabulary

- Server: A server is a computer that serves information to other computers. These computers, called clients, can connect to a server through either a local area network or a wide area network, such as the internet. A server is a vital piece of your IT infrastructure

- Pub/Sub: is an asynchronous messaging service that decouples services that produce events from services

- WRRC: The request/response cycle traces how a user's request flows through the app. Understanding the request/response cycle is helpful to figure out which files to edit when developing an app (and where to look when things aren't working).

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   AWS, Socket io, Canvas in Html5

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   AWS, React framwork

3. What are you most excited about trying to implement or see how it works?
   I'm really excited to implement React and start using it.

- Virtual Machines

  A virtual machine (VM) is a virtual environment that functions as a virtual computer system with its own CPU, memory, network interface, and storage, created on a physical hardware system (located off- or on-premises).

- Amazon EC2
  - is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers
  - Amazon EC2 offers the broadest and deepest compute platform with choice of processor, storage, networking, operating system, and purchase model

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-16)
