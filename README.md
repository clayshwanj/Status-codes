# Highlights on the response.writeHead method

# Sets the status code and headers for the HTTP response.

# The numbers in the writeHead method refer to HTTP status codes, which indicate the result of the HTTP request..

# Syntax:

response.writeHead(statusCode, { headers });

1. statusCode:
   This is a numerical value representing the HTTP status code.
   Status codes are standardized codes that describe the outcome of the HTTP request.

2. headers:

This is an object where the keys are header names and the values are header values.
HTTP headers provide additional information about the response.

# Common HTTP Status Codes

# 1xx: Informational

1. 100 Continue: The server has received the request headers and the client should proceed to send the request body.
2. 101 Switching Protocols: The requester has asked the server to switch protocols, and the server has agreed to do so.

# 2xx: Success

3. 200 OK: The request has succeeded.
4. 201 Created: The request has been fulfilled, resulting in the creation of a new resource.
5. 204 No Content: The server successfully processed the request, but is not returning any content.

# 3xx: Redirection

6. 301 Moved Permanently: The requested resource has been permanently moved to a new URL.
7. 302 Found: The requested resource has been temporarily moved to a different URL.
8. 304 Not Modified: The resource has not been modified since the last request.

# 4xx: Client Errors

9. 400 Bad Request: The server cannot or will not process the request due to a client error (e.g., malformed request syntax).
10. 401 Unauthorized: Authentication is required and has failed or has not yet been provided.
11. 403 Forbidden: The server understands the request, but refuses to authorize it.
12. 404 Not Found: The requested resource could not be found.

# 5xx: Server Errors

13. 500 Internal Server Error: The server encountered an unexpected condition that prevented it from fulfilling the request.
14. 502 Bad Gateway: The server received an invalid response from the upstream server.
15. 503 Service Unavailable: The server is not ready to handle the request, often due to being overloaded or down for maintenance.
