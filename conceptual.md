### Conceptual Exercise

Answer the following questions below:

- What is PostgreSQL?
PostgreSQL is an open-source relational database management system (RDBMS) known for its robustness, extensibility, and standards compliance. It supports SQL (Structured Query Language) and is known for its advanced features, including support for complex queries, indexing, and transactions.

- What is the difference between SQL and PostgreSQL?
SQL (Structured Query Language) is a standard language for managing and manipulating relational databases. PostgreSQL is one specific implementation of an RDBMS that follows the SQL standard. While SQL provides a general set of syntax and commands, PostgreSQL adds its own extensions and features beyond the standard, making it a specific RDBMS product.

- In `psql`, how do you connect to a database?
To connect to a database using `psql`, you use the following command:
### ```bash
### psql -U <username> -d <database_name>
Replace <username> with your PostgreSQL username and <database_name> with the name of the database you want to connect to.

- What is the difference between `HAVING` and `WHERE`?
The WHERE clause is used to filter rows before they are grouped and aggregated in a query. On the other hand, the HAVING clause is used to filter the results of aggregate functions in a query. In simple terms, WHERE is used for filtering individual rows, while HAVING is used for filtering aggregated results.

- What is the difference between an `INNER` and `OUTER` join?
An INNER join returns only the rows that have matching values in both tables, excluding non-matching rows. Conversely, an OUTER join returns all rows from one table and the matched rows from another. Non-matching rows from the second table contain NULL values.

- What is the difference between a `LEFT OUTER` and `RIGHT OUTER` join?
In a LEFT OUTER JOIN, all rows from the left table are returned along with the matched rows from the right table. If there is no match, NULL values are returned for columns from the right table. In a RIGHT OUTER JOIN, it's the opposite: all rows from the right table are returned with matched rows from the left table or NULL values if there is no match.

- What is an ORM? What do they do?
ORM stands for Object-Relational Mapping. It is a programming technique that converts data between incompatible type systems, in object-oriented programming languages, by creating a virtual object database. In the context of databases, an ORM allows developers to interact with a database using an object-oriented paradigm, abstracting away the underlying SQL queries.

- What are some differences between making HTTP requests using AJAX and from the server side using a library like `requests`?
AJAX (Asynchronous JavaScript and XML) is used for making asynchronous requests from the client side, typically in web browsers. It allows updating parts of a web page without reloading the entire page. On the server side, the requests library in Python is used to make HTTP requests. The primary difference is the context: AJAX is client-side, while requests is server-side. Additionally, AJAX requests are typically initiated by user interactions, while server-side requests are often part of the backend logic.

- What is CSRF? What is the purpose of the CSRF token?
CSRF (Cross-Site Request Forgery) is a type of security vulnerability where an attacker tricks a user's browser into performing an undesired action on a web application in which the user is authenticated. To mitigate CSRF attacks, a CSRF token is often used. The purpose of the CSRF token is to validate that the requests coming to the server are legitimate and were initiated by the same application. The token is typically included in forms and headers to ensure that the request is not a result of a malicious third-party site.

- What is the purpose of `form.hidden_tag()`?
In Flask-WTF (WTForms for Flask), form.hidden_tag() is used to render hidden input fields for CSRF protection. It includes a hidden input field with the CSRF token, which is then used to verify the integrity of form submissions and protect against CSRF attacks. This function is often included in HTML forms to ensure that the CSRF token is submitted with the form data.
