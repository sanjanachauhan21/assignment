#Assignment
css workshop assingnment
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Number Incrementer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #dfe6e9; /* Light blue-gray */
      margin: 0;
      padding: 0;
    }

    .container {
      width: 50%;
      margin: 50px auto;
      padding: 20px;
      background-color: #ffffff; /* White */
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    }

    h1 {
      color: #6c5ce7; /* Purple */
      text-align: center;
    }

    .input-container {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 20px;
    }

    input[type="number"] {
      width: 100px;
      padding: 10px;
      border: 2px solid #6c5ce7; /* Purple */
      border-radius: 5px;
      font-size: 16px;
      text-align: center;
    }

    .button-container {
      margin-top: 20px;
      display: flex;
      justify-content: center;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin: 0 10px;
      background-color: #0984e3; /* Blue */
      color: white;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #6c5ce7; /* Purple */
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Number Incrementer</h1>
    <div class="input-container">
      <input type="number" id="numberInput" value="0">
    </div>
    <div class="button-container">
      <button onclick="increment(1)">+1</button>
      <button onclick="increment(-1)">-1</button>
      <button onclick="increment(10)">+10</button>
      <button onclick="increment(-10)">-10</button>
    </div>
  </div>

  <script>
    function increment(value) {
      var numberInput = document.getElementById("numberInput");
      var currentValue = parseInt(numberInput.value);
      numberInput.value = currentValue + value;
    }
  </script>
</body>
</html>
