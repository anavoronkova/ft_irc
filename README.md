# ft_irc

## Internet Relay Chat

### Summary
**ft_irc** is a project aimed at creating a custom IRC server in C++ 98. The server allows multiple clients to connect and communicate using a text-based protocol similar to traditional IRC. This project provides an opportunity to learn about network programming, sockets, and handling concurrent connections.

### Introduction
**ft_irc** is an implementation of an IRC server following the traditional IRC protocol. Users can connect to the server using an existing IRC client, join channels, send messages, and communicate in real-time. The server handles user connections, messages, and channel operations, enabling a complete IRC experience.

### Installation
1. Clone the repository:
   ```
   git clone <repository_url>
   ```
2. Navigate to the project directory:
   ```
   cd ft_irc
   ```
3. Compile the project:
   ```
   make
   ```

### Usage
Run the server with:
```
./ircserv <port> <password>
```
- `<port>`: The port number the server will listen on.
- `<password>`: The password required for clients to connect.

### Features
- **Multi-Client Handling**: Supports multiple clients simultaneously.
- **IRC Commands**: Implements basic IRC commands:
  - **NICK**: Set user nickname.
  - **USER**: Set user details.
  - **JOIN**: Join a channel.
  - **PART**: Leave a channel.
  - **PRIVMSG**: Send private messages to users or channels.
  - **OPER**: Operator privileges.
  - **KICK, INVITE, TOPIC, MODE**: Channel operator commands.
- **Non-Blocking I/O**: Uses `poll()` (or equivalent) for non-blocking input/output.
- **TCP/IP Communication**: All client-server communication is done via TCP/IP.

