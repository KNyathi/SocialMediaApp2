# BACKEND

## Endpoints
### Posts
- http://localhost:5000/api/posts/create (create a post) [POST]
- http://localhost:5000/api/posts/:id (delete a post) [DELETE]
- http://localhost:5000/api/posts/:id (get a post) [GET]
- http://localhost:5000/api/posts/feed (get the feed) [GET]
- http://localhost:5000/api/posts/like/:id (like a post) [POST]
- http://localhost:5000/api/posts/reply/:id (reply to a post) [POST]
  
### Users
- http://localhost:5000/api/users/signup (create an account) [POST]
- http://localhost:5000/api/users/login (log in to your account) [POST]
- http://localhost:5000/api/users/logout (log out of your account) [POST]
- http://localhost:5000/api/users/follow (follow user) [POST]
- http://localhost:5000/api/users/update/:id (updating a user) [POST]
- http://localhost:5000/api/users/profile/:id (get a profile) [GET]

### Dependencies
- Express (web framework for nodejs)
- jsonwebtoken (JWT)
- mongoose (work with MongoDB)
- bycryptjs (hashing passwords when stored in database)
- dotenv (hide environmental keys)
- cookie-parser (parses cookies attached to client's request)

### Status
#### 1) 5xx Server Error:
- 500 Internal Server Error: A generic error message indicating a problem with the server.
- 503 Service Unavailable: The server is currently unavailable (e.g., due to maintenance or overload).
- 504 Gateway Timeout: The server, while acting as a gateway or proxy, did not receive a timely response from the upstream server it accessed in attempting to complete the request.
2) 4xx Client Error:
- 400 Bad Request: The server cannot process the request due to a client error (e.g., malformed request syntax).
- 401 Unauthorized: The request requires user authentication.
- 403 Forbidden: The server understood the request, but it refuses to authorize it.
- 404 Not Found: The server cannot find the requested resource.
3) 3xx Redirection:
- 301 Moved Permanently: The requested resource has been permanently moved to a new location.
- 304 Not Modified: The client's cached copy is up-to-date, so the server responds without sending the requested content.
4) 2xx Success:
- 200 OK: The request has succeeded.
- 201 Created: The request has been fulfilled, and a new resource is created.
- 204 No Content: The server successfully processed the request but does not need to return an entity-body.
5) 1xx Informational:
- 100 Continue: The server has received the request headers and the client should proceed to send the request body.
- 101 Switching Protocols: The server is changing protocols, such as switching to WebSocket.
