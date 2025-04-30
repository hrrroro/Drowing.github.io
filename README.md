<!DOCTYPE html>
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
      background-color: #FFFAE6;
      font-family: 'KCCImkwontaek', sans-serif;
      color: #000;
      height: 100vh;
      overflow: hidden;
    }

    .container {
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;
      padding: 2rem 3rem;
      height: 100%;
    }

    .title {
      font-size: 2.5rem;
      color: #f08ca3;
      white-space: pre-line;
      margin-bottom: 2rem;
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
      font-family: sans-serif;
    }

    /* 깃허브 기본 스타일 제거 */
    header {
      display: none !important;
    }
  </style>
</head>
<body>
  <div class="top-right">마음껏 그려보세요</div>

  <div class="container">
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
</body>
</html>
