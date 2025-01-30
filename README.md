<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Документы Карсакбаевой Жулдыз</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }
        .page {
            display: none;
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 80%;
            max-width: 600px;
        }
        .page.active {
            display: block;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <div id="page1" class="page active">
            <h1>КАРСАКБАЕВА ЖУЛДЫЗ</h1>
            <p>ИИН: 030604601931</p>
            <h2>Мои эцп</h2>
            <h3>Адреса</h3>
            <button onclick="showPage('page2')">Мои документы</button>
        </div>
        <div id="page2" class="page">
            <h1>Мои документы</h1>
            <h2>Документы, удостоверяющие личность</h2>
            <h3>УДОСТОВЕРЕНИЕ РК №048637885</h3>
            <p>Орган выдачи: МИНИСТЕРСТВО ВНУТРЕННИХ ДЕЛ РК</p>
            <p>21.06.2020 - 20.06.2031</p>
            <p>ИИН 030604601931</p>
            <h3>ПАСПОРТ РК N13685442</h3>
            <p>Орган выдачи: МИНИСТЕРСТВО ВНУТРЕННИХ ДЕЛ РК</p>
            <p>14.05.2020 - 13.05.2031</p>
            <p>ИИН 030604601931</p>
            <button onclick="showPage('page1')">Назад</button>
        </div>
    </div>

    <script>
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            document.getElementById(pageId).classList.add('active');
        }
    </script>
</body>
</html>
