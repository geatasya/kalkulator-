<!DOCTYPE html>
<html lang="id">
<head>
    <title>Kalkulator</title>
    <style type="text/css">
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #2b2b2b;
            color: white;
            font-family: Arial, sans-serif;
        }
        .operator{
            background-color: rgb(122, 122, 122);
        }
        table {
            background-color: rgb(255, 255, 255);
            border-radius: 15px;
            border-spacing: 5px;
            padding: 20px;
        }
        input {
            width: 90%;
            height: 30px;
            font-size: 20px;
            text-align: right;
            border-radius: 5px;
            border: none;
            padding: 10px;
            margin-bottom: 10px;
        }
        button {
            width: 100%;
            padding: 20px;
            color: beige;
            background-color: slategray;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            font-size: 18px;
            border: none;
        }
        .samadengan {
            height: 270px;
            background-color: rgb(18, 209, 18);
        }
        .clear {
            background-color: rgb(216, 11, 11);
        }
    </style>
</head>
<body>
    <table border="1">
        <tr>
            <td colspan="4"><input type="text" id="display" readonly></td>
        </tr>
        <tr>
            <td><button class="operator" onclick="appendToDisplay('+')">+</button></td>
            <td><button class="operator" onclick="appendToDisplay('-')">-</button></td>
            <td><button class="operator" onclick="appendToDisplay('*')">x</button></td>
            <td><button class="operator" onclick="appendToDisplay('/')">:</button></td>
        </tr>
        <tr>
            <td><button onclick="appendToDisplay('1')">1</button></td>
            <td><button onclick="appendToDisplay('2')">2</button></td>
            <td><button onclick="appendToDisplay('3')">3</button></td>
            <td rowspan="4"><button class="samadengan" onclick="calculateResult()">=</button></td>
        </tr>
        <tr>
            <td><button onclick="appendToDisplay('4')">4</button></td>
            <td><button onclick="appendToDisplay('5')">5</button></td>
            <td><button onclick="appendToDisplay('6')">6</button></td>
        </tr>
        <tr>
            <td><button onclick="appendToDisplay('7')">7</button></td>
            <td><button onclick="appendToDisplay('8')">8</button></td>
            <td><button onclick="appendToDisplay('9')">9</button></td>
        </tr>
        <tr>
            <td><button onclick="appendToDisplay('.')">.</button></td>
            <td><button onclick="appendToDisplay('0')">0</button></td>
            <td><button class="clear" onclick="clearDisplay()">C</button></td>
        </tr>
    </table>
    <script>
        function appendToDisplay(value) {
            document.getElementById("display").value += value;
        }
        function calculateResult() {
            try {
                document.getElementById("display").value = eval(document.getElementById("display").value);
            } catch (e) {
                alert("Input tidak valid");
            }
        }
        function clearDisplay() {
            document.getElementById("display").value = "";
        }
    </script>
</body>
</html>
