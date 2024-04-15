# informatyka_projekt_html

### All

```html css

<!DOCTYPE html>
<html lang="pl">
<head>
    <noscript>JavaScript nie jest obsługiwany przez twoją przeglądarkę! <br> Niektóre funkcje strony nie są dostępne!</noscript>
    <link rel="stylesheet" href="UI.css">
    <title>Wielbłądy</title>
</head>
<body>

<header>
    <h1>Wielbłądy</h1>
</header>

<nav>
    <a href="#przegląd">Przegląd</a>
    <a href="#gatunek">Gatunki</a>
    <a href="#wygląd">Wygląd</a>
    <a href="#habitat">Środowisko</a>
    <a href="#zachowanie">Zachowanie</a>
    <a href="galeria.html">Galeria zdjęć</a>
</nav>

<section id="przegląd">
    <h2>Przegląd</h2>
    <div class="div_image">
    <img src="WB.jpg" class="lewo">
    <p>    ● Wielbłądy, znane również jako dromader lub wielbłąd arabski, są jednymi z najbardziej charakterystycznych zwierząt pustynnych.<br>
        ● Mają długie nogi i szyję, oraz grzbiet pokryty grzywą.<br>
        ● Ich najbardziej charakterystyczną cechą są garby na grzbiecie, które zawierają tkankę tłuszczową, pomagającą im przetrwać w warunkach pustynnych.<br></p>
    </div>
</section>

<section id="gatunek">
    <h2>Gatunki</h2>
    <div class="div_image">
        <img src="WB2.jpg" class="lewo">
        <p>● Wielbłąd arabski, który ma jeden garb. <br>
            ● Wielbłąd dwugarbny, który ma dwa garby.</p>
        <img src="WB3.jpg" class="prawo">
    </div>
</section>

<section id="wygląd">
    <h2>Wygląd</h2>
    <div class="div_image">
        <img src="WB4.jpg" class="lewo">
        <p>    ● Wielbłądy mają duże, szerokie kopyta, co pomaga im poruszać się po piaszczystym terenie bez zapadania się.<br>
            ● Ich futro jest zazwyczaj długie i grube, chroniąc przed skrajnymi temperaturami i piaskiem.<br></p>
    </div>
</section>


<section id="habitat">
    <h2>Środowisko</h2>
    <div class="div_image">
        <img src="WB5.jpg" class="lewo">
    <p>    ● Wielbłądy są dobrze przystosowane do życia w surowych warunkach pustynnych.<br>
        ● Spotyka się je głównie w obszarach Afryki Północnej i Azji, gdzie występują rozległe pustynie.<br></p>
    </div>
</section>

<section id="zachowanie">
    <h2>Zachowanie</h2>
    <div class="div_image">
        <img src="WB6.jpg" class="lewo">
    <p>    ● Są zwierzętami stadnymi, które żyją w dużych grupach, zwanych trzodami.<br>
        ● Wielbłądy są znane ze swojej wytrzymałości na ekstremalne warunki, w tym na brak wody i pokarmu przez długie okresy.<br>
        ● Potrafią przechowywać zapasy tłuszczu i wody w swoich garbach, co pozwala im przetrwać nawet w najtrudniejszych warunkach.<br>
        ● Mają też znakomite zdolności do dostosowywania się do zmieniających się warunków pogodowych i terenowych.<br>
    </p>
    </div>
</section>

<footer>
    <p>Piotr Kujawa 7B</p>
</footer>

<button class="dark-mode-toggle" onclick="toggleDarkMode()">🌙</button>

<script>
    function toggleDarkMode() {
        const body = document.querySelector('body');
        body.classList.toggle('dark-mode');
    }
</script>

</body>
</html>


--------------------

<!DOCTYPE html>

<html lang="pl">

    <head>
        <noscript>JavaScript nie jest obsługiwany przez twoją przeglądarkę! <br> Niektóre funkcje strony nie są dostępne!</noscript>
        <link rel="stylesheet" href="UI.css">
        <title>Wielbłądy</title>
    </head>

    <header>
        <h1>Wielbłądy - Galeria</h1>
    </header>

    <nav>
        <a href="index.html">Powrót</a>
    </nav>
<body>

<div class="galeria">

        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">
        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">
        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">

    </div>

</body>

<footer>
    <p>Piotr Kujawa 7B</p>
</footer>

<button class="dark-mode-toggle" onclick="toggleDarkMode()">🌙</button>

<script>

    function toggleDarkMode() {
        const body = document.querySelector('body');
        body.classList.toggle('dark-mode');
    }
</script>

</html>

-------------------

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
    transition: background-color 0.5s ease;
}
body.dark-mode {
    background-color: #333;
}
header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

img {

    border: 1px;
    border-radius: 5px;
    max-width: 100%;
    height: auto;

}

.galeria {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 10px;
}
.prawo {
    margin-left: 25px;
}
.lewo {
    margin-right: 25px;
}

.div_image {
    display: flex;
    align-items: center;
}
nav {
    background-color: #444;
    padding: 10px 0;
    text-align: center;
}
nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
    font-weight: bold;
}
nav a:hover {
    background-color: #555;
}
section {
    text-align: left;
    border: 1px solid #ccc;
    border-radius: 25px;
    padding: 20px;
    margin: 20px;
    background-color: #fff;
}

footer {
    background-color: #444;
    color: #fff;
    text-align: center;
    padding: 1px;
    position: fixed;
    bottom: -10px;
    width: 100%;

    opacity: 1;
    transition: 0.5s ease;
}

footer:hover {
    opacity: 0.25;
    transition: 0.5s ease;
}


.dark-mode-toggle {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: transparent;
    color: #fff;
    border: none;
    cursor: pointer;
}

```

