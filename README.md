<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Love for You 💖</title>
  <style>
    body {
      background-color: #000;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .heart {
      width: 100px;
      height: 90px;
      position: relative;
      transform: scale(1);
      animation: beat 1s infinite;
    }

    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      top: 0;
      width: 100px;
      height: 90px;
      background: red;
      border-radius: 50px 50px 0 0;
    }

    .heart::before {
      left: 50px;
      transform: rotate(-45deg);
      transform-origin: 0 100%;
    }

    .heart::after {
      left: 0;
      transform: rotate(45deg);
      transform-origin: 100% 100%;
    }

    @keyframes beat {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.2);
      }
    }
  </style>
</head>
<body>
  <div class="heart"></div>
</body>
</html>
