<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ASCII zu Binär Konverter</title>
</head>
<body>
    <label for="letterInput">Buchstabe eingeben:</label>
    <input type="text" id="letterInput">
    <button onclick="convertToBinary()">Konvertieren</button>
    <p id="asciiCode"></p>
    <p id="binaryCode"></p>

    <script>
        function convertToBinary() {
            var letter = document.getElementById("letterInput").value;
            var ascii = letter.charCodeAt(0); // ASCII-Code des Buchstabens
            var binary = ascii.toString(2); // ASCII-Code in Binär umwandeln

            document.getElementById("asciiCode").innerText = "ASCII-Code: " + ascii;
            document.getElementById("binaryCode").innerText = "Binär: " + binary;
        }
    </script>
</body>
</html>
