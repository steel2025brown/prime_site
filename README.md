# prime_site <!--🚧 Projeto do Dia 5: Mini Portfólio com botão interativo
Você vai criar um site com:

Seu nome e profissão fictícia (ex: Desenvolvedor Web)

Uma breve bio

Uma lista de habilidades (HTML, CSS, JS)

Um botão que mostra ou esconde um parágrafo com mais informações-->
<!DOCTYPE html>
<html lang="pt-Br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #e3f2fd;
            color: #333;
            padding: 20%;
        }

        .card {
            background: white;
            padding: 20%;
            border-radius: 10px;
            box-shadow: 0 2px 8px rgb(0,0,0,0.2);
            max-width: 400px;
            margin: auto;
        }
        button {
            margin: 10px;
            padding: 10px 15px;
            font-weight: bold;
            border: none;
            border-radius: 5px;
            background-color: #2196f3;
            color: white;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="card">
        <h1>Steel Brown</h1>
        <p>Desenvolvedor Web</p>
        <ul>
            <li>HTML5</li>
            <li>CSS3</li>
            <li>JAVASCRIPT</li>
        </ul>
        <button onclick="toggleInfo()">Mostrar Mais</button>
        <p id="info">Sou um desenvolver aprendiz. Apaixonado por tecnologia e amo criar interfaces modernas e responsivas.</p>
    </div>
    <script>
        function toggleInfo() {
            const info = document.getElementById("info");
            if (info.style.display === "none") {
              info.style.display = "block";  
            } else {
                info.style.display = "none";
            }
        }
        
    </script>
    
</body>
</html>
