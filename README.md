<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Palau – Complete Encyclopedie</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #eef2f3;
        }

        /* NAVBAR */
        nav {
            background: #005f73;
            padding: 12px 18px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav .links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
            font-weight: bold;
            font-size: 14px;
        }

        nav input {
            padding: 6px 8px;
            border-radius: 5px;
            border: none;
            width: 190px;
            font-size: 14px;
        }

        /* SLIDER */
        .slider {
            position: relative;
            width: 100%;
            height: 60vh;
            overflow: hidden;
        }

        .slides {
            display: flex;
            width: 300%;
            height: 100%;
            animation: slide 18s infinite ease-in-out;
        }

        .slides img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        @keyframes slide {
            0% { transform: translateX(0%); }
            30% { transform: translateX(0%); }
            35% { transform: translateX(-100%); }
            65% { transform: translateX(-100%); }
            70% { transform: translateX(-200%); }
            95% { transform: translateX(-200%); }
            100% { transform: translateX(0%); }
        }

        /* CONTENT */
        main {
            max-width: 1000px;
            margin: auto;
            padding: 20px;
        }

        section {
            margin: 35px 0;
            padding: 20px;
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 0 8px rgba(0,0,0,0.05);
        }

        h2 {
            color: #005f73;
            margin-top: 0;
        }

        h3 {
            color: #0a9396;
            margin-bottom: 5px;
        }

        .infoblock {
            margin-bottom: 18px;
            line-height: 1.6;
            font-size: 15px;
        }

        ul {
            margin-top: 5px;
            margin-bottom: 10px;
            padding-left: 20px;
        }

        .tag {
            display: inline-block;
            background: #e0fbfc;
            color: #005f73;
            padding: 2px 6px;
            border-radius: 4px;
            font-size: 11px;
            margin-right: 4px;
            margin-bottom: 4px;
        }

        @media (max-width: 768px) {
            nav .links {
                display: none;
            }
            .slider {
                height: 45vh;
            }
            main {
                padding: 10px;
            }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->
<nav>
    <div class="links">
        <a href="#algemeen">Algemeen</a>
        <a href="#geografie">Geografie</a>
        <a href="#geschiedenis">Geschiedenis</a>
        <a href="#politiek">Politiek</a>
        <a href="#economie">Economie</a>
        <a href="#natuur">Natuur</a>
        <a href="#duiken">Duiken</a>
        <a href="#cultuur">Cultuur</a>
        <a href="#toerisme">Toerisme</a>
    </div>
    <input id="search" type="text" placeholder="Zoek in alle info...">
</nav>

<!-- SLIDER -->
<div class="slider" id="home">
    <div class="slides">
        <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e" alt="Strand Palau">
        <img src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21" alt="Lagune Palau">
        <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470" alt="Eilanden Palau">
    </div>
</div>

<main>

<!-- ALGEMEEN -->
<section id="algemeen">
    <h2>Algemene informatie over Palau</h2>

    <p class="infoblock">
        <span class="tag">Land</span><span class="tag">Oceanië</span><span class="tag">Micronesië</span>
        Palau (officieel: Republiek Palau) is een eilandstaat in de westelijke Stille Oceaan, in de regio Micronesië.
        Het land bestaat uit ongeveer 340 eilanden, waarvan er maar een deel bewoond is. De hoofdstad is Ngerulmud,
        op het eiland Babeldaob. De grootste stad en economische kern is Koror.
    </p>

    <p class="infoblock">
        Palau heeft ongeveer 18.000–20.000 inwoners. De officiële talen zijn Palauaans en Engels; in sommige staten
        zijn ook Sonsorolese, Tobiaans en Japans erkende talen. De munteenheid is de Amerikaanse dollar (USD).
    </p>

    <p class="infoblock">
        Palau is een onafhankelijke staat, maar heeft een Compact of Free Association met de Verenigde Staten:
        de VS zijn verantwoordelijk voor defensie en bieden economische steun, terwijl Palau intern zelfstandig is.
    </p>
</section>

<!-- GEOGRAFIE -->
<section id="geografie">
    <h2>Geografie & eilanden</h2>

    <p class="infoblock">
        Palau ligt in de westelijke Stille Oceaan, ten oosten van de Filipijnen en ten noorden van Indonesië.
        Het land heeft een totale landoppervlakte van ongeveer 460 km² en een kustlijn van meer dan 1.500 km.
        Het bestaat uit een boog van eilanden langs de Kyushu‑Palau‑rug.
    </p>

    <p class="infoblock">
        Belangrijke eilanden en eilandgroepen:
        <ul>
            <li><b>Babeldaob</b> – grootste eiland, locatie van de hoofdstad Ngerulmud</li>
            <li><b>Koror</b> – voormalige hoofdstad, economisch centrum, meeste inwoners</li>
            <li><b>Peleliu</b> – bekend door zware gevechten in de Tweede Wereldoorlog</li>
            <li><b>Angaur</b> – klein eiland, vroeger fosfaatwinning</li>
            <li><b>Rock Islands</b> – honderden kalkstenen eilandjes, UNESCO‑werelderfgoed</li>
            <li><b>Kayangel</b> – atol in het noorden</li>
            <li><b>Sonsorol & Hatohobei</b> – zuidelijke, afgelegen eilanden</li>
        </ul>
    </p>

    <p class="infoblock">
        Het landschap varieert van dichte tropische bossen en mangroven tot lagunes, koraalriffen en steile
        kalksteenformaties. De hoogste natuurlijke punt is Mount Ngerchelchuus (circa 242 meter) op Babeldaob.
    </p>
</section>

<!-- KLIMAAT -->
<section id="klimaat">
    <h2>Klimaat & weer</h2>

    <p class="infoblock">
        Palau heeft een tropisch regenwoudklimaat met het hele jaar door warme temperaturen, meestal tussen 27 en 30 °C.
        De luchtvochtigheid is hoog en er valt veel neerslag, gemiddeld rond de 3.000–3.500 mm per jaar.
    </p>

    <p class="infoblock">
        Er is geen strikte scheiding tussen een droog en een regenseizoen, maar de meeste regen valt vaak tussen
        juni en oktober. Palau ligt aan de rand van het tyfoongebied; zware stormen zijn mogelijk, maar minder
        frequent dan in sommige andere delen van de westelijke Stille Oceaan.
    </p>
</section>

<!-- GESCHIEDENIS -->
<section id="geschiedenis">
    <h2>Geschiedenis</h2>

    <p class="infoblock">
        De eerste bewoners van Palau arriveerden waarschijnlijk duizenden jaren geleden uit andere delen van
        Micronesië en Zuidoost‑Azië. Er ontwikkelden zich eigen talen, tradities en sociale structuren.
    </p>

    <p class="infoblock">
        Europese contacten begonnen in de 16e–18e eeuw met Spaanse ontdekkingsreizigers. Later werd Palau
        achtereenvolgens beïnvloed of bestuurd door:
        <ul>
            <li><b>Spanje</b> – tot het einde van de 19e eeuw</li>
            <li><b>Duitsland</b> – eind 19e eeuw tot de Eerste Wereldoorlog</li>
            <li><b>Japan</b> – mandaatgebied na de Eerste Wereldoorlog, sterke economische en culturele invloed</li>
            <li><b>Verenigde Staten</b> – na de Tweede Wereldoorlog als deel van het Trust Territory of the Pacific Islands</li>
        </ul>
    </p>

    <p class="infoblock">
        In 1994 werd Palau officieel een onafhankelijke staat onder een Compact of Free Association met de VS.
        Sindsdien heeft het land een eigen grondwet, regering en internationale vertegenwoordiging.
    </p>
</section>

<!-- POLITIEK -->
<section id="politiek">
    <h2>Politiek & bestuur</h2>

    <p class="infoblock">
        Palau is een unitaire presidentiële republiek met een niet‑partijgebonden democratie. De president is zowel
        staatshoofd als regeringsleider. Er is een tweekamerparlement, de Palau National Congress (Olbiil Era Kelulau),
        bestaande uit een Senaat en een Huis van Afgevaardigden.
    </p>

    <p class="infoblock">
        De grondwet van Palau legt veel nadruk op mensenrechten, milieu en traditionele structuren. Traditionele
        leiders (chiefs) spelen nog steeds een rol in lokale besluitvorming, naast de moderne staatsinstellingen.
    </p>

    <p class="infoblock">
        Palau onderhoudt nauwe banden met de Verenigde Staten, Japan en andere landen in de regio. Het is lid van
        de Verenigde Naties en verschillende regionale organisaties in de Stille Oceaan.
    </p>
</section>

<!-- ECONOMIE -->
<section id="economie">
    <h2>Economie</h2>

    <p class="infoblock">
        De economie van Palau is klein maar sterk afhankelijk van <b>toerisme</b>, vooral duik‑ en ecotoerisme.
        Andere sectoren zijn visserij, kleine landbouw, overheidsdiensten en buitenlandse hulp (vooral vanuit de VS).
    </p>

    <p class="infoblock">
        De munteenheid is de <b>Amerikaanse dollar (USD)</b>. Er is geen eigen centrale bank. Het bruto binnenlands
        product per hoofd van de bevolking ligt relatief hoog vergeleken met veel andere eilanden in de regio,
        mede door toerisme en internationale steun.
    </p>

    <p class="infoblock">
        Palau probeert de balans te bewaren tussen economische groei en bescherming van de natuur. Er zijn
        strikte regels voor visserij, bouw en toerisme in kwetsbare gebieden.
    </p>
</section>

<!-- NATUUR & MILIEU -->
<section id="natuur">
    <h2>Natuur, flora & fauna, milieu</h2>

    <p class="infoblock">
        Palau behoort tot de biologisch meest diverse gebieden ter wereld. De koraalriffen, mangroven, zeegrasvelden
        en tropische bossen vormen leefgebieden voor duizenden soorten planten en dieren.
    </p>

    <p class="infoblock">
        Belangrijke kenmerken:
        <ul>
            <li>Meer dan 1.300 soorten vissen en honderden soorten koralen</li>
            <li>Zeeschildpadden, rifhaaien, manta’s en dolfijnen</li>
            <li>Tropische vogels, waaronder endemische soorten</li>
            <li>Mangrovebossen die kusten beschermen en jonge vissen huisvesten</li>
        </ul>
    </p>

    <p class="infoblock">
        Palau is een pionier in natuurbehoud. Het <b>Palau National Marine Sanctuary</b> beschermt een enorm deel
        van de exclusieve economische zone tegen commerciële visserij. Palau was ook een van de eerste landen
        met een nationaal haaienreservaat.
    </p>

    <p class="infoblock">
        De <b>Palau Pledge</b> is een unieke belofte die elke bezoeker in zijn paspoort krijgt: toeristen beloven
        de natuur en cultuur van Palau te respecteren. Dit is een voorbeeld van hoe het land duurzaam toerisme
        probeert te bevorderen.
    </p>
</section>

<!-- DUIKEN -->
<section id="duiken">
    <h2>Duiken & onderwaterwereld</h2>

    <p class="infoblock">
        Palau wordt vaak genoemd als een van de beste duikbestemmingen ter wereld. Het zicht is vaak 30–40 meter
        of meer, en de watertemperatuur ligt rond de 27–30 °C.
    </p>

    <p class="infoblock">
        Bekende duiklocaties:
        <ul>
            <li><b>Blue Corner</b> – sterke stromingen, veel haaien, barracuda’s en grote scholen vissen</li>
            <li><b>Blue Holes</b> – onderwatergrotten met lichtstralen die door openingen naar binnen vallen</li>
            <li><b>German Channel</b> – manta’s, haaien en rijke koraalriffen</li>
            <li><b>Ulong Channel</b> – driftduik met prachtige koralen en haaien</li>
            <li><b>Chandelier Cave</b> – grotten met luchtkamers, populair bij ervaren duikers</li>
            <li><b>Jellyfish Lake</b> – meer met niet‑stekende kwallen (soms tijdelijk gesloten voor herstel)</li>
        </ul>
    </p>

    <p class="infoblock">
        Duiken in Palau is sterk gereguleerd om de natuur te beschermen. Duikers betalen vaak een milieupas en
        moeten zich houden aan strikte regels, zoals niet aanraken van koralen en geen afval achterlaten.
    </p>
</section>

<!-- CULTUUR -->
<section id="cultuur">
    <h2>Cultuur, taal & religie</h2>

    <p class="infoblock">
        De Palause cultuur is diep geworteld in familie, gemeenschap en respect voor de natuur. Traditionele
        structuren, zoals clans en chiefs, spelen nog steeds een rol in het sociale leven.
    </p>

    <p class="infoblock">
        <b>Taal:</b> Palauaans is de belangrijkste lokale taal. Engels wordt veel gebruikt in overheid, onderwijs
        en toerisme. In sommige staten zijn ook Sonsorolese, Tobiaans en Japans officiële of erkende talen.
    </p>

    <p class="infoblock">
        <b>Religie:</b> Het grootste deel van de bevolking is christelijk (voornamelijk rooms‑katholiek en protestants).
        Er zijn ook aanhangers van de inheemse religie Modekngei, die elementen van christendom en traditionele
        overtuigingen combineert, en een kleine moslimgemeenschap.
    </p>

    <p class="infoblock">
        <b>Bai‑huizen</b> (traditionele vergaderhuizen) zijn belangrijke symbolen van de Palause identiteit.
        Ze zijn vaak rijk versierd met houtsnijwerk dat mythen, geschiedenis en sociale regels uitbeeldt.
    </p>
</section>

<!-- TOERISME -->
<section id="toerisme">
    <h2>Toerisme & reizen naar Palau</h2>

    <p class="infoblock">
        Toerisme is een van de belangrijkste pijlers van de economie. De meeste bezoekers komen voor duiken,
        snorkelen, kajakken, natuurbeleving en cultuur. Koror is het belangrijkste vertrekpunt voor tours en duiktrips.
    </p>

    <p class="infoblock">
        Reizen naar Palau gebeurt meestal via vluchten vanuit onder andere Guam, de Filipijnen, Taiwan of Japan.
        Bezoekers hebben vaak een geldig paspoort nodig en moeten voldoen aan de inreisregels, waaronder de
        Palau Pledge.
    </p>

    <p class="infoblock">
        Palau probeert massatoerisme te vermijden en richt zich op kwalitatief, duurzaam toerisme. Dit betekent
        soms hogere prijzen, maar ook beter behoud van natuur en cultuur.
    </p>
</section>

<!-- DEMOGRAFIE, ONDERWIJS, GEZONDHEID (SAMENGEVAT) -->
<section id="maatschappij">
    <h2>Bevolking, onderwijs & gezondheidszorg</h2>

    <p class="infoblock">
        De bevolking van Palau bestaat voornamelijk uit Palauan (Micronesische) inwoners, met daarnaast Aziatische
        gemeenschappen (onder andere Filipijns, Chinees, Japans) en kleinere groepen uit andere regio’s.
    </p>

    <p class="infoblock">
        Onderwijs is verplicht tot een bepaalde leeftijd en er zijn basisscholen en middelbare scholen verspreid
        over de eilanden. Voor hoger onderwijs gaan veel studenten naar het buitenland of naar regionale instellingen.
    </p>

    <p class="infoblock">
        De gezondheidszorg is geconcentreerd in Koror en Babeldaob. Voor zeer gespecialiseerde zorg wordt soms
        uitgeweken naar andere landen, zoals de VS of Guam.
    </p>
</section>

</main>

<script>
/* --- ZOEKFUNCTIE: filtert ALLE tekstblokken --- */
document.getElementById("search").addEventListener("input", function() {
    const q = this.value.toLowerCase();
    const blocks = document.querySelectorAll(".infoblock");
    blocks.forEach(block => {
        const text = block.textContent.toLowerCase();
        block.style.display = text.includes(q) ? "block" : "none";
    });
});
</script>

</body>
</html>
