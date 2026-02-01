<!DOCTYPE html>
100% { transform: translateY(0); }
}
</style>
</head>
<body>


<section>
<div class="card">
<h1>Happy Valentine’s Day My Dearest Boyfriend 💖</h1>
<h2>To My Beloved Hazey (aka Henry, aka Phone Hein Htet)</h2>
<p>You make my days brighter, my laughs louder, and my heart fuller.</p>
<div class="heart">❤️</div>
</div>


<div class="card">
<h2>How much do you love me?</h2>
<input type="range" min="0" max="100" value="50" id="loveSlider" />
<p id="loveValue">50%</p>
</div>


<div class="card">
<h2>Mini Quiz 💌</h2>
<p>What do you love most about us?</p>
<button onclick="answer('Everything 😌')">Everything 😌</button>
<button onclick="answer('Your smile 🥺')">Your smile 🥺</button>
<button onclick="answer('Our memories 💭')">Our memories 💭</button>
<p id="quizResult"></p>
</div>


<div class="card">
<h2>One Last Question…</h2>
<p>Will you be my Valentine?</p>
<button onclick="yesAnswer()">Yes 💕</button>
<button onclick="noAnswer()">No 🙃</button>
<p id="finalAnswer"></p>
</div>
</section>


<script>
const slider = document.getElementById('loveSlider');
const output = document.getElementById('loveValue');
output.innerHTML = slider.value + "%";


slider.oninput = function() {
output.innerHTML = this.value + "%";
}


function answer(text) {
document.getElementById('quizResult').innerText = "Aww 🥹 I love that you chose: " + text;
}


function yesAnswer() {
document.getElementById('finalAnswer').innerText = "YAY!! 💖 I love you, Hazey.";
}


function noAnswer() {
document.getElementById('finalAnswer').innerText = "That button was just for decoration 😌";
}
</script>


</body>
</html>