# -----------------------------

### Index.html

```html index.html

<!DOCTYPE html>
<html lang="pl">
<head>
    <noscript>JavaScript nie jest obsługiwany przez twoją przeglądarkę! <br> Niektóre funkcje strony nie są dostępne!</noscript>
    <link rel="stylesheet" href="UI.css">
    <title>Wielbłądy</title>
</head>
<body>

<header>
    <h1>Wielbłądy</h1>
</header>

<nav>
    <a href="#przegląd">Przegląd</a>
    <a href="#gatunek">Gatunki</a>
    <a href="#wygląd">Wygląd</a>
    <a href="#habitat">Środowisko</a>
    <a href="#zachowanie">Zachowanie</a>
    <a href="galeria.html">Galeria zdjęć</a>
</nav>

<section id="przegląd">
    <h2>Przegląd</h2>
    <div class="div_image">
    <img src="WB.jpg" class="lewo">
    <p>    ● Wielbłądy, znane również jako dromader lub wielbłąd arabski, są jednymi z najbardziej charakterystycznych zwierząt pustynnych.<br>
        ● Mają długie nogi i szyję, oraz grzbiet pokryty grzywą.<br>
        ● Ich najbardziej charakterystyczną cechą są garby na grzbiecie, które zawierają tkankę tłuszczową, pomagającą im przetrwać w warunkach pustynnych.<br></p>
    </div>
</section>

<section id="gatunek">
    <h2>Gatunki</h2>
    <div class="div_image">
        <img src="WB2.jpg" class="lewo">
        <p>● Wielbłąd arabski, który ma jeden garb. <br>
            ● Wielbłąd dwugarbny, który ma dwa garby.</p>
        <img src="WB3.jpg" class="prawo">
    </div>
</section>

<section id="wygląd">
    <h2>Wygląd</h2>
    <div class="div_image">
        <img src="WB4.jpg" class="lewo">
        <p>    ● Wielbłądy mają duże, szerokie kopyta, co pomaga im poruszać się po piaszczystym terenie bez zapadania się.<br>
            ● Ich futro jest zazwyczaj długie i grube, chroniąc przed skrajnymi temperaturami i piaskiem.<br></p>
    </div>
</section>


<section id="habitat">
    <h2>Środowisko</h2>
    <div class="div_image">
        <img src="WB5.jpg" class="lewo">
    <p>    ● Wielbłądy są dobrze przystosowane do życia w surowych warunkach pustynnych.<br>
        ● Spotyka się je głównie w obszarach Afryki Północnej i Azji, gdzie występują rozległe pustynie.<br></p>
    </div>
</section>

<section id="zachowanie">
    <h2>Zachowanie</h2>
    <div class="div_image">
        <img src="WB6.jpg" class="lewo">
    <p>    ● Są zwierzętami stadnymi, które żyją w dużych grupach, zwanych trzodami.<br>
        ● Wielbłądy są znane ze swojej wytrzymałości na ekstremalne warunki, w tym na brak wody i pokarmu przez długie okresy.<br>
        ● Potrafią przechowywać zapasy tłuszczu i wody w swoich garbach, co pozwala im przetrwać nawet w najtrudniejszych warunkach.<br>
        ● Mają też znakomite zdolności do dostosowywania się do zmieniających się warunków pogodowych i terenowych.<br>
    </p>
    </div>
</section>

<footer>
    <p>Piotr Kujawa 7B</p>
</footer>

<button class="dark-mode-toggle" onclick="toggleDarkMode()">🌙</button>

<script>
    function toggleDarkMode() {
        const body = document.querySelector('body');
        body.classList.toggle('dark-mode');
    }
</script>

</body>
</html>


```

