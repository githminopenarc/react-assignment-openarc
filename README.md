
# OpenArc React Assignment API Documentation

This dummy API provides functionalities for user authentication and managing posts. It uses JWT for authentication and cookies to manage session tokens.

**TASK :**
**You should use all endpoints at least once, while the login should be in a route similar to localhost:3000/login, posts at localhost:3000/posts and users at localhost:3000/users.**

**At the end of given time period please submit your project to HR. A Github link is preferred.**


** CORS enabled for http://localhost:3000 and for methods: "GET, POST, PUT, PATCH, DELETE, HEAD, OPTIONS"
## Base URL

[**openarc-react-assignment.cyclic.app**](https://openarc-react-assignment.cyclic.app)




### **Users Route**

### URL: /api/v1/users

Method: GET

Description:Retrieves a list of users (requires authentication).


### URL: /api/v1/users/register

Method: POST

Description: Registers a new user.

Request Body:

```json
{
  "email": "user@example.com",
  "password": "userpassword"
}

```

### URL: /api/v1/users/login

Method: POST

Description: Authenticates a user and returns a JWT token.

Request Body:

```json
{
  "email": "user@example.com",
  "password": "userpassword"
}

```

### URL: /api/v1/users

Method: DELETE

Description:Deletes a user by ID (requires authentication).

Request Body:

```json
{
  "id": "user_id"
}


```

### **Posts Route**


### URL: /api/v1/posts
Method: GET

Description: Retrieves a list of posts.

### URL: /api/v1/posts
Method: POST

Description: Creates a new post (requires authentication).

Request Body:
```json
{
  "title": "Post Title",
  "content": "Post Content"
}

```

### URL: /api/v1/posts
Method: DELETE

Description: Deletes a post by ID (requires authentication).

Request Body:
```json
{
  "id": "post_id"
}
```

### URL: /api/v1/posts
Method: PUT

Description:Updates a post by ID (requires authentication).

Request Body:
```json
{
  "id": "post_id",
  "title": "Updated Title",
  "content": "Updated Content"
}

```