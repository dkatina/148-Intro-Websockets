## Learning Objectives

- The students should be able to analyze the advantages of WebSockets over traditional HTTP communication, including reduced latency and more efficient data transfer.
- The students should be able to understand how WebSocket works and its protocols to establish communication channels between a client and a server.
- The students should be able to identify and describe real-world use cases for WebSockets, such as chat applications, online gaming, and collaborative editing tools.

## **Understanding What WebSockets Are and How They Work**

Unlike traditional HTTP, which uses a request-response model, WebSockets allow for asynchronous communication between a client and a server.

### How WebSockets Work

1. **Handshake**: The client sends an HTTP request to the server, requesting to upgrade the connection to a WebSocket connection. The server responds with an HTTP 101 status code, indicating that the upgrade was successful.
2. **Connection Establishment**: Once the connection is established, both the client and the server can send messages to each other at any time. This enables real-time communication without the need for polling or continuous HTTP requests.

## **Comparing WebSockets with Traditional HTTP**

1. **Latency**: WebSockets use a long-lived TCP (Transmission Control Protocol) connection, which reduces the latency of establishing and tearing down connections for each message.
2. **Efficient Data Transfer**: WebSockets use a binary protocol, which allows for more efficient data transfer compared to text-based protocols like HTTP.
3. **Real-Time Communication**: WebSockets support full-duplex communication, which means that both the client and the server can send and receive messages simultaneously versus traditional HTTP, where a client sends a request to the server, and the server responds with a single response.

## WebSocket Protocol Basics

### Handshake

Think of the WebSocket handshake as the initial greeting between two people. When a client wants to establish a WebSocket connection with a server, it sends an HTTP request with specific headers, indicating its intent to upgrade the connection to a WebSocket connection. The server then responds with an HTTP 101 status code, indicating that the upgrade was successful.

### Persistent Connections

A persistent connection is like a long-lasting conversation. Once the WebSocket connection is established, both the client and the server can send and receive messages at any time without the need for continuous polling. This allows for efficient and low-latency communication between the client and the server.

### **WebSocket Frames**

WebSocket frames are like individual messages in a conversation. They are the basic unit of communication in the WebSocket protocol and consist of an `opcode`, `payload length`, and `payload data`.

1. **Opcode**: The opcode specifies the type of message being sent, such as text, binary, or control messages like ping and pong.
2. **Payload Length**: The payload length specifies the length of the payload data in bytes.
3. **Payload Data**: The payload data contains the actual message being sent.

WebSocket frames allow for efficient data transfer and support full-duplex communication, which means that both the client and the server can send and receive messages simultaneously.