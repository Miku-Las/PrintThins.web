<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webové stránky</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
        }
        header {
            background-color: #0073e6;
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            gap: 15px;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        nav ul li a:hover {
            text-decoration: underline;
        }
        main {
            padding: 20px;
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        iframe {
            width: 100%;
            border: none;
            min-height: 80vh;
        }
    </style>
    <script>
        function showTab(tabId) {
            const tabs = document.querySelectorAll('.tab-content');
            tabs.forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
        }
    </script>
</head>
<body>
    <header>
        <h1>Project 3D tisk</h1>
        <nav>
            <ul>
                <li><a href="#" onclick="showTab('services')">Služby</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="services" class="tab-content active">
            <h2>Služby</h2>
            <h3>Podání poptávky</h3>
            <p>Pokud máte zájem o naše služby, neváhejte využít níže uvedený formulář. Rádi vám pomůžeme realizovat vaše projekty.</p>
            <iframe src="https://kalkukacka.for3dtisk.production.clients.sentiscrape.cz/calculator.html?formId=PwlrKV0PiMalFdOvNl62Rw"></iframe>
        </section>
    </main>
</body>
</html>
