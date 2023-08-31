# Transaction Management Backend

This is a backend project built using Fastify and Knex to provide API endpoints for managing transactions. It allows users to create new transactions, obtain a summary of their account, list all transactions, and view a single transaction.

## Functional Requirements

- Users can create new transactions.
- Users can obtain a summary of their account.
- Users can list all transactions that have taken place.
- Users can view a single transaction.

## Business Rules

- Transactions can be of two types: credit or debit.
- A credit transaction adds to the total amount, while a debit transaction subtracts from it.
- User identification is required for requests.
- Users can only view transactions they have created.

## Features

- Create a new transaction.
- Retrieve an account summary.
- List all transactions.
- View a single transaction.

## Getting Started

1. Clone the repository.
2. Install the project dependencies using `npm install`.
3. Configure your database connection in `knexfile.js`.
4. Run database migrations using `npm run knex migrate:latest`.
5. Start the server with `npm start`.
6. The server will be running at `http://localhost:3000`.

## API Endpoints

- `POST /transactions`: Create a new transaction.
- `GET /account-summary`: Obtain a summary of the user's account.
- `GET /transactions`: List all transactions.
- `GET /transactions/:id`: View a single transaction.

## Technologies Used

- Fastify: A fast and low overhead web framework for Node.js.
- Knex: A SQL query builder for Node.js.
- PostgreSQL (or your preferred database): Used for data storage.

## Folder Structure

  - `src/`: Contains the source code for the backend application.
  - `controllers/`: Contains the route controllers.
  - `db/`: Contains database related configuration and migrations.
  - `models/`: Contains database models.
  - `routes/`: Contains the route definitions.
  - `index.js`: Entry point of the application.

## Contributing

Contributions are welcome! Please create a pull request with your changes.

## License

This project is licensed under the [MIT License](LICENSE).
