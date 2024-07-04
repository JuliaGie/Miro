<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplikacja Miro</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffffff;
            color: #333333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #ff9900;
            color: #ffffff;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            background-color: #ff9900;
            overflow: hidden;
        }
        nav a {
            float: left;
            display: block;
            color: #ffffff;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #ff7700;
        }
        .container {
            padding: 20px;
        }
        .section {
            margin-bottom: 20px;
        }
        .section h2 {
            color: #ff9900;
        }
        .accordion {
            cursor: pointer;
            padding: 10px;
            width: 100%;
            text-align: left;
            outline: none;
            border: none;
            transition: background-color 0.4s ease;
        }
        .active, .accordion:hover {
            background-color: #ffcc80;
        }
        .panel {
            padding: 0 18px;
            background-color: white;
            display: none;
            overflow: hidden;
        }
        footer {
            background-color: #ff9900;
            color: #ffffff;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

<header>
    <h1>Strona o aplikacji Miro</h1>
</header>

<nav>
    <a href="#info">Informacje</a>
    <a href="#proscons">Wady i zalety</a>
    <a href="#students">Możliwości dla uczniów i nauczycieli</a>
    <a href="#pricing">Abonament</a>
    <a href="#examples">Przykłady zastosowań</a>
    <a href="#opinions">Opinie</a>
    <a href="#about">O mnie</a>
</nav>

<div class="container">
    <div id="info" class="section">
        <h2>Informacje na temat aplikacji</h2>
        <p>Miro to narzędzie do współpracy online, które umożliwia zespołom pracę na wspólnej tablicy. Jest szczególnie przydatne w pracy zdalnej, gdzie użytkownicy mogą tworzyć, edytować i udostępniać swoje projekty w czasie rzeczywistym.</p>
    </div>

    <div id="proscons" class="section">
        <h2>Wady i zalety</h2>
        <button class="accordion">Zalety</button>
        <div class="panel">
            <ul>
                <li>Łatwa w użyciu</li>
                <li>Dostępna na różnych platformach</li>
                <li>Współpraca w czasie rzeczywistym</li>
            </ul>
        </div>

        <button class="accordion">Wady</button>
        <div class="panel">
            <ul>
                <li>Może być kosztowna dla dużych zespołów</li>
                <li>Wymaga stabilnego połączenia internetowego</li>
            </ul>
        </div>
    </div>

    <div id="students" class="section">
        <h2>Możliwości dla uczniów i nauczycieli</h2>
        <p>Miro oferuje wiele narzędzi, które wspierają proces edukacyjny, takie jak:</p>
        <ul>
            <li>Interaktywne tablice</li>
            <li>Możliwość współpracy w czasie rzeczywistym</li>
            <li>Integracja z innymi narzędziami edukacyjnymi</li>
        </ul>
    </div>

    <div id="pricing" class="section">
        <h2>Informacje o abonamencie</h2>
        <p>Miro oferuje różne plany abonamentowe, w tym darmowy plan podstawowy oraz plany płatne z dodatkowymi funkcjami:</p>
        <ul>
            <li>Darmowy - podstawowe funkcje</li>
            <li>Team - dodatkowe funkcje i integracje</li>
            <li>Business - zaawansowane narzędzia do zarządzania zespołem</li>
            <li>Enterprise - pełna funkcjonalność i wsparcie</li>
        </ul>
    </div>

    <div id="examples" class="section">
        <h2>Wizualizacja zastosowań - przykłady</h2>
        <img src="example1.jpg" alt="Przykład 1" style="width:100%;height:auto;">
        <img src="example2.jpg" alt="Przykład 2" style="width:100%;height:auto;">
    </div>

    <div id="opinions" class="section">
        <h2>Opinie użytkowników</h2>
        <p>Studentka Ania: "Miro ułatwiło nam pracę nad projektem grupowym, mogliśmy współpracować zdalnie bez żadnych problemów."</p>
        <p>Nauczyciel Marek: "Dzięki Miro mogę prowadzić lekcje online w sposób bardziej interaktywny i angażujący dla uczniów."</p>
    </div>

    <div id="about" class="section">
        <h2>O mnie</h2>
        <p>Nazywam się Jan Kowalski. Jestem studentem informatyki i pasjonatem nowych technologii. Na tej stronie dzielę się informacjami o aplikacji Miro, której często używam w swojej codziennej pracy i nauce.</p>
    </div>
</div>

<footer>
    <p>Kontakt: jan.kowalski@example.com</p>
</footer>

<script>
    var acc = document.getElementsByClassName("accordion");
    var i;

    for (i = 0; i < acc.length; i++) {
        acc[i].addEventListener("click", function() {
            this.classList.toggle("active");
            var panel = this.nextElementSibling;
            if (panel.style.display === "block") {
                panel.style.display = "none";
            } else {
                panel.style.display = "block";
            }
        });
    }
</script>

</body>
</html>
