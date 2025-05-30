<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AruÁ - Festa no Rio São Francisco</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body, html {
      height: 100%;
      font-family: 'Segoe UI', sans-serif;
      background: url('https://i.imgur.com/xsC0jUA.jpeg') no-repeat center center fixed;
      background-size: cover;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle, rgba(0, 0, 0, 0.7) 20%, rgba(0, 0, 0, 0.9) 100%);
      z-index: 0;
    }

    .container {
      position: relative;
      z-index: 1;
      max-width: 600px;
      padding: 2rem;
      background: rgba(0, 0, 0, 0.6);
      border-radius: 20px;
      box-shadow: 0 0 30px rgba(0, 0, 0, 0.6);
    }

    header h1 {
      font-size: 3rem;
      text-align: center;
      color: #e0ff4f;
      margin-bottom: 0.2rem;
    }

    .sub {
      text-align: center;
      font-style: italic;
      color: #d4d4d4;
      margin-bottom: 2rem;
    }

    .intro {
      margin-bottom: 1.5rem;
      color: #eeeeee;
      font-size: 1rem;
      text-align: center;
    }

    label {
      display: block;
      margin-top: 1rem;
      font-weight: bold;
      color: #e8e8e8;
    }

    input, textarea {
      width: 100%;
      padding: 0.8rem;
      margin-top: 0.3rem;
      border: 1px solid #444;
      border-radius: 8px;
      font-size: 1rem;
      background: rgba(255, 255, 255, 0.1);
      color: white;
    }

    button {
      margin-top: 2rem;
      padding: 1rem;
      width: 100%;
      background-color: #e0ff4f;
      color: black;
      border: none;
      border-radius: 10px;
      font-size: 1.1rem;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #c2e63f;
    }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <div class="container">
    <header>
      <h1>AruÁ</h1>
      <p class="sub">A festa mais exclusiva nas águas do Rio São Francisco</p>
    </header>

    <section class="form-section">
      <p class="intro">Você foi indicado. Agora é sua chance de mostrar por que deve viver essa experiência única no coração do Velho Chico.</p>

      <form action="https://formspree.io/f/xqabzbaz" method="POST">
        <label for="nome">Nome completo:</label>
        <input type="text" id="nome" name="nome" required />

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required />

        <label for="telefone">Número de WhatsApp:</label>
        <input type="tel" id="telefone" name="telefone" required />

        <label for="instagram">Perfil do Instagram:</label>
        <input type="text" id="instagram" name="instagram" required />

        <label for="descricao">Por que você merece estar no AruÁ?</label>
        <textarea id="descricao" name="descricao" rows="5" required></textarea>

        <button type="submit">Enviar candidatura</button>
      </form>
    </section>
  </div>
</body>
</html>
