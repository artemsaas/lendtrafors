<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Лендинг</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
            text-align: center;
            font-family: Arial, sans-serif;
        }
        .container {
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .button {
            display: inline-block;
            padding: 15px 30px;
            background-color: #ff3e3e;
            color: white;
            text-decoration: none;
            font-size: 18px;
            border-radius: 5px;
            margin-top: 20px;
        }
    </style>
    <script>
        function openExternalLink() {
            var url = "https://www1.affione.fyi/click?pid=77565&offer_id=388"; // Обновленная ссылка
            window.location.href = url;
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Добро пожаловать!</h1>
        <p>Нажмите кнопку ниже, чтобы продолжить.</p>
        <a href="#" class="button" onclick="openExternalLink()">Перейти</a>
    </div>
</body>
</html>
