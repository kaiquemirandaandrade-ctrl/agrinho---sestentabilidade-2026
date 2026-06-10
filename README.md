# agrinho---sustentabilidade-2026<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EcoFuture - Sustentabilidade Ambiental</title>
    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            font-family:'Segoe UI', sans-serif;
        }
        body{
            background:#f5fdf6;
            color:#333;
            line-height:1.6;
        }
        header{
            background:linear-gradient(135deg,#2e7d32,#4caf50);
            color:white;
            text-align:center;
            padding:100px 20px;
        }
        header h1{
            font-size:3rem;
            margin-bottom:15px;
        }
        header p{
            font-size:1.2rem;
            max-width:700px;
            margin:auto;
        }
        .btn{
            display:inline-block;
            margin-top:20px;
            padding:12px 25px;
            background:white;
            color:#2e7d32;
            text-decoration:none;
            border-radius:30px;
            font-weight:bold;
            transition:.3s;
        }
        .btn:hover{
            transform:translateY(-3px);
        }
        section{
            padding:80px 10%;
        }
        .titulo{
            text-align:center;
            margin-bottom:40px;
            color:#2e7d32;
        }
        .cards{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:25px;
        }
        .card{
            background:white;
            padding:25px;
            border-radius:15px;
            box-shadow:0 5px 15px rgba(0,0,0,.1);
            transition:.3s;
        }
        .card:hover{
            transform:translateY(-8px);
        }
        .card h3{
            margin-bottom:10px;
            color:#388e3c;
        }
        .impacto{
            background:#e8f5e9;
            text-align:center;
        }
        .contador{
            font-size:3rem;
            font-weight:bold;
            color:#2e7d32;
        }
        footer{
            background:#1b5e20;
            color:white;
            text-align:center;
            padding:25px;
        }
    </style>
</head>
<body>
    <header>
        <h1><span aria-hidden="true">🌍</span> EcoFuture</h1>
        <p>Promovendo a conscientização ambiental e incentivando ações sustentáveis para construir um futuro melhor.</p>
        <a href="#acoes" class="btn">Conheça as Ações</a>
    </header>
    
    <main>
        <section>
            <h2 class="titulo">Por que a Sustentabilidade é Importante?</h2>
            <div class="cards">
                <div class="card">
                    <h3><span aria-hidden="true">♻️</span> Reciclagem</h3>
                    <p>Reduz o volume de resíduos e preserva recursos naturais.</p>
                </div>
                <div class="card">
                    <h3><span aria-hidden="true">🌳</span> Reflorestamento</h3>
                    <p>Ajuda a recuperar áreas degradadas e protege a biodiversidade.</p>
                </div>
                <div class="card">
                    <h3><span aria-hidden="true">💧</span> Uso Consciente da Água</h3>
                    <p>Pequenas atitudes evitam desperdícios e garantem recursos futuros.</p>
                </div>
            </div>
        </section>

        <section class="impacto">
            <h2 class="titulo">Nosso Impacto</h2>
            <div class="contador" id="contador">0</div>
            <p>Árvores simbolicamente plantadas</p>
        </section>

        <section id="acoes">
            <h2 class="titulo">Como Você Pode Ajudar?</h2>
            <div class="cards">
                <div class="card">
                    <h3><span aria-hidden="true">🚲</span> Transporte Sustentável</h3>
                    <p>Utilize bicicleta, caminhada ou transporte coletivo.</p>
                </div>
                <div class="card">
                    <h3><span aria-hidden="true">⚡</span> Economia de Energia</h3>
                    <p>Desligue aparelhos que não estão sendo utilizados.</p>
                </div>
                <div class="card">
                    <h3><span aria-hidden="true">🌱</span> Consumo Responsável</h3>
                    <p>Prefira produtos sustentáveis e de origem consciente.</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 EcoFuture | Projeto de Sustentabilidade Ambiental</p>
    </footer>

    <script>
        let contador = 0;
        const alvo = 5000;
        const elementoContador = document.getElementById("contador");

        function animarContador() {
            if (contador < alvo) {
                contador += 25;
                elementoContador.innerText = contador.toLocaleString("pt-BR");
                requestAnimationFrame(animarContador);
            } else {
                elementoContador.innerText = alvo.toLocaleString("pt-BR");
            }
        }
        
        animarContador();
    </script>
</body>
</html>
