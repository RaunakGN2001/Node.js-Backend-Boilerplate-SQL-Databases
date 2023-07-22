# Node.js Backend Project Boilerplate (SQL Databases)

This Node.js Backend Project Boilerplate is designed to provide a solid foundation for building backend applications using SQL databases. It follows the Model-View-Controller (MVC) architecture and includes major folders to organize your code effectively.

## Features

- MVC Architecture: Easily manage your application's components with clear separation of concerns.
- SQL Database Support: Built to work with SQL databases for data storage and retrieval.
- Organized Codebase: Major folders for different components to keep your codebase clean and maintainable.
- Ready-to-Use Structure: Clone this repository as a starting point for any new backend project.

## Folder Structure

The project follows a well-organized folder structure to help you easily manage your codebase:

- **config**: Contains configuration files for your application, such as database configurations, environment variables, etc.
- **controllers**: Handles the application's logic by interacting with models and sending responses to clients.
- **middlewares**: Includes custom middleware functions for request processing and handling.
- **migrations**: Stores database migration files to manage database schema changes.
- **models**: Defines database models and interacts with the database through Sequelize ORM.
- **repositories**: Implements data access logic to interact with the database models.
- **routes**: Contains route files that define API endpoints and link them to corresponding controllers.
- **seeders**: Stores database seed files to populate initial data into the database.
- **services**: Contains business logic and application services.
- **utils**: Holds utility functions and helper modules to be used throughout the application.
- **logs**: Used to store application logs for debugging and monitoring.

## Prerequisites

Before using this project boilerplate, ensure you have the following installed:

- Node.js (>=12.x)
- npm (>=6.x)
- SQL Database (e.g., PostgreSQL, MySQL, SQLite)

## Getting Started

1. Fork this repository first.
2. Clone the forked repo to your local machine:

```
git clone https://github.com/<your-github-username>/Node.js-Backend-Boilerplate-SQL-Databases.git
cd Node.js-Backend-Boilerplate-SQL-Databases
```

2. Install dependencies using npm:

```
npm install
```

3. Configure your database connection by creating a config.json file inside src/config/ and update the credentials in the following format:
```
{
  "development": {
    "username": "root",
    "password": your-db-password,
    "database": "database_development",
    "host": "127.0.0.1",
    "dialect": /* one of 'mysql' | 'postgres' | 'sqlite' | 'mariadb' | 'mssql' | 'db2' | 'snowflake' | 'oracle' */
  },
  "test": {
    "username": "root",
    "password": your-db-password,
    "database": "database_test",
    "host": "127.0.0.1",
    "dialect": /* one of 'mysql' | 'postgres' | 'sqlite' | 'mariadb' | 'mssql' | 'db2' | 'snowflake' | 'oracle' */
  },
  "production": {
    "username": "root",
    "password": your-db-password,
    "database": "database_production",
    "host": "127.0.0.1",
    "dialect": /* one of 'mysql' | 'postgres' | 'sqlite' | 'mariadb' | 'mssql' | 'db2' | 'snowflake' | 'oracle' */
  }
}
```

4. Run database migrations to set up the database schema:

```
npx sequelize-cli db:migrate
```

5. Optionally, you can run database seeders to populate initial data:

```
npx sequelize-cli db:seed:all
```

6. Start the development server:

```
npm start
```

You can now begin building your backend application on top of this boilerplate!

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

Happy coding! :rocket:
