
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
            background: #1e293b;
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
            border-top: 1px solid #334155;
        }

        tr:hover {
            background: #334155;
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
    <h2>Test</h2>

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
            <tr>
                <td>A</td>
                <td>01/01/2026</td>
                <td>15/06/2026</td>
                <td>5</td>
            </tr>
            <tr>
                <td>B</td>
                <td>10/02/2026</td>
                <td>20/06/2026</td>
                <td>3</td>
            </tr>
            <tr>
                <td>C</td>
                <td>05/03/2026</td>
                <td>18/06/2026</td>
                <td>7</td>
            </tr>
            <tr>
                <td>D</td>
                <td>12/04/2026</td>
                <td>25/06/2026</td>
                <td>2</td>
            </tr>
        </tbody>
    </table>
</section>

<section id="contatti" class="container">
    <h2>Contatti</h2>
    <p>Email: info@test-oil.com</p>
</section>

<footer>
    <p>© 2026 Test | Tutti i diritti riservati</p>
</footer>

<script>
function searchClient() {
    let input = document.getElementById("searchInput");
    let filter = input.value.toUpperCase();
    let table = document.getElementById("clientTable");
    let tr = table.getElementsByTagName("tr");

    for (let i = 1; i < tr.length; i++) {
        let td = tr[i].getElementsByTagName("td")[0];
tContent || td.innerText;
            tr[i].style.display =
                txtValue.toUpperCase().indexOf(filter) > -1
                    ? ""
                    : "none";
        }
    }
}
</script>

</body>
</html>

