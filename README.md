# Happy-birthday-<!DOCTYPE html>
<html>
<head>
<title>Happy Birthday</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  font-family: Arial;
  text-align: center;
  background: linear-gradient(to right, #ff758c, #ff7eb3);
  color: white;
}

.section {
  padding: 50px 20px;
}

.card {
  background: white;
  color: black;
  padding: 20px;
  margin: 20px;
  border-radius: 15px;
}

img {
  width: 200px;
  border-radius: 15px;
  margin: 10px;
}

button {
  background: purple;
  color: white;
  padding: 12px 25px;
  border: none;
  border-radius: 10px;
  font-size: 16px;
}

#countdown {
  font-size: 30px;
  margin-top: 20px;
}
</style>
</head>

<body>

<div class="section">
<h1>🎂 Happy Birthday My Love 🎂</h1>
<p>You are the most special person in my life ❤️</p>
<button onclick="showMessage()">Click Here</button>
</div>

<div class="section card">
<h2>💌 Birthday Letter</h2>
<p>
Happy Birthday! <br>
I wish you lots of happiness, success and love. <br>
You are very special for me and always will be. ❤️
</p>
</div>

<div class="section">
<h2>📸 Our Memories</h2>
<img src="photo1.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">
</div>

<div class="section">
<h2>🎵 Your Song</h2>
<audio controls>
  <source src="song.mp3" type="audio/mpeg">
</audio>
</div>

<div class="section">
<h2>⏳ Countdown</h2>
<div id="countdown"></div>
</div>

<script>
function showMessage() {
  alert("I Love You So Much ❤️");
}

// Countdown Timer
var countDate = new Date("April 10, 2026 00:00:00").getTime();

var x = setInterval(function() {
  var now = new Date().getTime();
  var gap = countDate - now;

  var days = Math.floor(gap / (1000 * 60 * 60 * 24));
  var hours = Math.floor((gap % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((gap % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((gap % (1000 * 60)) / 1000);

  document.getElementById("countdown").innerHTML =
    days + "d " + hours + "h " + minutes + "m " + seconds + "s ";
}, 1000);
</script>

</body>
</html>
