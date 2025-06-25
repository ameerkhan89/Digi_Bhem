# Digi_Bhem
Creating a real time calculator using hml,css and javascript
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            color: #333;
        }

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 50px;
        }

        h1 {
            margin-bottom: 20px;
        }

        .calculator {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
        }

        input[type="text"] {
            width: 100%;
            margin-bottom: 10px;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 3px;
            box-sizing: border-box;
        }

        .buttons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            grid-gap: 10px;
        }

        button {
            padding: 10px;
            border: none;
            background-color: #eee;
            border-radius: 3px;
            cursor: pointer;
        }

        button:hover {
            background-color: #ddd;
        }

        .mode-toggle {
            margin-top: 20px;
        }

        .mode-toggle label {
            margin-right: 10px;
        }

        .dark-mode {
            background-color: #333;
            color: #fff;
        }

        .dark-mode button {
            background-color: #555;
        }

        .dark-mode button:hover {
            background-color: #444;
        }
    </style>
</head>

<body>
    <div class="container">
        <h1>Calculator</h1>
        <div class="calculator">
            <input type="text" id="display" disabled>
            <div class="buttons">
                <button onclick="clearDisplay()">C</button>
                <button onclick="appendToDisplay('/')">/</button>
                <button onclick="appendToDisplay('*')">x</button>
                <button onclick="appendToDisplay('-')">-</button>
                <button onclick="appendToDisplay('7')">7</button>
                <button onclick="appendToDisplay('8')">8</button>
                <button onclick="appendToDisplay('9')">9</button>
                <button onclick="appendToDisplay('+')">+</button>
                <button onclick="appendToDisplay('4')">4</button>
                <button onclick="appendToDisplay('5')">5</button>
                <button onclick="appendToDisplay('6')">6</button>
                <button onclick="calculate()">=</button>
                <button onclick="appendToDisplay('1')">1</button>
                <button onclick="appendToDisplay('2')">2</button>
                <button onclick="appendToDisplay('3')">3</button>
                <button onclick="appendToDisplay('0')">0</button>
            </div>
        </div>
        <div class="mode-toggle">
            <label for="mode-toggle">Mode:</label>
            <input type="checkbox" id="mode-toggle" onchange="toggleMode()">
        </div>
    </div>
    <script>
        let displayValue = '';

        function appendToDisplay(value) {
            displayValue += value;
            document.getElementById('display').value = displayValue;
        }

        function calculate() {
            try {
                const result = eval(displayValue);
                document.getElementById('display').value = result;
                displayValue = '';
            } catch (error) {
                document.getElementById('display').value = 'Error';
                displayValue = '';
            }
        }

        function clearDisplay() {
            displayValue = '';
            document.getElementById('display').value = '';
        }

        function toggleMode() {
            const body = document.querySelector('body');
            body.classList.toggle('dark-mode');
        }
    </script>
</body>

</html>
