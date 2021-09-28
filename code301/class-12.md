# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 301

# Read: 12 - CRUD

## Reading

### [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
1. Descripe the data:

* 100’s = Tells client that header part of request has been received and server will try to transmit demand of the client.
* 200’s = Tells client that its request was accepted.
* 300’s = Tells client that the resource they are requesting isn’t available in tht location anymore.
* 400’s = Invalid requests a client sent to a server.
* 500’s = Problems with overwhelmed servers or unreachable.

2. A status code 202 code tells the client that the request was valid, but is process.
3. A status code 308 code is a permanent redirect. 
4. If an update didn't return to a client, send code 404.
5. If resource no longer exists, send code 410.
6. The 'Forbidden' status code is code 403.

### [Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)
