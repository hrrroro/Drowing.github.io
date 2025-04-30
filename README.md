<html lang="ko">
<head>
  <meta charset="UTF-8">
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
      padding: 0;
      background-color: #FFFAE6; /* 단색 배경 */
      font-family: 'KCCImkwontaek', sans-serif;
      color: #000;
    }

    .container {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      height: 100vh;
      padding: 2rem;
    }

    .left {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .title {
      font-size: 2.5rem;
      color: #f08ca3; /* 핑크색 텍스트 */
      white-space: pre-line;
      margin-bottom: 2rem;
      font-family: 'KCCImkwontaek', sans-serif;
    }

    .menu {
      font-size: 1rem;
      line-height: 1.6;
    }

    .top-right {
      position: absolute;
      top: 1rem;
      right: 2rem;
      font-size: 0.85rem;
    }
  </style>
</head>
<body>
  <div class="top-right">마음껏 그려보세요</div>

  <div class="container">
    <div class="left">
      <div class="title">Let's<br>Draw!</div>
      <div class="menu">
        Digital Painting<br>
        장비<br>
        그림툴<br>
        그림체<br>
        도서<br>
        강의<br>
        ect.
      </div>
    </div>
  </div>
</body>
</html>
