<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Portafolio minimalista in stile GitHub">
  <title>Portfolio di Nome Cognome</title>
  <style>
    /* Stile generale */
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      background-color: #f6f8fa;
      margin: 0;
      padding: 0;
      color: #24292f;
    }
    
    /* Stile per l'header */
    header {
      background-color: #24292f;
      color: #ffffff;
      padding: 20px;
      text-align: center;
    }
    
    header h1 {
      font-size: 24px;
      margin: 0;
    }
    
    header p {
      font-size: 16px;
      margin-top: 5px;
      color: #c9d1d9;
    }
    
    /* Stile per le sezioni */
    section {
      width: 80%;
      max-width: 900px;
      margin: 20px auto;
      background-color: #ffffff;
      padding: 20px;
      border-radius: 6px;
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    }
    
    section h2 {
      font-size: 20px;
      color: #0366d6;
    }
    
    section p {
      font-size: 16px;
      line-height: 1.5;
    }
    
    ul {
      padding-left: 20px;
    }
    
    ul li {
      margin-bottom: 10px;
    }
    
    a {
      color: #0366d6;
      text-decoration: none;
    }
    
    a:hover {
      text-decoration: underline;
    }
    
    /* Stile del footer */
    footer {
      text-align: center;
      padding: 10px;
      background-color: #24292f;
      color: white;
      margin-top: 40px;
    }
    
    /* Stile per il pulsante di tema */
    .theme-toggle {
      display: flex;
      justify-content: flex-end;
      width: 80%;
      max-width: 900px;
      margin: 10px auto;
    }
    
    .theme-toggle button {
      padding: 10px 15px;
      background-color: #0366d6;
      color: #ffffff;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-size: 14px;
    }
    
    .theme-toggle button:hover {
      background-color: #005cc5;
    }
    
    /* Modalità dark */
    body.dark-mode {
      background-color: #0d1117;
      color: #c9d1d9;
    }
    
    body.dark-mode header {
      background-color: #161b22;
    }
    
    body.dark-mode section {
      background-color: #161b22;
    }
    
    body.dark-mode a {
      color: #58a6ff;
    }
    
    body.dark-mode footer {
      background-color: #161b22;
    }
    
    body.dark-mode .theme-toggle button {
      background-color: #58a6ff;
      color: #0d1117;
    }
  </style>
</head>
<body>

  <header>
    <h1>Portfolio di Nome Cognome</h1>
    <p>Sviluppatore Web | Designer | Programmatore</p>
  </header>

  <div class="theme-toggle">
    <button onclick="toggleTheme()">Attiva Modalità Scura</button>
  </div>

  <section>
    <h2>Chi Sono</h2>
    <p>Sono uno sviluppatore appassionato di tecnologia e innovazione, con esperienza in diversi linguaggi di programmazione e framework. Amo creare soluzioni semplici e ben progettate.</p>
  </section>

  <section>
    <h2>Progetti</h2>
    <ul>
      <li><a href="https://github.com/username/progetto1">Progetto 1</a> - Descrizione breve del progetto 1.</li>
      <li><a href="https://github.com/username/progetto2">Progetto 2</a> - Descrizione breve del progetto 2.</li>
      <li><a href="https://github.com/username/progetto3">Progetto 3</a> - Descrizione breve del progetto 3.</li>
    </ul>
  </section>

  <section>
    <h2>Contatti</h2>
    <p>Email: nomecognome@example.com</p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/tuonome">https://www.linkedin.com/in/tuonome</a></p>
  </section>

  <footer>
    <p>&copy; 2024 Nome Cognome</p>
  </footer>

  <script>
    // Funzione per attivare/disattivare la modalità scura
    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
      
      const button = document.querySelector('.theme-toggle button');
      if (document.body.classList.contains('dark-mode')) {
        button.textContent = 'Attiva Modalità Chiara';
      } else {
        button.textContent = 'Attiva Modalità Scura';
      }
    }
  </script>

</body>
</html>
