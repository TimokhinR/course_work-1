<!DOCTYPE html>
<html lang="uk">

<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Авторизація</title>
    <style>
        /* Стилі тут... */
    </style>
</head>

<body>
    <header>
        <h1>Авторизація</h1>
    </header>
    <section class="section">
        <form id="loginForm">
            <label for="username">Логін:</label>
            <input type="text" id="username" name="username" required>

            <label for="password">Пароль:</label>
            <input type="password" id="password" name="password" required>

            <button type="button" onclick="authenticateUser()">Увійти</button>
        </form>
    </section>

<script>
    function authenticateUser() {
        var username = document.getElementById("username").value;
        var password = document.getElementById("password").value;


        if (username && password) {

            window.location.href = "головна_сторінка.html";
        } else {
            alert("Будь ласка, введіть логін і пароль");
        }
    }
</script>
