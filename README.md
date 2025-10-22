<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tabiiy Asal | To‘lov sahifasi</title>
  <style>
    body {
      font-family: "Poppins", Arial, sans-serif;
      background-color: #f7f8fa;
      color: #222;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      margin: 0;
    }

    .container {
      text-align: center;
      background: #fff;
      padding: 40px 30px;
      border-radius: 16px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
      max-width: 420px;
      width: 90%;
    }

    img {
      width: 100%;
      max-width: 320px;
      border-radius: 12px;
      margin-bottom: 25px;
    }

    h1 {
      font-size: 1.6em;
      margin-bottom: 10px;
      color: #333;
    }

    .card-number {
      background-color: #f1f3f6;
      padding: 14px 18px;
      border-radius: 8px;
      font-size: 1.2em;
      letter-spacing: 1px;
      display: inline-block;
      margin-bottom: 12px;
    }

    .copy-btn {
      display: inline-block;
      margin-left: 8px;
      padding: 10px 14px;
      background-color: #007bff;
      color: #fff;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.2s ease;
    }

    .copy-btn:hover {
      background-color: #0056b3;
    }

    .pay-buttons {
      margin-top: 25px;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .pay-btn {
      text-decoration: none;
      padding: 14px;
      border-radius: 10px;
      font-weight: 500;
      color: #fff;
      transition: transform 0.2s ease, opacity 0.2s ease;
    }

    .pay-btn:hover {
      transform: translateY(-2px);
      opacity: 0.9;
    }

    .click {
      background-color: #007bff;
    }

    .payme {
      background-color: #00c98d;
    }

    footer {
      margin-top: 25px;
      font-size: 0.9em;
      color: #777;
    }
  </style>
</head>
<body>

  <div class="container">
    <img src="https://i.ibb.co/zwR8kY8/plastik-Tabiiy-Asal.png" alt="Karta rasmi">

    <h1>To‘lov uchun karta raqam</h1>

    <div>
      <span class="card-number" id="cardNumber">9860 1801 0447 5413</span>
      <button class="copy-btn" onclick="copyCard()">📋 Nusxa olish</button>
    </div>

    <div class="pay-buttons">
      <a class="pay-btn click" href="https://my.click.uz/services/pay?service_id=25968&merchant_id=12345&amount=10000" target="_blank">
        🔵 To‘g‘ridan to‘g‘ri to‘lov (Click)
      </a>

      <a class="pay-btn payme" href="https://payme.uz/home/payment" target="_blank">
        🟢 To‘g‘ridan to‘g‘ri to‘lov (Payme)
      </a>
    </div>

    <footer>
      © 2025 Tabiiy Asal
    </footer>
  </div>

  <script>
    function copyCard() {
      const card = document.getElementById("cardNumber").innerText;
      navigator.clipboard.writeText(card);
      alert("Karta raqami nusxalandi: " + card);
    }
  </script>

</body>
</html>
