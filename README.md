# HTTP Status Codes Cheat Sheet

This repository provides a quick reference for HTTP status codes as defined in the HTTP/1.1 specification. HTTP status codes are divided into five categories: 1xx for informational, 2xx for success, 3xx for redirection, 4xx for client errors, and 5xx for server errors.

Each status code represents a specific meaning in the HTTP protocol. Clients (like web browsers) and servers communicate with each other using these status codes as part of the HTTP response.

Please note that this cheat sheet does not cover all possible status codes defined by various HTTP extensions and APIs, but it includes the most common ones that you're likely to encounter.

For a more detailed and comprehensive list of HTTP status codes, please refer to the HTTP/1.1 specification or consult online resources like the Mozilla Developer Network.

## 1xx - Informational

### 100 Continue: 
The server has received the request headers and the client should proceed to send the request body.
### 101 Switching Protocols: 
The requester has asked the server to switch protocols and the server has agreed to do so.
### 102 Processing (WebDAV): 
A WebDAV request may contain many sub-requests, and this status code indicates that the server is processing the request.

## 2xx - Success

### 200 OK:
The request was successful, and the response body depends on the request method.
### 201 Created:
The request was successful and a new resource was created as a result.
### 202 Accepted:
The request has been accepted for processing, but the processing has not been completed.
### 204 No Content:
The server successfully processed the request, but is not returning any content.

## 3xx - Redirection

### 300 Multiple Choices:
There are multiple options that the client may follow.
### 301 Moved Permanently:
The URL of the requested resource has been changed permanently.
### 302 Found (Previously "Moved Temporarily"):
The server is currently responding to the request with a page from a different location, but the requester should continue to use the original location for future requests.
### 304 Not Modified:
The resource has not been modified since the last request.

## 4xx - Client errors

### 400 Bad Request: 
The server could not understand the request due to invalid syntax.
### 401 Unauthorized:
The request lacks valid authentication credentials for the target resource.
### 403 Forbidden:
The server understood the request, but refuses to authorize it.
### 404 Not Found:
The requested resource could not be found on the server.
### 405 Method Not Allowed:
The method specified in the request is not allowed for the resource.
### 422 Unprocessable Content
Used when the server understands the content type of the request, and the syntax of the request is correct, but the server is unable to process the contained instructions.

## 5xx - Server errors

### 500 Internal Server Error:
The server encountered an unexpected condition that prevented it from fulfilling the request.
### 501 Not Implemented:
The server does not support the functionality required to fulfill the request.
### 502 Bad Gateway:
The server, while acting as a gateway or proxy, received an invalid response from an inbound server it accessed while attempting to fulfill the request.
### 503 Service Unavailable:
The server is currently unable to handle the request due to a temporary overloading or maintenance of the server.
