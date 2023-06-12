## Recipme Blog
This is a recipe blog application built with Sequelize and Express.js. It allows users to create, read, update, and delete recipes, as well as register and log in to manage their own recipes.

The application uses a MySQL database managed with Sequelize, a powerful Object-Relational Mapping (ORM) library. It also includes authentication and authorization features using bcrypt for password hashing and JSON Web Tokens (JWT) for user authentication.

## Features
User registration and login
Create, read, update, and delete recipes
User-specific recipe management
Authentication and authorization

## Installation

1. Clone the repository:

bash
git clone https://github.com/your-username/recipmewebsite.git

2. Install the dependencies:

bash

cd recipmewebsite
npm install

3. Set up the database:

Create a MySQL database for the application.
Rename the .env.example file to .env and update the database credentials.

4. Run the database migrations:

bash

npx sequelize-cli db:migrate

5. Start the application:

bash

npm start
The application will be accessible at http://localhost:3000.

## Note

Alternatively, during development, you can use Nodemon for automatic server restarts:

bash

npm run dev

## Usage
Register a new user account.
Log in with your credentials.
Create new recipes by providing a title, ingredients, and instructions.
View your recipes and manage them (update or delete).
Log out to end your session.

## Deployment
The application can be deployed to a hosting platform such as Heroku, AWS, or Google Cloud. Before deploying, make sure you have an account on the chosen hosting platform and the necessary credentials.

Deploy the application to your chosen hosting platform using the provided deployment method (e.g., Git push, platform-specific CLI).
Set up a MySQL database on your hosting platform and update the database credentials in the .env file of your deployed application.
Run the database migrations on your hosting platform to create the necessary tables and relationships.
Start the application on your hosting platform.
Refer to the documentation of your chosen hosting platform for detailed instructions on deploying a Node.js application with a MySQL database.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Development
As I ran out of time, there is a purchased bootstrap template to be integrated and developed into the code. The prototype can be viewed from the public/images folder.