# Web-Dev-Week-2-Assignment
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Expense Management System</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            color: #333;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background-color: #007bff;
            color: #fff;
            padding: 10px 0;
            margin-bottom: 20px;
        }
        nav {
            background-color: #343a40;
            color: #fff;
            padding: 10px 0;
            margin-bottom: 20px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }
        section {
            margin: 20px;
            padding: 20px;
            background-color: #fff;
            border: 1px solid #ddd;
            border-radius: 5px;
            text-align: left;
        }
        form {
            margin-top: 20px;
        }
        form label {
            display: block;
            margin-bottom: 10px;
            font-weight: bold;
        }
        form input[type="text"], form input[type="password"], form textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }
        form input[type="submit"] {
            background-color: #007bff;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        form input[type="submit"]:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <header>
        <h1>Expense Management System</h1>
    </header>
    <nav>
        <a href="#index">Home</a>
        <a href="#register">Register</a>
        <a href="#login">Login</a>
        <a href="#add_expense">Add Expense</a>
        <a href="#edit_expense">Edit Expense</a>
        <a href="#view_expense">View Expense</a>
    </nav>
    <section id="index">
        <h2>Welcome to Expense Management System</h2>
        <p>This is the main page of the system.</p>
    </section>
    <section id="register">
        <h2>Register</h2>
        <form action="register.php" method="post">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required>
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required>
            <input type="submit" value="Register">
        </form>
    </section>
    <section id="login">
        <h2>Login</h2>
        <form action="login.php" method="post">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required>
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required>
            <input type="submit" value="Login">
        </form>
    </section>
    <section id="add_expense">
        <h2>Add Expense</h2>
        <form action="add_expense.php" method="post">
            <label for="expense_name">Expense Name:</label>
            <input type="text" id="expense_name" name="expense_name" required>
            <label for="amount">Amount:</label>
            <input type="text" id="amount" name="amount" required>
            <label for="description">Description:</label>
            <textarea id="description" name="description"></textarea>
            <input type="submit" value="Add Expense">
        </form>
    </section>
    <section id="edit_expense">
        <h2>Edit Expense</h2>
        <form action="edit_expense.php" method="post">
            <label for="expense_id">Expense ID:</label>
            <input type="text" id="expense_id" name="expense_id" required>
            <label for="new_amount">New Amount:</label>
            <input type="text" id="new_amount" name="new_amount" required>
            <input type="submit" value="Edit Expense">
        </form>
    </section>
    <section id="view_expense">
        <h2>View Expense</h2>
        <p>Here you can view all expenses.</p>
    </section>
</body>
</html>
