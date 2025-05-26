<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Loja de Roupas e Tênis</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: #f9f9f9;
      color: #333;
    }

    header {
      background-color: #111;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .container {
      max-width: 1200px;
      margin: 30px auto;
      padding: 0 20px;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .product {
      background: white;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      padding: 20px;
      text-align: center;
    }

    .product img {
      max-width: 100%;
      border-radius: 10px;
    }

    .product h2 {
      font-size: 1.2rem;
      margin: 10px 0;
    }

    .price {
      font-weight: bold;
      margin-bottom: 10px;
      color: #e91e63;
    }

    .buttons {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .buttons form,
    .buttons a {
      text-decoration: none;
    }

    .pix-box {
      background: #e1f5e1;
      padding: 10px;
      border: 1px dashed green;
      border-radius: 8px;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Loja Estilo Urbano</h1>
    <p>Moda casual com estilo e conforto</p>
  </header>

  <div class="container">
    <div class="products">

      <!-- Produto 1 -->
      <div class="product">
        <img src="https://via.placeholder.com/300x200?text=T%C3%AAnis+Preto" alt="Tênis Preto" />
        <h2>Tênis Preto</h2>
        <div class="price">R$ 199,90</div>
        <div class="buttons">
          <!-- PayPal -->
          <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
            <input type="hidden" name="cmd" value="_xclick" />
            <input type="hidden" name="business" value="SEUEMAIL@EXEMPLO.COM" />
            <input type="hidden" name="item_name" value="Tênis Preto" />
            <input type="hidden" name="amount" value="199.90" />
            <input type="hidden" name="currency_code" value="BRL" />
            <input type="submit" value="Comprar com PayPal" />
          </form>

          <!-- Pix -->
          <div class="pix-box">
            <strong>Chave Pix:</strong><br />
            123e4567@pix.com
          </div>
        </div>
      </div>

      <!-- Produto 2 -->
      <div class="product">
        <img src="https://via.placeholder.com/300x200?text=Camiseta+Branca" alt="Camiseta Branca" />
        <h2>Camiseta Branca</h2>
        <div class="price">R$ 89,90</div>
        <div class="buttons">
          <!-- PayPal -->
          <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
            <input type="hidden" name="cmd" value="_xclick" />
            <input type="hidden" name="business" value="SEUEMAIL@EXEMPLO.COM" />
            <input type="hidden" name="item_name" value="Camiseta Branca" />
            <input type="hidden" name="amount" value="89.90" />
            <input type="hidden" name="currency_code" value="BRL" />
            <input type="submit" value="Comprar com PayPal" />
          </form>

          <!-- Pix -->
          <div class="pix-box">
            <strong>Chave Pix:</strong><br />
            123e4567@pix.com
          </div>
        </div>
      </div>

    </div>
  </div>
</body>
</html>
