# E-commerce Back End

[![Node.js](https://img.shields.io/badge/Node.js-v14.17.3-green.svg)](https://nodejs.org/)
[![mysql2](https://img.shields.io/badge/mysql2-v2.3.0-blue.svg)](https://www.npmjs.com/package/mysql2) [![MySQL](https://img.shields.io/badge/MySQL-v8.0-blue.svg)](https://www.mysql.com/)
[![MySQL Workbench](https://img.shields.io/badge/MySQL%20Workbench-v8.0-blue.svg)](https://www.mysql.com/products/workbench/)
[![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-v1.59.0-blue.svg)](https://code.visualstudio.com/)

[![Sequelize](https://img.shields.io/badge/Sequelize-00b4db?style=for-the-badge&logo=sequelize&logoColor=white)](https://sequelize.org/)
[![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![Insomnia](https://img.shields.io/badge/Insomnia-5849BE?style=for-the-badge&logo=insomnia&logoColor=white)](https://insomnia.rest/)


## User Story

As a manager at an internet retail company, I want a back end for my e-commerce website that utilizes the latest technologies. This will enable my company to compete effectively with other e-commerce businesses.

## Acceptance Criteria

To fulfill the user story, the following acceptance criteria need to be met:

### 1. Database Configuration
- Given a functional Express.js API
- When I add my database name, MySQL username, and MySQL password to an environment variable file
- Then I am able to connect to a database using Sequelize

### 2. Database Initialization
- When I enter schema and seed commands
- Then a development database is created and seeded with test data

### 3. Application Initialization
- When I enter the command to invoke the application
- Then my server is started, and the Sequelize models are synced to the MySQL database

### 4. API Endpoints
- When I open API GET routes in Insomnia Core for categories, products, or tags
- Then the data for each of these routes is displayed in a formatted JSON

### 5. API Functionality
- When I test API POST, PUT, and DELETE routes in Insomnia Core
- Then I am able to successfully create, update, and delete data in my database

## Technologies Used
- Express.js
- MySQL
- Sequelize
- Insomnia Core

## Getting Started

1. Clone this repository to your local machine.

   ```bash
   git clone git@github.com:Otabek0111/E-commerceBackEnd.git
    ```
2. Navigate to the develop folder using the command prompt.

   ```bash
   cd E-commerceBackEnd
   ```
3. Install all required NPM packages.

   ```bash
    npm install
    ```
4. Create a .env file in the root of the project and add the following code to it:

    ```bash
     DB_NAME='ecommerce_db'
     DB_USER='root'
     DB_PW='your password'
     ```
5. Open MySQL shell and run the following commands:
    
        ```bash
        mysql> source db/schema.sql
        mysql> quit
        ```
6. Seed the database with test data:
    
        ```bash
        npm run seed
        ```
7. Start the server:
    
        ```bash
        npm start
        ```
8. Open Insomnia Core and test the API routes.

## Video Walkthrough

[Watch the video](https://watch.screencastify.com/v/SOvnofe6UlD7PKmI2fW9)







## API Endpoints

### Categories

- GET `/api/categories` - get all categories
- GET `/api/categories/:id` - get one category by id
- POST `/api/categories` - create a new category
- PUT `/api/categories/:id` - update a category by id
- DELETE `/api/categories/:id` - delete a category by id

### Products

- GET `/api/products` - get all products
- GET `/api/products/:id` - get one product by id
- POST `/api/products` - create a new product
- PUT `/api/products/:id` - update a product by id
- DELETE `/api/products/:id` - delete a product by id

### Tags

- GET `/api/tags` - get all tags
- GET `/api/tags/:id` - get one tag by id
- POST `/api/tags` - create a new tag
- PUT `/api/tags/:id` - update a tag by id
- DELETE `/api/tags/:id` - delete a tag by id



## Resources and Technologies Used 


- [Node.js](https://nodejs.org/en/) 
- [mysql2](https://www.npmjs.com/package/mysql2)
- [MySQL](https://www.mysql.com/)
- [MySQL Workbench](https://www.mysql.com/products/workbench/)
- [Visual Studio Code](https://code.visualstudio.com/) 
- [dotenv](https://www.npmjs.com/package/dotenv)
- [Sequelize](https://sequelize.org/)
- [Express](https://expressjs.com/)
- [Insomnia](https://insomnia.rest/)
- [Screencastify](https://www.screencastify.com/)


## License

This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE) file for details 