# Projeto-surf

HTML

<!DOCTYPE html>
<html lang="pt-br">

<head>
  <meta charset="UTF-8" />
  <title>Suporte</title>
  <link rel="stylesheet" href="/css/suporte.css">
</head>

<body>
  <div class="container">

    <!-- HEADER -->
    <header class="topo">
      <button class="voltar">←</button>
      <h1>SUPORTE</h1>
    </header>

    <!-- GRID DE OPÇÕES -->
    <main class="grid">

      <a href="perfil.html" class="card">
        <img src="https://img.icons8.com/ios-filled/100/user.png" />
        <span>Perfil do atleta</span>
      </a>
      <a href="config.html" class="card"><img src="https://img.icons8.com/ios-filled/100/settings.png" />
        <span>Configuração</span>
      </a>
      <a href="videos.html" class="card"><img src="https://img.icons8.com/ios-filled/100/video.png" />
        <span>Vídeos</span>
      </a>
      <a href="planos.html" class="card mover"><img src="https://img.icons8.com/ios-filled/100/planner.png" />
        <span>Planos</span>
      </a>
      <a href="contato.html" class="card mover"><img src="https://img.icons8.com/ios-filled/100/phone.png" />
        <span>Contato</span>
      </a>


    </main>
  </div>
</body>

</html>







CSS

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

body {
  background: #111;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

/* CONTAINER PRINCIPAL */
.container {
  width: 900px;
  height: 500px;
  background: white;
  border-radius: 6px;
  overflow: hidden;
}

/* HEADER */
.topo {
  height: 70px;
  background: #1e4f67;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.topo h1 {
  letter-spacing: 2px;
}

.voltar {
  position: absolute;
  left: 20px;
  background: none;
  border: none;
  font-size: 24px;
  color: white;
  cursor: pointer;
}

.voltar:hover {
  color: orange;
  cursor: pointer;
  transform: scale(1.2);
}

/* GRID */
.grid {
  height: calc(100% - 70px);
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 50px;
  padding: 40px 100px;
  place-items: center;
}

/* CARDS */
.card {
  width: 150px;
  height: 150px;
  background: #fcb83c;
  border-radius: 25px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 12px;
  cursor: pointer;
  transition: 0.2s;
  text-decoration: none;
  color: inherit;
}

.card:hover {
  transform: scale(1.05);
  background: #f49c38;
  scale: 1.05;
  box-shadow: 0 6px 18px rgba(0,0,0,0.25);
}

.card img {
  width: 40px;
  opacity: 0.7;
  filter: invert(1);
}

.card span {
  font-size: 14px;
}

.card:nth-child(4),
.card:nth-child(5) {
  transform: translateX(80px);
}

.mover {
  position: relative;
  left: 50px;
   transform: translateX(120px);
  transition: 0.2s;
}
.card:hover {
  scale: 1.05;
}

