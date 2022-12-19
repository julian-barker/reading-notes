[Home](../README.md)

# Class 13

## Message Queues

### Socket.io Chat Example

- The chat example serves an html page to the client and uses inline scripts to listen for the submission of the form input element.
- proof of life on the backend is achieved by calling `io.on()` on the frontend and logging to the backend console on connect and disconnect
- to send to everyone but the sender, use the broadcast flag by calling `socket.broadcast.emit`

### Rooms

- rooms are used to broadcast event to asubest of clients on a socket or namespace
- you join a room with `socket.join(roomname)`
- leave a room with `socket.leave(roomname)`

### Namespaces

- namespaces also compartmentalize data flow across a socket.
- they have their own handlers, rooms, and middlewares
- these can be restricted to certain users and implement different logic for those users
