# sqlite3

This is my database that allows the user to enter their credentials like: username, email address and password.

Here is the snapshot of the sql table
````py
CREATE TABLE IF NOT EXISTS users(
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    username VARCHAR(255) UNIQUE NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    password VARCHAR(300) UNIQUE NOT NULL,
    create_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

````