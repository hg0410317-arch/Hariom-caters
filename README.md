# Hariom-caters
Hariom Caterers Booking Website
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hariom Caterers</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f7f7f7;
      color: #222;
    }

    header {
      background: #111;
      color: white;
      padding: 25px 20px;
      text-align: center;
    }

    header h1 {
      font-size: 30px;
      margin-bottom: 8px;
    }

    header p {
      color: #ddd;
    }

    .hero {
      padding: 45px 20px;
      text-align: center;
      background: white;
    }

    .hero h2 {
      font-size: 28px;
      margin-bottom: 12px;
    }

    .hero p {
      color: #555;
      margin-bottom: 25px;
    }

    .btn {
      display: inline-block;
      background: #25D366;
      color: white;
      padding: 14px 24px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }

    .section {
      padding: 35px 20px;
      max-width: 900px;
      margin: auto;
    }

    .section h2 {
      text-align: center;
      margin-bottom: 25px;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 15px;
    }

    .card {
      background: white;
      padding: 22px;
      border-radius: 12px;
      box-shadow: 0 3px 12px rgba(0,0,0,0.08);
      text-align: center;
    }

    .card h3 {
      margin-bottom: 10px;
    }

    form {
      background: white;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 3px 12px rgba(0,0,0,0.08);
    }

    input, select, textarea {
      width: 100%;
      padding: 13px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 7px;
      font-size: 16px;
    }

    textarea {
      height: 100px;
      resize: none;
    }

    button {
      width: 100%;
      padding: 14px;
      background: #25D366;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 17px;
      font-weight: bold;
      cursor: pointer;
    }

    footer {
      background: #111;
      color: white;
      text-align: center;
      padding: 25px;
      margin-top: 20px;
    }
  </style>
</head>

<body>

  <header>
    <h1>🍽️ Hariom Caterers</h1>
    <p>Make Your Events Delicious</p>
  </header>

  <section class="hero">
    <h2>Har Event Ke Liye Catering</h2>
    <p>Wedding • Birthday • Party • Function • Corporate Events</p>

    <a class="btn"
       href="https://wa.me/917805071012"
       target="_blank">
       📲 WhatsApp Booking
    </a>
  </section>

  <section class="section">
    <h2>Our Services</h2>

    <div class="services">

      <div class="card">
        <h3>💍 Wedding Catering</h3>
        <p>Shaadi aur reception ke liye complete catering service.</p>
      </div>

      <div class="card">
        <h3>🎂 Birthday Party</h3>
        <p>Birthday aur small parties ke liye delicious food.</p>
      </div>

      <div class="card">
        <h3>🏢 Corporate Events</h3>
        <p>Office events aur corporate functions ke liye catering.</p>
      </div>

      <div class="card">
        <h3>🍛 All Types of Catering</h3>
        <p>Aapke event ke according customized catering.</p>
      </div>

    </div>
  </section>

  <section class="section">
    <h2>📋 Booking Request</h2>

    <form id="bookingForm">

      <input type="text" id="name"
             placeholder="Aapka Naam" required>

      <input type="tel" id="phone"
             placeholder="Mobile Number" required>

      <select id="event" required>
        <option value="">Event Select Kare</option>
        <option>Wedding</option>
        <option>Birthday</option>
        <option>Party</option>
        <option>Corporate Event</option>
        <option>Other</option>
      </select>

      <input type="date" id="date" required>

      <input type="number" id="guests"
             placeholder="Kitne Guests?" required>

      <textarea id="message"
                placeholder="Extra Details"></textarea>

      <button type="submit">
        WhatsApp Par Booking Bheje
      </button>

    </form>
  </section>

  <footer>
    <p>© 2026 Hariom Caterers</p>
    <p>All Types of Catering Available</p>
  </footer>

  <script>
    document.getElementById("bookingForm").addEventListener("submit", function(e) {

      e.preventDefault();

      const name = document.getElementById("name").value;
      const phone = document.getElementById("phone").value;
      const event = document.getElementById("event").value;
      const date = document.getElementById("date").value;
      const guests = document.getElementById("guests").value;
      const message = document.getElementById("message").value;

      const whatsappNumber = "919XXXXXXXXX";

      const text =
        "🍽️ *Hariom Caterers Booking Request*%0A%0A" +
        "👤 Name: " + name + "%0A" +
        "📞 Mobile: " + phone + "%0A" +
        "🎉 Event: " + event + "%0A" +
        "📅 Date: " + date + "%0A" +
        "👥 Guests: " + guests + "%0A" +
        "📝 Details: " + message;

      window.open(
        "https://wa.me/" + whatsappNumber + "?text=" + text,
        "_blank"
      );
    });
  </script>

</body>
</html>