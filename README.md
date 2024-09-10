<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div id="cake-section">
            <img src="https://image.shutterstock.com/image-vector/cute-birthday-cake-19-number-260nw-1536829799.jpg" id="birthday-cake" alt="Birthday Cake with 19 Candle">
            <button id="wish-button" onclick="makeAWish()">Make a Wish</button>
        </div>

        <div id="message-section" class="hidden">
            <h1>Happy Birthday, My Baby!</h1>
            <div class="flowers">
                <img src="https://image.shutterstock.com/image-photo/bouquet-roses-tulips-isolated-on-260nw-1939095192.jpg" alt="Roses and Tulips">
            </div>
            <div class="giphy-container">
                <img src="https://media.giphy.com/media/3oriO0OEd9QIDdllqo/giphy.gif" alt="Cute Cat Holding Flowers and Balloon">
            </div>
            <p id="love-message">I love you so much!</p>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    background-color: #add8e6;
    text-align: center;
    font-family: 'Arial', sans-serif;
}

.container {
    padding: 20px;
    margin-top: 50px;
}

#birthday-cake {
    width: 200px;
    height: auto;
    margin-bottom: 20px;
}

button {
    background-color: #ff69b4;
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    border-radius: 5px;
}

button:hover {
    background-color: #ff1493;
}

#message-section {
    margin-top: 30px;
}

.hidden {
    display: none;
}

#love-message {
    color: red;
    font-size: 24px;
    margin-top: 20px;
}

.flowers img {
    width: 150px;
    height: auto;
}

.giphy-container img {
    width: 200px;
    height: auto;
    margin-top: 10px;
}
function makeAWish() {
    document.getElementById('cake-section').classList.add('hidden');
    document.getElementById('message-section').classList.remove('hidden');
}

