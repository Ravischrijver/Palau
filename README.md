<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Palau Info Portal</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #eef2f3;
        }

        /* NAVBAR */
        nav {
            background: #005f73;
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }

        nav input {
            padding: 8px;
            border-radius: 5px;
            border: none;
            width: 200px;
        }

        /* SLIDER */
        .slider {
            position: relative;
            width: 100%;
            height: 70vh;
            overflow: hidden;
        }

        .slides {
            display: flex;
            width: 300%;
            height: 100%;
            animation: slide 15s infinite ease-in-out;
        }

        .slides img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        @keyframes slide {
            0% { transform: translateX(0%); }
            33% { transform: translateX(-100%); }
            66% { transform: translateX(-200%); }
            100% { transform: translateX(0%); }
        }

        /* CONTENT */
        section {
            padding: 40px 20px;
            max-width: 900px;
            margin: auto;
        }

        h2 {
            color: #005f73;
        }

        /* AI CHAT */
        #chatbox {
            background: white;
            padding: 20px;
            border-radius: 10px;
            margin-top: 40px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        #chatlog {
            height: 200px;
            overflow-y: auto;
            border: 1px solid #ccc;
            padding: 10px;
            margin-bottom: 15px;
            background: #fafafa;
        }

        #chatlog p {
            margin: 5px 0;
        }

        #chatinput {
            width: 80%;
            padding: 10px;
        }

        #sendbtn {
            padding: 10px 15px;
            background: #005f73;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
</head>

<body>

<!-- NAVBAR -->
<nav>
    <div>
        <a href="#home">Home</a>
        <a href="#info">Info</a>
        <a href="#ai">AI Chat</a>
    </div>
    <input id="search" type="text" placeholder="Zoek info...">
</nav>

<!-- SLIDER -->
<div class="slider" id="home">
    <div class="slides">
        <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e">
        <img src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21">
        <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470">
    </div>
</div>

<!-- INFO SECTION -->
<section id="info">
    <h2>Over Palau</h2>
    <p class="infoblock">
        Palau is een eilandstaat in Micronesië, bekend om zijn kristalheldere wateren, koraalriffen en unieke natuur.
    </p>

    <h2>Natuur</h2>
    <p class="infoblock">
        De Rock Islands zijn een UNESCO-werelderfgoedlocatie en behoren tot de mooiste natuurgebieden ter wereld.
    </p>

    <h2>Duiken</h2>
    <p class="infoblock">
        Palau is een topbestemming voor duikers, met plekken zoals Blue Corner, German Channel en Jellyfish Lake.
    </p>

    <h2>Cultuur</h2>
    <p class="infoblock">
        De Palause cultuur draait om gemeenschap, traditie en respect voor de natuur. Traditionele Bai-huizen zijn iconisch.
    </p>
</section>

<!-- AI CHAT -->
<section id="ai">
    <h2>Vraag de AI over Palau</h2>

    <div id="chatbox">
        <div id="chatlog"></div>

        <input id="chatinput" type="text" placeholder="Stel een vraag over Palau...">
        <button id="sendbtn">Verstuur</button>
    </div>
</section>

<script>
/* --- ZOEKFUNCTIE --- */
document.getElementById("search").addEventListener("input", function() {
    const q = this.value.toLowerCase();
    document.querySelectorAll(".infoblock").forEach(block => {
        block.style.display = block.textContent.toLowerCase().includes(q) ? "block" : "none";
    });
});

/* --- AI CHAT --- */
document.getElementById("sendbtn").onclick = async function() {
    const input = document.getElementById("chatinput").value;
    if (!input) return;

    const log = document.getElementById("chatlog");
    log.innerHTML += `<p><b>Jij:</b> ${input}</p>`;

    const response = await fetch("https://api.openai.com/v1/chat/completions", {
        method: "POST",
        headers: {
            "Content-Type": "application/json",
            "Authorization": "bearer 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"
        },
        body: JSON.stringify({
            model: "gpt-3.5-turbo",
            messages: [{ role: "user", content: input }]
        })
    });

    const data = await response.json();
    const answer = data.choices[0].message.content;

    log.innerHTML += `<p><b>AI:</b> ${answer}</p>`;
    document.getElementById("chatinput").value = "";
    log.scrollTop = log.scrollHeight;
};
</script>

</body>
</html>
