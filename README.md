
<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test-Oil</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #0f172a;
            color: white;
        }

        header {
            background: #020617;
            padding: 20px;
            text-align: center;
        }

        header h1 {
            margin: 0;
            color: #38bdf8;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }

        .hero {
            padding: 80px 20px;
            text-align: center;
            background: linear-gradient(135deg, #1e293b, #0369a1);
        }

        .hero h2 {
            font-size: 40px;
        }

        .container {
            padding: 40px;
        }

        .card {
            background: #1e293b;
            padding: 20px;
            margin: 15px;
            border-radius: 10px;
            display: inline-block;
            width: 250px;
        }

        footer {
            background: #020617;
            padding: 15px;
            text-align: center;
            margin-top: 30px;
        }

        button {
            padding: 10px 20px;
            border: none;
            background: #38bdf8;
            color: black;
            font-weight: bold;
            border-radius: 5px;
            cursor: pointer;
        }

    </style>
</head>

<body>

<header>
    <h1>Test-Oil</h1>
    <nav>
        <a href="#">Home</a>
        <a href="#servizi">Servizi</a>
        <a href="#contatti">Contatti</a>
    </nav>
</header>

<section class="hero">
    <h2>Energia. Innovazione. Futuro.</h2>
    <p>Soluzioni intelligenti per efficienza energetica e sostenibilità</p>
    <button onclick="alert('Benvenuto su Test-Oil!')">Scopri di più</button>
</section>

<section id="servizi" class="container">
    <h2>Servizi</h2>

    <div class="card">
        <h3>Analisi Energetica</h3>
        <p>Ottimizzazione consumi e performance.</p>
    </div>

    <div class="card">
        <h3>Consulenza</h3>
        <p>Strategie sostenibili per aziende.</p>
    </div>

    <div class="card">
        <h3>Innovazione</h3>
        <p>Tecnologie avanzate nel settore oil & energy.</p>
    </div>
</section>

<section id="contatti" class="container">
    <h2>Contatti</h2>
    <p>Email: info@test-oil.com</p>
</section>

<footer>
    <p>© 2026 Test-Oil | Tutti i diritti riservati</p>
</footer>

</body>
</html>
