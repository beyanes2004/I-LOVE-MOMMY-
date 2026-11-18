
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Hola Mamacita ❤️</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    background:
        radial-gradient(circle at top, #34445b, transparent 55%),
        linear-gradient(145deg, #080d18, #172438, #0b101d);
    font-family: Georgia, serif;
    color: #f5ead3;
    text-align: center;
    overflow-x: hidden;
    padding: 35px 0;
}

.container {
    position: relative;
    z-index: 2;
    width: 90%;
    max-width: 520px;
    margin: auto;
    padding: 35px 24px;
    background: rgba(255,255,255,0.055);
    border: 1px solid rgba(220,190,130,0.4);
    border-radius: 25px;
    box-shadow: 0 15px 60px #00000080;
    backdrop-filter: blur(12px);
    animation: appear 1.5s ease;
}

.top-heart {
    font-size: 55px;
    margin-bottom: 15px;
    animation: heartbeat 1.5s infinite;
}

h1 {
    font-size: clamp(30px, 8vw, 43px);
    color: #e6c68c;
    letter-spacing: 2px;
    margin-bottom: 18px;
    text-shadow: 0 0 20px #e6c68c50;
}

.subtitle {
    font-size: 17px;
    color: #d9c9ac;
    line-height: 1.8;
    margin-bottom: 25px;
}

/* HER PICTURE */

.photo-frame {
    width: 100%;
    padding: 7px;
    margin: 20px auto 28px;
    border: 1px solid #d7b779;
    border-radius: 18px;
    background: #172438;
    box-shadow: 0 0 30px #d7b77930;
}

.photo {
    display: block;
    width: 100%;
    height: auto;
    max-height: 750px;
    object-fit: contain;
    border-radius: 12px;
}

/* MESSAGE */

.message {
    padding: 25px 12px;
    border-top: 1px solid #d7b77970;
    border-bottom: 1px solid #d7b77970;
}

.message h2 {
    font-size: 25px;
    color: #e6c68c;
    margin-bottom: 20px;
}

.message p {
    color: #f5ead3;
    font-size: 20px;
    line-height: 2;
}

.smile {
    font-size: 32px;
    margin-top: 18px;
}

/* BUTTON */

button {
    margin-top: 28px;
    padding: 15px 30px;
    border: 1px solid #e6c68c;
    border-radius: 30px;
    background: linear-gradient(135deg, #b18b50, #e4c68c);
    color: #111827;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
}

button:hover {
    transform: scale(1.06);
    box-shadow: 0 0 25px #e6c68c70;
}

/* SURPRISE */

#surprise {
    display: none;
    margin-top: 25px;
    color: #f5dfb3;
    font-size: 21px;
    line-height: 1.9;
    animation: appear 1s ease;
}

/* LAST MESSAGE */

.last {
    margin-top: 35px;
    padding-top: 25px;
    border-top: 1px solid #d7b77970;
}

.last h2 {
    font-size: 26px;
    color: #e6c68c;
    line-height: 1.6;
}

.last p {
    margin-top: 12px;
    color: #e9dcc5;
    font-size: 17px;
}

footer {
    margin-top: 30px;
    color: #bcae96;
    font-size: 14px;
}

/* FLOATING DECORATIONS */

.floating {
    position: fixed;
    bottom: -50px;
    pointer-events: none;
    z-index: 1;
    animation: float 9s linear infinite;
}

@keyframes heartbeat {
    50% {
        transform: scale(1.15);
    }
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes float {
    to {
        transform: translateY(-110vh) rotate(360deg);
    }
}
</style>
</head>

<body>

<div class="container">

    <div class="top-heart">❤️</div>

    <h1>HOLA MAMACITA</h1>

    <div class="subtitle">
        A little something for my favorite girl ✨
    </div>

    <div class="photo-frame">
        <img
            src="mamati.jpg"
            alt="My gorgeous girl"
            class="photo"
        >
    </div>

    <div class="message">

        <h2>MY BEAUTIFUL GIRL</h2>

        <p>
            I LOVE U SO MUCH ❤️
            <br>
            YOURE SO GORGEOUS
            <br>
            SMILEEEEE 🥹
        </p>

        <div class="smile">✨ ❤️ ✨</div>

    </div>

    <button onclick="showSurprise()">
        OPEN THIS FOR ME 💌
    </button>

    <div id="surprise">
        YOU DESERVE ALL THE LOVE
        <br>
        AND ALL THE HAPPINESS IN THE WORLD.
        <br><br>
        NEVER FORGET HOW SPECIAL YOU ARE.
        <br>
        MWAHHHHH 💋❤️
    </div>

    <div class="last">

        <h2>AND ONE LAST THING...</h2>

        <br>

        <h2>NICE ASS THO 😋</h2>

        <p>HAHAHAHA I LOVE YOUUU ❤️</p>

    </div>

    <footer>
        Made with love, just for you.
        <br><br>
        Forever yours ❤️
    </footer>

</div>

<script>

function showSurprise() {
    document.getElementById("surprise").style.display = "block";
}

const decorations = ["❤️", "✨", "🤍", "💫", "♥"];

for (let i = 0; i < 30; i++) {

    let item = document.createElement("div");

    item.className = "floating";

    item.innerHTML =
        decorations[Math.floor(Math.random() * decorations.length)];

    item.style.left = Math.random() * 100 + "vw";

    item.style.animationDuration =
        (6 + Math.random() * 8) + "s";

    item.style.animationDelay =
        Math.random() * 8 + "s";

    item.style.fontSize =
        (15 + Math.random() * 22) + "px";

    document.body.appendChild(item);
}

</script>

</body>
</html>
