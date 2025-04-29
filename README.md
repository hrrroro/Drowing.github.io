<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Let's Draw!</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            background: radial-gradient(circle, #FFFFFF 60%, #FFFAE6 60%);
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 20px;
            font-family: Arial, sans-serif;
        }

        .header {
            font-size: 2em;
            color: #333;
            cursor: pointer;
        }

        .button-container {
            display: flex;
            flex-direction: column;
            margin-top: 20px;
        }

        .button {
            background-color: #FFFAE6;
            padding: 10px;
            margin: 5px;
            border: 1px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
            text-align: center;
        }

        .button:hover {
            background-color: #FFF0C1;
        }

        .submenu {
            display: none;
            flex-direction: column;
            margin-left: 20px;
        }

        .submenu .submenu-button {
            background-color: #FFFFFF;
            border: 1px solid #ddd;
            padding: 8px;
            margin: 5px;
            cursor: pointer;
            text-align: center;
        }

        .submenu .submenu-button:hover {
            background-color: #F1F1F1;
        }

        .show-submenu .submenu {
            display: flex;
        }
    </style>
</head>
<body>

    <div class="header" id="header">Let's Draw!</div>

    <div class="button-container">
        <div class="button" id="digitalPaintingBtn">Digital Painting</div>
        <div class="button">Ect.</div>

        <!-- Digital Painting Submenu -->
        <div class="submenu" id="digitalPaintingSubmenu">
            <div class="submenu-button">장비</div>
            <div class="submenu-button">그림툴</div>
            <div class="submenu-button">도서</div>
            <div class="submenu-button">강의</div>
            <div class="submenu-button">그림체</div>
        </div>
    </div>

    <script>
        const digitalPaintingBtn = document.getElementById('digitalPaintingBtn');
        const digitalPaintingSubmenu = document.getElementById('digitalPaintingSubmenu');

        digitalPaintingBtn.addEventListener('click', () => {
            digitalPaintingSubmenu.classList.toggle('show-submenu');
        });
    </script>

</body>
</html>
