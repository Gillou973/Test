# React PostgreSQL Form

This example shows how to create a simple form in React that inserts data into a PostgreSQL database using a small Express backend.

## Setup

1. Ensure PostgreSQL is running and create a database named `testdb` with a table:

```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL
);
```

2. Install dependencies in the `backend` directory:

```bash
npm install express body-parser pg
```

3. Start the backend server:

```bash
node server.js
```

4. Open `frontend/index.html` in a browser. The form will send requests to the backend to insert items.
