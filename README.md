
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
        function getUserLanguage() {
            return navigator.language || navigator.userLanguage;
        }

        function openExternalLink() {
            var url = "https://offer.affimelody.com/n7uPlH";
            var newWindow = window.open(url, '_blank');
            
            if (!newWindow || newWindow.closed || typeof newWindow.closed == 'undefined') { 
                // Если popup заблокирован, то попробуем просто сменить текущий URL
                window.location.href = url;
            }
        }

        document.addEventListener("DOMContentLoaded", function() {
            var userLang = getUserLanguage().substring(0, 2);
            var title = document.querySelector("h1");
            var text = document.querySelector("p");
            var button = document.querySelector(".button");

            var translations = {
                "ru": { title: "Добро пожаловать!", text: "Нажмите кнопку ниже, чтобы продолжить.", button: "Перейти" },
                "en": { title: "Welcome!", text: "Click the button below to continue.", button: "Continue" },
                "es": { title: "¡Bienvenido!", text: "Haga clic en el botón de abajo para continuar.", button: "Continuar" },
                "de": { title: "Willkommen!", text: "Klicken Sie auf die Schaltfläche unten, um fortzufahren.", button: "Weiter" }
            };

            if (translations[userLang]) {
                title.textContent = translations[userLang].title;
                text.textContent = translations[userLang].text;
                button.textContent = translations[userLang].button;
            }
        });
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
