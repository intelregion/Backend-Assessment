# Backend-Assessment

Here's a comprehensive and complex coding challenge designed to evaluate an experienced backend developer. The challenge focuses on CRUD functionality and incorporates various aspects such as database design, API creation, authentication, and deployment.

---

## Coding Challenge: Comprehensive Backend Development Task

### Objective:
Create a RESTful API for a simple blog application. The API should handle CRUD operations for posts, comments, and users. Additionally, implement user authentication and authorization, and ensure the application is ready for deployment.

### Requirements:

1. **User Stories:**
   - As a user, I want to register and log in so that I can create, read, update, and delete my posts.
   - As a user, I want to create, read, update, and delete comments on posts.
   - As a user, I want to view posts and comments created by other users.

2. **Entities:**
   - **User**: `id`, `username`, `email`, `password`
   - **Post**: `id`, `title`, `content`, `authorId`, `createdAt`, `updatedAt`
   - **Comment**: `id`, `postId`, `authorId`, `content`, `createdAt`, `updatedAt`

3. **API Endpoints:**

   **User Endpoints:**
   - POST `/api/users/register` - Register a new user
   - POST `/api/users/login` - Authenticate user and return a token
   - GET `/api/users/profile` - Get user profile (Authenticated)

   **Post Endpoints:**
   - GET `/api/posts` - Retrieve all posts (Paginated)
   - GET `/api/posts/:id` - Retrieve a single post by ID
   - POST `/api/posts` - Create a new post (Authenticated)
   - PUT `/api/posts/:id` - Update a post by ID (Authenticated & Author only)
   - DELETE `/api/posts/:id` - Delete a post by ID (Authenticated & Author only)

   **Comment Endpoints:**
   - GET `/api/posts/:postId/comments` - Retrieve all comments for a post (Paginated)
   - POST `/api/posts/:postId/comments` - Create a new comment on a post (Authenticated)
   - PUT `/api/comments/:id` - Update a comment by ID (Authenticated & Author only)
   - DELETE `/api/comments/:id` - Delete a comment by ID (Authenticated & Author only)

4. **Authentication & Authorization:**
   - Use JWT for user authentication.
   - Protect routes that require authentication.
   - Ensure users can only update or delete their own posts and comments.

5. **Database:**
   - Use a relational database (e.g. MySQL).
   - Design the database schema based on the entities mentioned.

6. **Deployment:**
   - Dockerize the application.
   - Write a Dockerfile and a `docker-compose.yml` for easy setup.
   - Prepare the application for deployment on a cloud provider (e.g., AWS, Heroku).

### Evaluation Criteria:
- **Code Quality:** Clean, readable, and well-documented code.
- **Functionality:** The API should meet all specified requirements.
- **Security:** Proper implementation of authentication and authorization.
- **Database Design:** Efficient and normalized schema design.
- **Error Handling:** Graceful handling of errors and edge cases.
- **Deployment:** Successful containerization and readiness for deployment.
- **Testing:** Implement unit and integration tests for critical parts of the application.

### Submission Guidelines:
- Create a GitHub repository and commit your code.
- Deploy your code.
- Include a README.md file with instructions on how to set up and run the application.
- Ensure your submission includes sample data and API documentation (e.g., Postman collection).
- Send your links to intelregion.com@gmail.com
- Also, if you have any question you can forward them to intelregion.com@gmail.com

### Bonus Points:
- Implement pagination and search functionality for posts.
- Use a modern framework (e.g., NestJS, Django) to enhance productivity.
- Set up CI/CD pipeline for automated testing and deployment.

--- 

Note: Dealine for submission is Friday, 26th July, 2024. 
Goodluck.
