<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Yumyum-v3t on yt!</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
/* 🌸 BODY + DESKTOP BACKGROUND */
body {
    margin:0;
    font-family:"Comic Sans MS",cursive;
    cursor:url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEgOEg1TDEgMTIiIHN0cm9rZT0iI2ZmY2JmZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiLz4KPC9zdmc+'), auto;
    background-size:cover;
    transition: background 1s ease-in-out;
}

/* 🌸 DESKTOP WINDOWS */
.window {
    position:absolute;
    background: rgba(255,255,255,0.85);
    border-radius: 15px;
    padding: 15px;
    border: 2px solid #ffc2e2;
    box-shadow: 0 5px 15px rgba(0,0,0,0.15);
    cursor: grab;
    transition: transform 0.3s, box-shadow 0.3s;
}
.window:hover { transform: scale(1.03); box-shadow:0 10px 25px rgba(0,0,0,0.2); }

/* 🌸 HEADER */
header {
    text-align:center;
    padding:30px;
    background: rgba(255,255,255,0.6);
    backdrop-filter: blur(10px);
    border-bottom: 3px dashed #ffc2e2;
}
h1 { font-size:2.5em; color:#ff8acb; }
.tagline { color:#a38bff; font-size:1.2em; }

/* 🌸 HEARTS & SPARKLES */
.heart{position:fixed;color:pink;animation:floatUp 3s linear forwards;}
@keyframes floatUp{0%{transform:translateY(0);opacity:1}100%{transform:translateY(-200px);opacity:0}}
.sparkle{position:absolute;width:8px;height:8px;background:white;border-radius:50%;pointer-events:none;animation:sparkleAnim 1s forwards}
@keyframes sparkleAnim{to{transform:scale(2);opacity:0}}

/* 🌸 EASTER EGGS */
.easter{display:inline-block;width:20px;height:20px;}

/* 🌸 MESSAGE */
#message{font-weight:bold;color:#ff7fbc;margin-top:10px;font-size:1.1em;}

button{background:#ffb3e6;border:none;padding:10px 20px;border-radius:15px;cursor:pointer;font-family:inherit;margin-top:10px;}
button:hover{background:#ffa3db;}
</style>
</head>
<body>

<header>
<h1>🌸 Yumyum-v3t on yt! 🌸</h1>
<p class="tagline">✨ KNY edits • cute vibes • anime lover ✨</p>
</header>

<!-- WINDOWS -->
<div class="window" id="aboutWin" style="top:100px;left:50px;width:250px;">
<h2>💗 About Me</h2>
<p>Hi!! I'm Yumyum-v3t 💕 I love making cute edits and KNY content ⚔️🌸</p>
<p>Click hearts for secret messages!</p>
</div>

<div class="window" id="musicWin" style="top:150px;left:350px;width:300px;">
<h2>🎶 Music Player</h2>
<p>Soft intro + RUDE! vibes 😆</p>
<button onclick="toggleMusic()">Play / Pause 🎧</button>
<iframe id="ytMusic" width="100%" height="80" src="https://www.youtube.com/embed/0eoNKfG4fX4?autoplay=0" title="RUDE! Music" frameborder="0" allow="autoplay; encrypted-media"></iframe>
</div>

<div class="window" id="ytWin" style="top:200px;left:700px;width:250px;">
<h2>🎥 My YouTube</h2>
<p><b>Yumyum-v3t on yt!</b></p>
<button onclick="subscribe()">Subscribe 💗</button>
</div>

<div class="window" id="interactiveWin" style="top:400px;left:200px;width:280px;">
<h2>✨ Interactive Button</h2>
<p>Press for a cute message 💬</p>
<button onclick="showMessage()">Click me 💕</button>
<p id="message"></p>
</div>

<div class="window" id="eggWin" style="top:450px;left:600px;width:230px;">
<h2>👀 Easter Egg</h2>
<p>Hover over this pink dot → <span class="easter" onclick="secret()">💖</span></p>
</div>

<footer style="position:fixed;bottom:0;width:100%;text-align:center;color:#888;">🌸 Made with love + pastel desktop vibes 🌸</footer>

<script>
// MUSIC
let playing=false;
function toggleMusic(){
    const frame=document.getElementById("ytMusic");
    const url = frame.src;
    if(!playing){ frame.src = url.replace("autoplay=0","autoplay=1"); playing=true; }
    else{ frame.src = url.replace("autoplay=1","autoplay=0"); playing=false; }
}

// MESSAGE
function showMessage(){
    const msgs=["You're amazing 💖","Keep editing!! 🎬","KNY forever ⚔️","Stay cute!! 🌸","YT superstar incoming 💗"];
    document.getElementById("message").innerText=msgs[Math.floor(Math.random()*msgs.length)];
}

// SUBSCRIBE
function subscribe(){ alert("TYSM FOR SUPPORTING 💕😭"); }

// HEARTS + SPARKLES
document.addEventListener("click",function(e){
    const heart=document.createElement("div");
    heart.className="heart"; heart.innerText="💗";
    heart.style.left=e.clientX+"px"; heart.style.top=e.clientY+"px";
    document.body.appendChild(heart);
    setTimeout(()=>heart.remove(),3000);
    for(let i=0;i<5;i++){
        const s=document.createElement("div"); s.className="sparkle";
        s.style.left=e.clientX+"px"; s.style.top=e.clientY+"px";
        document.body.appendChild(s); setTimeout(()=>s.remove(),1000);
    }
});

// EASTER EGG
function secret(){ alert("You found a secret heart!! 💖✨"); }

// ROTATING BACKGROUNDS
const bgImages=[
'https://i.imgur.com/FZ4rBHz.jpg',
'https://i.imgur.com/xfw2zKq.jpg',
'https://i.imgur.com/LWcER1T.jpg'
];
let bgIndex=0;
function rotateBackground(){
    document.body.style.background=`url(${bgImages[bgIndex]}) no-repeat center center fixed`;
    document.body.style.backgroundSize='cover';
    bgIndex=(bgIndex+1)%bgImages.length;
}
setInterval(rotateBackground,10000);

// DRAGGABLE WINDOWS
let dragItem=null;
let offsetX=0, offsetY=0;
document.querySelectorAll('.window').forEach(win=>{
    win.onmousedown=function(e){
        dragItem=win;
        offsetX=e.clientX-win.offsetLeft;
        offsetY=e.clientY-win.offsetTop;
        win.style.cursor="grabbing";
    }
});
document.onmouseup=function(){ if(dragItem){ dragItem.style.cursor="grab"; dragItem=null; }}
document.onmousemove=function(e){
    if(dragItem){
        dragItem.style.left=(e.clientX-offsetX)+'px';
        dragItem.style.top=(e.clientY-offsetY)+'px';
    }
}
</script>

</body>
</html><!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Yumyum-v3t on yt!</title>

<style>
body{
margin:0;
font-family:cursive;
background:linear-gradient(135deg,#ffd6f6,#d6faff,#e6d6ff);
overflow:hidden;
transition:0.5s;
}

/* WINDOWS */
.window{
position:absolute;
background:white;
border-radius:15px;
padding:15px;
border:2px solid pink;
box-shadow:0 5px 15px rgba(0,0,0,0.2);
cursor:grab;
}

/* BUTTON */
button{
background:#ffb3e6;
border:none;
padding:8px;
border-radius:10px;
cursor:pointer;
}

/* FLOATING */
.float{position:fixed;animation:floatUp 6s linear infinite;}
@keyframes floatUp{0%{transform:translateY(100vh)}100%{transform:translateY(-10vh)}}

/* CURSOR TRAIL */
.trail{position:absolute;pointer-events:none;animation:fade 1s forwards;}
@keyframes fade{to{opacity:0;transform:scale(2);}}

/* CHIBI */
#chibi{
position:fixed;
bottom:0;
left:0;
font-size:40px;
animation:walk 10s linear infinite;
}
@keyframes walk{
0%{left:0;}
50%{left:80%;}
100%{left:0;}
}

/* NIGHT MODE */
.dark{
background:linear-gradient(135deg,#2a003f,#000);
color:white;
}
</style>
</head>

<body>

<h1 style="text-align:center;color:#ff8acb;">🌸 Yumyum-v3t on yt! 🌸</h1>

<!-- CLICKER GAME -->
<div class="window" style="top:80px;left:40px;">
<h2>💗 Heart Clicker</h2>
<p>Hearts: <span id="hearts">0</span></p>
<button onclick="addHeart()">Click 💖</button>
</div>

<!-- COOKING -->
<div class="window" style="top:200px;left:250px;">
<h2>🍓 Cooking</h2>
<button onclick="cook()">Make Dessert</button>
<p id="food"></p>
</div>

<!-- DRESS -->
<div class="window" style="top:350px;left:500px;">
<h2>🎀 Dress Up</h2>
<p id="outfit">Outfit: Basic</p>
<button onclick="dress()">Change</button>
</div>

<!-- MUSIC -->
<div class="window" style="top:150px;left:700px;">
<h2>🎵 Music</h2>
<iframe width="200" height="100"
src="https://www.youtube.com/embed/0eoNKfG4fX4"
allow="autoplay"></iframe>
</div>

<!-- TOGGLE -->
<div class="window" style="top:400px;left:800px;">
<h2>🌙 Mode</h2>
<button onclick="toggleMode()">Toggle</button>
</div>

<!-- CHIBI -->
<div id="chibi">🐰</div>

<script>
// CLICKER
let hearts=0;
function addHeart(){
hearts++;
document.getElementById("hearts").innerText=hearts;
}

// COOKING
function cook(){
const foods=["Mochi 🍓","Magic Cake ✨","Jelly 🌈","CHAOS 😭"];
document.getElementById("food").innerText=
foods[Math.floor(Math.random()*foods.length)];
}

// DRESS
function dress(){
const outfits=["Princess 👑","Magical ✨","Goth 🎀","Slayer ⚔️"];
document.getElementById("outfit").innerText=
"Outfit: "+outfits[Math.floor(Math.random()*outfits.length)];
}

// MODE
function toggleMode(){
document.body.classList.toggle("dark");
}

// FLOATING
setInterval(()=>{
let e=document.createElement("div");
e.className="float";
e.innerText=["💖","✨","🎀","🌸"][Math.floor(Math.random()*4)];
e.style.left=Math.random()*100+"vw";
document.body.appendChild(e);
setTimeout(()=>e.remove(),6000);
},500);

// TRAIL
document.addEventListener("mousemove",e=>{
let t=document.createElement("div");
t.className="trail";
t.innerText="✨";
t.style.left=e.pageX+"px";
t.style.top=e.pageY+"px";
document.body.appendChild(t);
setTimeout(()=>t.remove(),1000);
});

// DRAG
let drag=null,ox,oy;
document.querySelectorAll('.window').forEach(w=>{
w.onmousedown=e=>{
drag=w;ox=e.clientX-w.offsetLeft;oy=e.clientY-w.offsetTop;}
});
document.onmouseup=()=>drag=null;
document.onmousemove=e=>{
if(drag){
drag.style.left=(e.clientX-ox)+'px';
drag.style.top=(e.clientY-oy)+'px';
}
}
</script>

</body>
</html><!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Yumyum-v3t on yt!</title>

<style>
body{
margin:0;
font-family:cursive;
background:linear-gradient(135deg,#ffd6f6,#d6faff,#e6d6ff);
overflow:hidden;
}

/* CUTENESS OVERLOAD */
.star,.bow{
position:fixed;
animation:float 6s linear infinite;
}
@keyframes float{
0%{transform:translateY(100vh)}
100%{transform:translateY(-10vh)}
}

/* WINDOWS */
.window{
position:absolute;
background:white;
border-radius:15px;
padding:15px;
border:2px solid pink;
}

/* BUTTON */
button{
background:pink;
border:none;
padding:10px;
border-radius:10px;
cursor:pointer;
}

/* GAME */
#result{
margin-top:10px;
color:#ff69b4;
font-weight:bold;
}
</style>
</head>

<body>

<h1>🌸 Yumyum-v3t on yt! 🌸</h1>

<!-- MADOKA SECTION -->
<div class="window" style="top:100px;left:50px;">
<h2>🩷 Madoka Magic</h2>
<p>Magical girl vibes forever ✨</p>
<p>"Even miracles have a cost..."</p>
</div>

<!-- COOKING GAME -->
<div class="window" style="top:200px;left:300px;">
<h2>🍓 Cute Cooking Game</h2>
<p>Pick ingredients!</p>

<button onclick="cook('strawberry')">🍓</button>
<button onclick="cook('chocolate')">🍫</button>
<button onclick="cook('milk')">🥛</button>

<p id="result"></p>
</div>

<script>
// COOKING GAME
function cook(item){
const foods=[
"Strawberry Mochi 🍓",
"Magical Cupcake ✨",
"Chocolate Dream Cake 🍫",
"Chaos Dessert 😭"
];
document.getElementById("result").innerText=
foods[Math.floor(Math.random()*foods.length)];
}

// FLOATING CUTENESS
setInterval(()=>{
let star=document.createElement("div");
star.className="star";
star.innerText="✨";
star.style.left=Math.random()*100+"vw";
document.body.appendChild(star);
setTimeout(()=>star.remove(),6000);
},500);
</script>

</body>
</html>
