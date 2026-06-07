<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Mithi ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#ff9a9e,#fad0c4);
min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
overflow:hidden;
padding:20px;
}

.card{
width:100%;
max-width:800px;
background:rgba(255,255,255,0.18);
backdrop-filter:blur(15px);
border-radius:25px;
padding:35px;
text-align:center;
color:white;
box-shadow:0 8px 32px rgba(0,0,0,0.15);
animation:fadeIn 1s;
}

h1,h2{
margin-bottom:20px;
}

p{
line-height:1.8;
font-size:18px;
}

button{
margin-top:25px;
padding:14px 30px;
border:none;
border-radius:50px;
background:white;
color:#ff4f81;
font-size:18px;
font-weight:bold;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.05);
}

.hidden{
display:none;
}

@keyframes fadeIn{
from{
opacity:0;
transform:translateY(20px);
}
to{
opacity:1;
transform:translateY(0);
}
}

.heart{
position:fixed;
bottom:-20px;
font-size:20px;
animation:float 8s linear infinite;
opacity:.6;
}

@keyframes float{
from{
transform:translateY(0);
}
to{
transform:translateY(-110vh);
}
}

.footer{
margin-top:25px;
font-style:italic;
opacity:.9;
}
</style>
</head>

<body>

<div class="card">

<div id="screen1">
<h1>🎂 Happy Birthday Mithi! 💖</h1>
<p>Today is all about celebrating you ✨</p>
<button onclick="nextScreen(1)">Tap Here ✨</button>
</div>

<div id="screen2" class="hidden">
<h2>🌸 Before you start your special day...</h2>
<p>Just a small birthday surprise waiting for you 💕</p>
<button onclick="nextScreen(2)">Next 💌</button>
</div>

<div id="screen3" class="hidden">
<h2>🎁 A Small Birthday Surprise</h2>
<p>For one of my favorite people ❤️</p>
<button onclick="nextScreen(3)">Open Message 🎂</button>
</div>

<div id="screen4" class="hidden">
<h2>💖 A Special Message For You 💖</h2>

<p>

Happy Birthday Mithi! 🎂💖

<br><br>

Pata nahi kaise thank you bolu, but sach me meri life ka ek important part banne ke liye thank you.
Har choti-badi baat share karne ke liye, meri bakwaas sunne ke liye, aur har situation me saath dene ke liye thank you.

<br><br>

Bahut log milte hain zindagi me, lekin har kisi ke saath itna comfort aur trust nahi banta.
Tu sirf meri best friend nahi, balki un logon me se hai jinke saath main bina kisi hesitation ke apni baatein share kar sakta hu.

<br><br>

Chahe hum hase ho, mazaak kiya ho, ya kisi difficult time se guzre ho,
har memory mere liye special hai.

<br><br>

Main bas itna chahta hu ki tu hamesha khush rahe, smile karti rahe aur jo bhi sapne dekhe hain wo sab pure ho.

<br><br>

Thank you for being such an amazing best friend. ❤️

<br><br>

Once again, Happy Birthday Mithi! 🎉✨

</p>

<div class="footer">
✨ For someone who made ordinary days a little better ✨
</div>

</div>

</div>

<script>

function nextScreen(step){
document.getElementById("screen"+step).classList.add("hidden");
document.getElementById("screen"+(step+1)).classList.remove("hidden");
}

for(let i=0;i<30;i++){
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="🤍";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(15+Math.random()*20)+"px";
heart.style.animationDuration=(5+Math.random()*5)+"s";
document.body.appendChild(heart);
}

</script>

</body>
</html>
