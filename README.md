<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Let's Draw!</title>
    <style>
        @font-face {
            font-family: 'KCCImkwontaek';
            src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/noonfonts_2202@1.0/KCCImkwontaek.woff') format('woff');
            font-weight: normal;
            font-style: normal;
        }

        body {
            margin: 0;
            height: 100vh;
            background: 
                linear-gradient(45deg, #FFFAE6 25%, #FFFFFF 25%) 0 0,
                linear-gradient(-45deg, #FFFAE6 25%, #FFFFFF 25%) 0 0,
                linear-gradient(45deg, #FFFFFF 75%, #FFFAE6 75%) 0 0,
                linear-gradient(-45deg, #FFFFFF 75%, #FFFAE6 75%) 0 0;
            background-size: 50px 50px;
            background-repeat: no-repeat;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 20px;
            font-family: Arial, sans-serif;
        }

        .header {
            font-family: 'KCCImkwontaek', sans-serif;
            font-size: 2em;
            color: #333;
            cursor: pointer;
            text-align: left;
            width: 100%;
        }

        .button-container {
            display: flex;
            flex-direction: column;
            margin-top: 20px;
            align-items: flex-start;
        }

        .button {
            color: #FFFAE6;
            font-size: 1.5em;
            margin: 10px 0;
            cursor: pointer;
            text-align: left;
            width: 100%;
        }

        .button:hover {
            color: #FFF0C1;
        }

        .submenu {
            display: none;
            flex-direction: column;
            margin-left: 20px;
        }

        .submenu .submenu-button {
            color: #FFFAE6;
            font-size: 1.2em;
            margin: 5px 0;
            cursor: pointer;
            text-align: left;
            width: 100%;
        }

        .submenu .submenu-button:hover {
            color: #FFF0C1;
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
