## High-level HTTP
- **the five steps in the HTTP Request Lifecycle**
1. Local Processing: Extract relevant information from the URL, such as protocol, host, port, resource path, and query strings.
2. Resolve an IP: The client resolves the hostname to an IP address through DNS lookup.
3. Establish a TCP Connection: A three-way handshake is initiated to establish a reliable TCP connection between the client and server.
4. Send an HTTP Request: The client sends an HTTP request to the server containing the request line, headers, and optional body.
5. Receive an HTTP Response: The server processes the request, sends an HTTP response back over the TCP connection, including headers and optional body.

- **two things the client needs before it can make an HTTP Request**
1. Know the target IP address. 
2. Establish a TCP connection with the server.

- **four-way handshake and what it does**
The four-way handshake ensures that both the client and server agree to terminate the connection, and it allows any remaining data to be received and acknowledged before the connection is fully closed.
1. The client initiates the termination by sending a FIN (Finish) packet to the server, indicating it has finished sending data.
2. The server acknowledges the client's FIN with an ACK (Acknowledgment) packet, indicating its receipt.
3. The server also sends its own FIN packet to the client, indicating that it has finished sending data.
4. The client responds with an ACK to acknowledge the server's FIN.

- **True or False: When making an HTTP request, you MUST follow any redirect returned by the request**
True. HTTP specifications expect clients to automatically follow redirects for efficient resource location.

- **Built-in Java class can be used to perform an HTTP request**
HttpURLConnection is the built-in Java class for performing HTTP requests.

- **HTTP status codes represent a successful response, A redirect, A client error**
1. Successful Responses (2xx): Indicate success, like 200 OK.
2. Redirect Responses (3xx): Indicate redirection, such as 301 Moved Permanently.
3. Client Error Responses (4xx): Indicate client errors, like 404 Not Found.