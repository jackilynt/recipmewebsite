# Recipme Blog

This is a recipe blog application built with Sequelize and Express.js. It allows users to create, read, update, and delete recipes, as well as register and log in to manage their own recipes.

The application uses a PostgreSQL database managed with Sequelize, a powerful Object-Relational Mapping (ORM) library. It also includes authentication and authorization features using bcrypt for password hashing and JSON Web Tokens (JWT) for user authentication.

## Features

- User registration and login
- Create, read, update, and delete recipes
- User-specific recipe management
- Authentication and authorization

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/recipmewebsite.git
   ```

2. Install the dependencies:

bash

cd recipe-blog
npm install

3. Set up the database:

Create a PostgreSQL database for the application.
Rename the .env.example file to .env and update the database credentials.

4. Run the database migrations:

bash

npx sequelize-cli db:migrate

5. Start the application:

bash

npm start
The application will be accessible at http://localhost:3000.

Alternatively during development, add the nodemon script to your modules:

 "devDependencies": {
    "nodemon": "^2.0.22"
  }

npm install nodemon --save-dev

add script    "dev": "nodemon server.js"

npm run dev

## Usage
Register a new user account.
Log in with your credentials.
Create new recipes by providing a title, ingredients, and instructions.
View your recipes and manage them (update or delete).
Log out to end your session.

## Deployment
The application can be deployed to Heroku for production. Before deploying, make sure you have a Heroku account and the Heroku CLI installed on your machine.

Create a new Heroku app:

bash

heroku create
Provision a PostgreSQL database addon:

bash

heroku addons:create heroku-postgresql
Set the environment variables on Heroku:

bash

heroku config:set DATABASE_URL=<your_database_url>
heroku config:set JWT_SECRET=<your_jwt_secret>
Deploy the application to Heroku:

bash

git push heroku main
Run the database migrations on Heroku:

bash

heroku run npx sequelize-cli db:migrate
Open the deployed application in your browser:

bash

heroku open

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Development
As I ran out of time, there is a purchased bootstrap template to be integrated and developed into the code. The prototype can viewed from the public/images folder.
