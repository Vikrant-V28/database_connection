<div align="center">
  <img height="60" src="https://user-images.githubusercontent.com/85709371/153715216-fd60ffca-1b79-4531-b03d-201440ecaee3.png">
  <img height="60" src="![mysql](https://user-images.githubusercontent.com/85709371/157084352-f7d187f7-b6df-4e14-91df-3fc7b7325d28.png)">
</div>

# MYSQL Database Connection with JavaScript - NodeJS 
The simple script to create Database connection using JavaScript.

### Prerequisites
- `JavaScript`
- `NodeJS`

### usage
Steps :
1. Open Terminal or Command Prompt.
2. Set Path to where File is Located (using cd).
3. Type `node databse_connection.js` and Click Enter
---

## Code🧑🏻‍💻
```javascript
var mysql = require("mysql")
var con = mysql.createConnection(
    {
        host: "localhost",
        user: "root",
        password: "password", // enter your password here
        database: "database_name" // enter database name 
    })

con.connect(function (err) {
    if (err)
        throw err;
    console.log("Connected");
    con.query("create database student", function (err, result) {
        if (err)
            throw err;
        console.log("Database created sucessfully");
    })

})
```