### Galeria.html

```html galeria.html

<!DOCTYPE html>

<html lang="pl">

    <head>
        <noscript>JavaScript nie jest obsługiwany przez twoją przeglądarkę! <br> Niektóre funkcje strony nie są dostępne!</noscript>
        <link rel="stylesheet" href="UI.css">
        <title>Wielbłądy</title>
    </head>

    <header>
        <h1>Wielbłądy - Galeria</h1>
    </header>

    <nav>
        <a href="index.html">Powrót</a>
    </nav>
<body>

<div class="galeria">

        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">
        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">
        <img src="WB.jpg" style="margin-right: 25px; margin-top: 25px; margin-left:25px; margin-bottom:25px;">

    </div>

</body>

<footer>
    <p>Piotr Kujawa 7B</p>
</footer>

<button class="dark-mode-toggle" onclick="toggleDarkMode()">🌙</button>

<script>

    function toggleDarkMode() {
        const body = document.querySelector('body');
        body.classList.toggle('dark-mode');
    }
</script>

</html>

```

### UI.css

```css UI.css


body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
    transition: background-color 0.5s ease;
}
body.dark-mode {
    background-color: #333;
}
header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

img {

    border: 1px;
    border-radius: 5px;
    max-width: 100%;
    height: auto;

}

.galeria {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 10px;
}
.prawo {
    margin-left: 25px;
}
.lewo {
    margin-right: 25px;
}

.div_image {
    display: flex;
    align-items: center;
}
nav {
    background-color: #444;
    padding: 10px 0;
    text-align: center;
}
nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
    font-weight: bold;
}
nav a:hover {
    background-color: #555;
}
section {
    text-align: left;
    border: 1px solid #ccc;
    border-radius: 25px;
    padding: 20px;
    margin: 20px;
    background-color: #fff;
}

footer {
    background-color: #444;
    color: #fff;
    text-align: center;
    padding: 1px;
    position: fixed;
    bottom: -10px;
    width: 100%;

    opacity: 1;
    transition: 0.5s ease;
}

footer:hover {
    opacity: 0.25;
    transition: 0.5s ease;
}


.dark-mode-toggle {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: transparent;
    color: #fff;
    border: none;
    cursor: pointer;
}

```
