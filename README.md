<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Valentine’s Day Hazey ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      color: #4a1c1c;
      text-align: center;
    }
    section {
      padding: 60px 20px;
      max-width: 800px;
      margin: auto;
    }
    h1, h2 {
      margin-bottom: 20px;
    }
    .card {
      background: rgba(255, 255, 255, 0.85);
      border-radius: 20px;
      padding: 30px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      margin-bottom: 40px;
    }
    button {
      padding: 12px 25px;
      border: none;
      border-radius: 30px;
      background: #ff4d6d;
      color: white;
      font-size: 1rem;
      cursor: pointer;
      transition: transform 0.2s, background 0.2s;
    }
    button:hover {
      background: #e63950;
      transform: scale(1.05);
    }
    input[type="range"] {
      width: 80%;
    }
    .hidden {
      display: none;
    }
    .heart {
      font-size: 2rem;
      animation: float 2s infinite ease-in-out;
    }
    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }
  </style>
</head>
<body>

  <section>
    <div class="card">
      <h1>Happy Valentine’s Day My Dearest Boyfriend 💖</h1>
      <h2>To my beloved Hazey (aka Henry, aka Phone Hein Htet)</h2>
      <p>Firstly, I want to greet my loveliest boyfriend and my future husband Hazey, Henry or Phone Hein Htet~ happy Valentine’s dayyy! I just want you to know how much you mean to me and I would be so happy if this little surprise or gift can bring a smile on your face~</p>
      <p>To love you is one of the easiest things to do, Hazey. In my eyes, you’re one of the most wonderful people I’ve ever met, and that’s why I wish I’d be able to keep you for as long as I could. You are my love, my best friend, my one and only, and I really love youuuu~</p>
      <p>Meeting you is one of the luckiest things that happened in my life. It’s still so magical and dreamy when I think about it again — how we met at a competition, how we noticed each other before the last moment possible. Heheh… I guess only serendipity can explain this. I’d love to thank the 4x4 Rubik’s cube for being the “wing man” that made you notice me 😁.</p>
      <p>I am so grateful for all the happiness you’ve brought into my life. Thank you for loving me and for not leaving me even during the times when I act like I don’t love you. You are my motivation, the fuel that pushes me to be a better version of myself. I want to be better, and even better, just to be with you~</p>
      <p>I love how you always understand and respect my choices. You’re my biggest supporter, my backbone, someone I can always rely on when I’m tired. You’re thoughtful, understanding, and you never judge me. You’re bright, optimistic, and the sunshine of my life.</p>
      <p>You have the most beautiful eyes that I could stare at forever, especially when they’re smiling. Your voice is so soothing, gentle, and charming — and sooooo cute to me. I wish I could hear it and see your smile for the rest of my life.</p>
      <p>You’re sooo damn cool, my sweetheart — especially when you play War Thunder. I love watching you stream your gameplay and hearing you yap about tanks and planes. I’m always impressed by how much you know, and I genuinely enjoy every moment.</p>
      <p>It’s still magical to me how quickly you earned my trust. I never regret confessing to you. I’m so glad I get to be your first French kiss — kissing you is something I want to do forever. Ah… I want to kiss you so bad right now…</p>
      <p>At last, I just want to say this: Hazey — my beloved, my honey, my sweetheart, my significant other, my loveliest, my dearest, my darling, my cutest boy — you are wonderful for at least 100 more reasons, and I love you for at least 100 more reasons. If I wrote them all out, it would be a few-thousand-words essay, hehe~</p>
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
