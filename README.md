<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ateen Gas Point Shop</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f4;
      color: #333;
    }
    header {
      background: #009688;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      background: #00796b;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 20px;
    }
    .card {
      background: white;
      padding: 20px;
      margin: 10px 0;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    footer {
      background: #00796b;
      color: white;
      text-align: center;
      padding: 10px;
      margin-top: 20px;
    }
    button {
      background: #009688;
      color: white;
      border: none;
      padding: 10px 15px;
      cursor: pointer;
      border-radius: 5px;
    }
    button:hover {
      background: #00796b;
    }
    input {
      padding: 8px;
      margin: 5px;
      width: 80%;
    }
  </style>
</head>
<body>

  <header>
    <h1>🚛 Ateen Gas Point Shop</h1>
    <p>Kot Nainana, Tehsil Shakargarh, District Narowal</p>
  </header>

  <nav>
    <a href="#services">Services</a>
    <a href="#spareparts">Spare Parts</a>
    <a href="#booking">Booking</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="services" class="card">
    <h2>Our Services</h2>
    <p>We provide high-quality gas cylinders, refilling, and spare parts for homes and businesses.</p>
  </section>

  <section id="spareparts" class="card">
    <h2>Spare Parts</h2>
    <ul>
      <li>Regulators</li>
      <li>Cocks</li>
      <li>Pipes</li>
      <li>Burners</li>
      <li>Other gas accessories</li>
    </ul>
  </section>

  <section id="booking" class="card">
    <h2>Book a Cylinder</h2>
    <p>Update your inventory below 👇</p>
    <label for="cylinders">Number of Cylinders Available:</label><br>
    <input type="number" id="cylinders" value="10"><br><br>
    <button onclick="bookCylinder()">Book Now on WhatsApp</button>
  </section>

  <section id="contact" class="card">
    <h2>Contact Us</h2>
    <p>📞 0300-6442464</p>
    <p>📞 0336-6442464</p>
    <p>📧 shaziabutt028@gmail.com</p>
    <p>📍 Kot Nainana, Tehsil Shakargarh, District Narowal</p>
  </section>

  <footer>
    <p>&copy; 2025 Ateen Gas Point Shop | All Rights Reserved</p>
  </footer>

  <script>
    function bookCylinder() {
      let quantity = document.getElementById("cylinders").value;
      let phone = "923006442464"; // WhatsApp number without 0
      let message = `Hello! I want to book a gas cylinder. Available cylinders: ${quantity}`;
      window.open(`https://wa.me/${phone}?text=${encodeURIComponent(message)}`, "_blank");
    }
  </script>

</body>
</html>
