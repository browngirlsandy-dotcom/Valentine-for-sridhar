<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Sridhar Nishant ❤️</title>

<style>
body {
  margin: 0;
  height: 100vh;
  background: linear-gradient(135deg, #ff758c, #ff7eb3);
  font-family: 'Courier New', monospace;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

/* Floating hearts */
.heart {
  position: fixed;
  bottom: -20px;
  font-size: 20px;
  animation: floatUp 6s linear infinite;
}
@keyframes floatUp {
  0% { transform: translateY(0); opacity: 1; }
  100% { transform: translateY(-100vh); opacity: 0; }
}

.card {
  background: white;
  padding: 30px;
  border-radius: 22px;
  text-align: center;
  box-shadow: 0 25px 50px rgba(0,0,0,0.35);
  max-width: 440px;
  z-index: 2;
}

h1 { color: #e63946; }
h3 { color: #e63946; }

.msg {
  font-size: 14px;
  color: #444;
  margin: 12px 0;
}

.countdown {
  margin: 15px 0;
  font-size: 14px;
  color: #e63946;
  font-weight: bold;
}

button {
  padding: 10px 24px;
  font-size: 16px;
  border: none;
  border-radius: 10px;
  cursor: pointer;
  margin: 10px;
}

.yes {
  background: #e63946;
  color: white;
}

.no {
  background: #adb5bd;
  color: white;
  position: absolute;
}

.signature {
  margin-top: 15px;
  font-size: 13px;
  color: #777;
}

audio { display: none; }
</style>
</head>

<body>

<!-- 🎵 Background Music -->
<audio autoplay loop>
  <source src="https://www.dropbox.com/scl/fi/8gk0y0e2h4m9x7zqk7z8e/Perfect-Ed-Sheeran.mp3?raw=1" type="audio/mpeg">
</audio>

<div class="card">
  <h1>💌 Hey Sridhar Nishant 💌</h1>

  <p>
    if (distance > 0) { <br>
    &nbsp;&nbsp;missYou++; <br>
    &nbsp;&nbsp;love *= infinity; <br>
    } <br>
    myForever = <b>you</b>;
  </p>

  <div class="msg">
    “I love you soo much my cutee handsome babyyyy ❤️🎉✨️  
    <br>counting dayss until we meet again 🫂💋💌”
  </div>

  <div class="countdown" id="countdown"></div>

  <h3>Will you be my Valentine? 🥺❤️</h3>

  <button class="yes" onclick="yesClicked()">YES 💖</button>
  <button class="no" onmouseover="moveButton(this)">NO 😜</button>

  <div class="signature">
    — Yours always,<br>
    <b>Sandhya Kumari Sharma 💌💋✨️</b>
  </div>
</div>

<script>
/* Floating hearts */
setInterval(() => {
  const heart = document.createElement("div");
  heart.className = "heart";
  heart.innerHTML = "💖";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.animationDuration = (Math.random() * 3 + 4) + "s";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 6000);
}, 400);

/* NO button runs away */
function moveButton(btn) {
  btn.style.top = Math.random() * 80 + "vh";
  btn.style.left = Math.random() * 80 + "vw";
}

/* YES click */
function yesClicked() {
  document.body.innerHTML = `
    <h1 style="color:white; text-align:center; padding:40px;">
      🎉 PERFECT TOGETHER 🎉<br><br>
      Sridhar Nishant ❤️<br>
      You are officially my Valentine 🫶<br><br>
      Distance doesn’t matter,<br>
      hearts already merged 💞♾️<br><br>
      <small>— Sandhya Kumari Sharma 💌</small>
    </h1>`;
}

/* Countdown (SET YOUR MEETING DATE HERE) */
const meetDate = new Date("2026-03-20"); // change if needed
const countdownEl = document.getElementById("countdown");

setInterval(() => {
  const now = new Date();
  const diff = meetDate - now;

  if (diff > 0) {
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    countdownEl.innerHTML = `⏳ ${days} days left until we meet 🫂`;
  } else {
    countdownEl.innerHTML = "🫂 Today we meet ❤️";
  }
}, 1000);
</script>

</body>
</html>
