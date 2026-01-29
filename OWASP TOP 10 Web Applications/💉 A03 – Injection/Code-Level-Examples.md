# Code-Level Examples

Consider a backend service constructing a SQL query dynamically.

## Insecure Example

```java
String query = "SELECT * FROM users WHERE username = '" + user + "' AND password = '" + pass + "'";
Statement stmt = connection.createStatement();
ResultSet rs = stmt.executeQuery(query);

This code assumes that user input is simple text.
In reality, the database does not know the difference.
If the input alters the structure of the query, the database executes it faithfully.

The issue is not SQL itself.
The issue is that the query logic and user data are merged into a single instruction.

Secure Example

PreparedStatement stmt = connection.prepareStatement(
  "SELECT * FROM users WHERE username = ? AND password = ?"
);
stmt.setString(1, user);
stmt.setString(2, pass);

Here, the database understands the query structure first.
User input is treated as data only, regardless of content.

The same principle applies beyond SQL.
Whether the interpreter is a shell, a template engine, or an API query language, injection happens when structure and data are not isolated.

Secure code does not rely on developer discipline.
It relies on enforced separation.

