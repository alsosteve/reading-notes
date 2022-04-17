# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 13 - Message Queues

## What does it mean that web sockets are bidirectional? Why is this useful?
This means that the information flows in both directions from the client and the server. It is useful because it is faster and doesn't require a client to submit new requests.

## Does socket.io use HTTP? Why?
Yes, this is required for the initial connection.

## What happens when a client emits an event?
The server reacts to the event.

## What happens when a server emits an event?
All clients react to the event.

## What happens if a client “misses” an event?
Probably nothing because the data just goes missing.

## How can we mitigate this?


## Vocab:

Socket: a software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network

Web Socket: a computer communications protocol, providing full-duplex communication channels over a single TCP connection

Socket.io: node.js realtime framework server

Client: a desktop computer or workstation that is capable of obtaining information and applications from a server

Server: a piece of computer hardware or software (computer program) that provides functionality for other programs or devices

OSI Model: The Open Systems Interconnection model (OSI model) is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology

TCP Model: The TCP/IP model consists of five layers: the application layer, transport layer, network layer, data link layer and physical layer.

TCP: Transmission Control Protocol

UDP: a communications protocol that is primarily used to establish low-latency and loss-tolerating connections between applications on the internet

Packets: a small segment of a larger message. Data sent over computer networks, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them
