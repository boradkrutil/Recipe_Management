Recipe App
This is a recipe application built with the MERN stack (MongoDB, Express.js, React.js, and Node.js). It allows users to sign up, log in, log out and perform CRUD operations on recipes. The project consists of two controllers: the user controller for authentication and the recipe controller.

Features
User authentication (sign up, log in, and log out)
Recipe management (create, read, update, and delete recipes)
User authentication middleware for protected routes
API documentation using Swagger UI
Dependencies
kindly check the package.json file for all the dependencies

Installation
Install the dependencies: npm install

cd <project_directory>
npm i
npm start
Configure the environment variables:

Update the necessary values in the .env file, such as the database connection URL.
Create a .env file in the root directory and add the following variables:

PORT = 5050
MONGO_URI = your mongoDB Atlas link
SECRET_KEY = your Secret key

The application will start running on http://localhost:${port}. Please refer to the API documentation using Swagger UI for more details on request and response formats.

Routes
For User : 
POST /user/register: Create a new user account.
POST /user/login: Log in to an existing user account.
GET /user/logout: Log out the current user.

For Recipe : 
POST /recipe/add: create a recipe
GET /recipe/: Get a all recipe 
GET /recipe/:recipeId: Get a recipe by its ID.
DELETE /recipe/delete/:recipeId: Delete a recipe by its ID.
PATCH /recipe/update/:recipeId: Update a recipe by its ID.
