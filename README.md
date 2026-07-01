
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

        .search-box {
            width: 100%;
            max-width: 400px;
            padding: 10px;
            margin: 20px 0;
            border-radius: 5px;
            border: none;
            font-size: 16px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: #ffffff;
            color: #000000;
            border-radius: 10px;
            overflow: hidden;
        }

        th {
            background: #0369a1;
            color: white;
            padding: 12px;
            text-align: left;
        }

        td {
            padding: 12px;
            border-top: 1px solid #d1d5db;
            color: #000000;
        }

        tr:nth-child(even) {
            background: #f1f5f9;
        }

        tr:nth-child(odd) {
            background: #ffffff;
        }

        tr:hover {
            background: #dbeafe;
        }
    </style>
</head>

<body>

<header>
    <h1>Test-Oil</h1>
    <nav>
        <a href="#">Home</a>
        <a href="#Test">Test</a>
        <a href="#contatti">Contatti</a>
    </nav>
</header>

<section class="hero">
    <h2>Innovazione per un futuro sostenibile.</h2>
    <p>Soluzioni intelligenti per economia circolare</p>
    <button onclick="alert('Benvenuto su Test-Oil!')">Scopri di più</button>
</section>

<section id="Test" class="container">
    <h2>Elenco Clienti</h2>

    <input
        type="text"
        id="searchInput"
        class="search-box"
        placeholder="Cerca cliente..."
        onkeyup="searchClient()"
    >

    <table id="clientTable">
        <thead>
            <tr>
                <th>Cliente</th>
                <th>Primo Test</th>
                <th>Ultimo Test</th>
                <th>Numero Test</th>
            </tr>
        </thead>

        <tbody>
            <tr><td>A</td><td>01/01/2026</td><td>15/06/2026</td><td>5</td></tr>
            <tr><td>B</td><td>02/01/2026</td><td>16/06/2026</td><td>3</td></tr>
            <tr><td>C</td><td>03/01/2026</td><td>17/06/2026</td><td>7</td></tr>
            <tr><td>D</td><td>04/01/2026</td><td>18/06/2026</td><td>2</td></tr>
            <tr><td>E</td><td>05/01/2026</td><td>19/06/2026</td><td>9</td></tr>
            <tr><td>F</td><td>06/01/2026</td><td>20/06/2026</td><td>4</td></tr>
            <tr><td>G</td><td>07/01/2026</td><td>21/06/2026</td><td>6</td></tr>
            <tr><td>H</td><td>08/01/2026</td><td>22/06/2026</td><td>8</td></tr>
            <tr><td>I</td><td>09/01/2026</td><td>23/06/2026</td><td>1</td></tr>
            <tr><td>J</td><td>10/01/2026</td><td>24/06/2026</td><td>5</td></tr>
            <tr><td>K</td><td>11/01/2026</td><td>25/06/2026</td><td>7</td></tr>
            <tr><td>L</td><td>12/01/2026</td><td>26/06/2026</td><td>3</td></tr>
            <tr><td>M</td><td>13/01/2026</td><td>27/06/2026</td><td>10</td></tr>
            <tr><td>N</td><td>14/01/2026</td><td>28/06/2026</td><td>2</td></tr>
            <tr><td>O</td><td>15/01/2026</td><td>29/06/2026</td><td>11</td></tr>
            <tr><td>P</td><td>16/01/2026</td><td>30/06/2026</td><td>4</td></tr>
            <tr><td>Q</td><td>17/01/2026</td><td>01/07/2026</td><td>6</td></tr>
            <tr><td>R</td><td>18/01/2026</td><td>02/07/2026</td><td>8</td></tr>
            <tr><td>S</td><td>19/01/2026</td><td>03/07/2026</td><td>5</td></tr>
            <tr><td>T</td><td>20/01/2026</td><td>04/07/2026</td><td>9</td></tr>
        </tbody>
    </table>
</section>

<section id="contatti" class="container">
    <h2>Contatti</h2>
    <p>Email: info@test-oil.com</p>
</section>

<footer>
    <p>© 2026 Test-Oil | Tutti i diritti riservati</p>
</footer>

<script>
function searchClient() {
    let input = document.getElementById("searchInput");
    let filter = input.value.toUpperCase();
    let table = document.getElementById("clientTable");
    let tr = table.getElementsByTagName("tr");

    for (let i = 1; i < tr.length; i++) {
        let td = tr[i].getElementsByTagName("td")[0];

        if (td) {
            let txtValue = td.textContent || td.innerText;
            tr[i].style.display =
                txtValue.toUpperCase().indexOf(filter) > -1
                    ? ""
          ody>
</html>

