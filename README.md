<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ganhe Revendendo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f5f5f5;
      text-align: center;
      transition: 0.3s;
    }

    header {
      background-color: #222;
      color: white;
      padding: 20px;
    }

    .buttons {
      margin-top: 15px;
    }

    .buttons button {
      margin: 0 10px;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
      background-color: #ff9800;
      color: white;
      transition: 0.3s;
    }

    .buttons button:hover {
      background-color: #e68900;
    }

    .container {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      margin: 40px 0;
    }

    .card {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      width: 220px;
      padding: 20px;
      text-align: center;
      transition: transform 0.2s;
    }

    .card:hover {
      transform: scale(1.03);
    }

    .card img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 15px;
    }

    .card h3 {
      margin-bottom: 10px;
    }

    .price {
      font-size: 20px;
      font-weight: bold;
      color: #333;
      margin-bottom: 15px;
    }

    .card button {
      background-color: #ff9800;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 6px;
      cursor: pointer;
      transition: 0.3s;
    }

    .card button:hover {
      background-color: #e68900;
    }

    /* Modo COMPRAR */
    .comprar {
      background-color: #007bff;
    }

    .comprar .card button {
      background-color: #004aad;
    }

    .comprar .card button:hover {
      background-color: #003d8f;
    }
  </style>
</head>
<body>

  <header>
    <h1>Ganhe Revendendo</h1>
    <div class="buttons">
      <button onclick="mostrar('revender')">Revender</button>
      <button onclick="mostrar('comprar')">Comprar</button>
    </div>
  </header>

  <div id="conteudo" class="container"></div>

  <script>
    const numero = "558396056952"; // seu WhatsApp no formato internacional

    function mostrar(tipo) {
      const conteudo = document.getElementById("conteudo");
      const produtos = [
        { 
          nome: "Relógio Digital", 
          preco: "R$80", 
          imagem: "https://images.unsplash.com/photo-1512499617640-c2f999098b96?auto=format&fit=crop&w=400&q=80"
        },
        { 
          nome: "Videogame Portátil", 
          preco: "R$70", 
          imagem: "https://images.unsplash.com/photo-1593642532744-d377ab507dc8?auto=format&fit=crop&w=400&q=80"
        }
      ];

      document.body.classList.toggle('comprar', tipo === 'comprar');

      let html = "";
      produtos.forEach(p => {
        const mensagem = encodeURIComponent(`Olá! Quero ${tipo === 'comprar' ? 'comprar' : 'revender'} o ${p.nome}.`);
        const link = `https://wa.me/${numero}?text=${mensagem}`;
        html += `
          <div class="card">
            <img src="${p.imagem}" alt="${p.nome}">
            <h3>${p.nome}</h3>
            <div class="price"

[site.txt](https://github.com/user-attachments/files/23338666/site.txt)
