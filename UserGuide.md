User Guide for Backend APIs
Introduction
Welcome to the backend APIs documentation for the Capstone project. This guide provides instructions for accessing various endpoints to interact with the backend services.

Base URL
The base URL for accessing the backend APIs is https://capstone-backend-1.onrender.com

Authentication
Authentication is required for certain endpoints. To authenticate, use the provided authentication routes:

Register a New User

Endpoint: POST /auth/register
Create a new user account by providing the required information in the request body.
Login

Endpoint: POST /auth/login
Authenticate and obtain an access token by providing valid credentials in the request body.
User Management
Manage user accounts and interactions using the following endpoints:

Get All Users

Endpoint: GET /users
Retrieve a list of all users.
Get User by ID

Endpoint: GET /users/{user_id}
Retrieve a specific user by their ID.
Update User

Endpoint: PUT /users/{user_id}
Update user information by providing the user ID and new data in the request body.
Delete User

Endpoint: DELETE /users/{user_id}
Delete a user account by providing the user ID.
Follow User

Endpoint: PUT /users/{user_id}/follow
Follow a specific user by their ID.
Unfollow User

Endpoint: PUT /users/{user_id}/unfollow
Unfollow a specific user by their ID.
Post Management
Manage posts and interactions using the following endpoints:

Create Post

Endpoint: POST /posts
Create a new post by providing the post content in the request body.
Get Post by ID

Endpoint: GET /posts/{post_id}
Retrieve a specific post by its ID.
Update Post

Endpoint: PUT /posts/{post_id}
Update a specific post by its ID.
Delete Post

Endpoint: DELETE /posts/{post_id}
Delete a specific post by its ID.
Like Post

Endpoint: PUT /posts/{post_id}/like
Like a specific post by its ID.
Get Timeline Posts

Endpoint: GET /posts/{user_id}/timeline
Retrieve timeline posts for a specific user by their ID.
Add Comment to Post

Endpoint: POST /posts/{post_id}/comment
Add a comment to a specific post by its ID.
File Upload
Upload files using the following endpoint:

Upload File
Endpoint: POST /upload
Upload a file by providing the file in the request body.

Here's an example of a complete URL for checking a specific user's details:

In this example:

**GET https://capstone-backend-1.onrender.com/users/123**

GET is the HTTP method used to retrieve data.
**https://capstone-backend-1.onrender.com** is the base URL of the backend API.
**/users/123** is the endpoint for retrieving the details of the user with ID 123.
Replace 123 with the actual ID of the user you want to retrieve details for. Similarly, you can construct complete URLs for other endpoints by combining the base URL with the specific endpoint paths.




