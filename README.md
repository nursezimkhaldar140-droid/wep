<div class="card">Содержимое карточки</div>

<style>
  .card {
    padding: 16px;
    border: 1px solid;
    border-radius: 8px;
  }
</style>

<div class="row">
  <div>Элемент 1</div>
  <div>Элемент 2</div>
  <div>Элемент 3</div>
</div>

<style>
  .row {
    display: flex;
    justify-content: space-between;
  }
</style>
```
!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Адаптивная страница</title>

  <style>
    .container {
      display: flex;
      flex-direction: row;
    }

    .block {
      padding: 20px;
      margin: 10px;
      background-color: lightblue;
    }

    @media (max-width: 600px) {
      .container {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <div class="container">
    <div class="block">Блок 1</div>
    <div class="block">Блок 2</div>
    <div class="block">Блок 3</div>
  </div>
</body>
</html>

const input = require('fs').readFileSync(0, 'utf-8').trim();
const n = Number(input);

function isEven(n) {
  return n % 2 === 0;
}

console.log(isEven(n));
!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Кнопка</title>
</head>
<body>

  <button id="myButton">Нажми меня</button>
  <p id="message">Исходный текст</p>

  <script>
    const button = document.getElementById('myButton');
    const message = document.getElementById('message');

    button.addEventListener('click', function() {
      message.textContent = 'Кнопка нажата!';
    });
  </script>

</body>
</html>

