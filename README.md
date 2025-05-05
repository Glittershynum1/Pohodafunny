# Pohodafunny
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Погода</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 100px;
      background: #e0f7fa;
    }
    .weather-box {
      margin: 20px auto;
      padding: 30px;
      width: 200px;
      border-radius: 15px;
      background: #ffffff;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      font-size: 24px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 10px;
      border: none;
      background-color: #4fc3f7;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #039be5;
    }
  </style>
</head>
<body>

  <div class="weather-box" id="weather">
    ☀️ Сонячно
  </div>
  <button onclick="changeWeather()">Змінити погоду</button>

  <script>
    const weathers = [
      "☀️ Сонячно",
      "🌧️ Дощ",
      "❄️ Сніг",
      "🌫️ Туман",
      "🌩️ Гроза",
      "🌬️ Вітер",
      "⛅ Хмарно"
    ];

    function changeWeather() {
      const randomIndex = Math.floor(Math.random() * weathers.length);
      document.getElementById('weather').textContent = weathers[randomIndex];
    }
  </script>

</body>
</html>
