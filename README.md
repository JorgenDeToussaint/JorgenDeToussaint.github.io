<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mateusz Zalewski | Dashboard</title>
    <style>
        /* Systemowa paleta barw - Deep Dark */
        :root {
            --bg-color: #0d1117;
            --tile-bg: #161b22;
            --border-color: #30363d;
            --text-main: #f0f6fc;
            --text-accent: #58a6ff;
            --hover-bg: #21262d;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            font-size: 2.5rem;
            color: var(--text-accent);
            margin: 0;
        }

        header p {
            color: #8b949e;
            font-size: 1.1rem;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            width: 90%;
            max-width: 900px;
        }

        .tile {
            background-color: var(--tile-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 30px;
            text-decoration: none;
            color: inherit;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .tile:hover {
            background-color: var(--hover-bg);
            border-color: #8b949e;
            transform: translateY(-8px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
        }

        .tile h2 {
            margin: 0 0 10px 0;
            color: var(--text-accent);
        }

        .tile p {
            font-size: 0.9rem;
            color: #8b949e;
            margin: 0;
        }

        /* Responsywność dla mobile */
        @media (max-width: 600px) {
            header h1 { font-size: 1.8rem; }
        }
    </style>
</head>
<body>

    <header>
        <h1>Mateusz Zalewski</h1>
        <p>Data Engineer | Strategist | Polymath</p>
    </header>

    <div class="grid-container">
        <a href="https://github.com/JorgenDeToussaint" class="tile">
            <h2>Data Engineering</h2>
            <p>AWS, SQL, Spark & Clean Code</p>
        </a>
        
        <a href="#" class="tile">
            <h2>Stowarzyszenie</h2>
            <p>Finanse i Zarządzanie (Skarbnik)</p>
        </a>

        <a href="#" class="tile">
            <h2>Knowledge Base</h2>
            <p>Blog techniczny i notatki inżynierskie</p>
        </a>

        <a href="#" class="tile">
            <h2>Experimental</h2>
            <p>Gaming (Soulsborne) & Future Projects</p>
        </a>
    </div>

</body>
</html>
