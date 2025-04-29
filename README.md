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
            background-color: #FFFAE6; /* 배경 색상 변경 */
            display: flex;
            flex-direction: column;
            align-items: flex-start; /* 왼쪽 정렬 */
            padding: 20px;
            font-family: Arial, sans-serif;
        }

        .header {
            font-family: 'KCCImkwontaek', sans-serif;
            font-size: 2em;
            color: #FFADAD;
            cursor: pointer;
            text-align: left;
            width: 100%;
        }

        .header span {
            display: block;
        }

        .button-container {
            display: flex;
            flex-direction: column;
            margin-top: 20px;
            align-items: flex-start; /* 버튼들도 왼쪽 정렬 */
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
            color: #505050;
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

    <div class="header" id="header">
        <span>Let's</span>
        <span>Draw!</span>
    </div>

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
