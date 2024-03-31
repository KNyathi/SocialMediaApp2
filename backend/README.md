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
1) 5xx Server Error:
- 500 Internal Server Error: A generic error message indicating a problem with the server.
- 503 Service Unavailable: The server is currently unavailable (e.g., due to maintenance or overload).
- 504 Gateway Timeout: The server, while acting as a gateway or proxy, did not receive a timely response from the upstream server it accessed in attempting to complete the request.
