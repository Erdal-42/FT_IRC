# FT_IRC

In this module I had to demonstrate message relays using network sockets. 

# TASKS

---

You have to develop an IRC server in C or C++ 98. You mustn’t develop a client. You mustn’t handle server-to-server communication. Your executable will be run as follows:
```
./ircserv <port> <password>
```
```
• port: The port number on which your IRC server will be listening to for incoming
IRC connections.
• password: The connection password. It will be needed by any IRC client that tries
to connect to your server.
```

Requirements
```
• The server must be capable of handling multiple clients at the same time and never
hang.
• Forking is not allowed. All I/O operations must be non-blocking.
• Only 1 poll() (or equivalent) can be used for handling all these operations (read,
write, but also listen, and so forth).
• Several IRC clients exist. You have to choose one of them as a reference. 
• Your reference client must be able to connect to your server without encountering
any error.
• Communication between client and server has to be done via TCP/IP (v4 or v6).
• Using your reference client with your server must be similar to using it with any
official IRC server. However, you only have to implement the following features:
	◦ You must be able to authenticate, set a nickname, a username, join a channel,
	send and receive private messages using your reference client.
	◦ All the messages sent from one client to a channel have to be forwarded to
	every other client that joined the channel.
	◦ You must have operators and regular users.
	◦ Then, you have to implement the commands that are specific to operators.

```
---
