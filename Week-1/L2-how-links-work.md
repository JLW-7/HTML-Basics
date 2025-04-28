# How Links Work

## Basic Vocab

**Servers**
- Machines that hold shared info
- Always connected to network

**Client**
- Personal machines (laptop, phone)

**Networks**
- LAN (Local Area Network), many clients connected to a shared server
- WAN (Wide Area Network), connects multiple LANs. An example is the internet

## Components of a URL

**Protocols**
- http: hypertext transfer protocol (transfers html code)
- https: same as above except more secure
- ftp: file transfer protocol (transfers not just html but any type of file)
- ensures correct device communication

**Domain Name**
- The server you are connecting to (e.g. google.com, wikipedia.org)
- Mapped to an address, called IP addresses.
- **Domain Name Server (DNS)** looks up IP address based on url typed in
- Different **top-level domains** (e.g. .edu, .com, .org, .gov)

**Document**
- a specific document (e.g. contact.html)
- If none specified then return default document: index.html, which is usually homepage of websites

## Requests and Response

**Request/Response Cycle**
- When url is put in, your computer (the client) requests pages from a server and it responds with corresponding files
- Requires multiple rounds of communication in between

**Requests**
1. Browser looks up domain in DNS
2. DNS returns corresponding IP address
3. Browser sends http request to the server at that address

**Response**
1. Server finds requested files* and sends it back
2. Browser takes it and styles the html code it recieved, often repeating the steps in Requests
3. If requests can't be fulfilled, error messages will be sent back (e.g. 404, 500)

> Note: usually multiple files are sent back, rarely single files
