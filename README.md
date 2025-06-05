<!DOCTYPE html><html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Dharam Pipra - A Smart Village App</title>
    <style>
      body {
        background-color: #111;
        color: #eee;
        font-family: 'Segoe UI', sans-serif;
        margin: 0;
        padding: 0;
      }
      header {
        background-color: #222;
        padding: 1rem;
        text-align: center;
      }
      header h1 {
        margin: 0;
        font-size: 2rem;
      }
      .section {
        padding: 1rem;
        border-bottom: 1px solid #333;
      }
      .card {
        background: #1c1c1c;
        padding: 1rem;
        border-radius: 10px;
        margin-bottom: 1rem;
        box-shadow: 0 0 10px rgba(0,0,0,0.3);
      }
      footer {
        background-color: #111;
        text-align: center;
        padding: 1rem;
        font-size: 0.9rem;
        color: #aaa;
      }
      .lang-toggle {
        float: right;
        margin-top: -2rem;
        margin-right: 1rem;
      }
    </style>
  </head>
  <body>
    <!-- Splash Screen -->
    <div id="splash" style="
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: #000;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      color: #fff;
      z-index: 1000;
    ">
      <img src="hanumanji.png" alt="Hanuman Ji" width="150" />
      <h1>Dharam Pipra</h1>
      <h3>A Smart Village App</h3>
      <p style="position: absolute; bottom: 1rem; font-size: 0.9rem;">Powered by Dharam Pipra Community</p>
    </div><!-- Language Toggle -->
<div class="lang-toggle">
  <select onchange="switchLang(this.value)">
    <option value="en">English</option>
    <option value="hi">हिंदी</option>
  </select>
</div>

<header>
  <h1>Dharam Pipra Village</h1>
</header>

<main>
  <div class="section">
    <h2>People Directory (800+)</h2>
    <div class="card">Apurv Kumar - ID: 001 - House #A1</div>
    <div class="card">Sita Devi - ID: 002 - House #B5</div>
  </div>

  <div class="section">
    <h2>Houses</h2>
    <div class="card">House A1 - 4 Members</div>
    <div class="card">House B5 - 6 Members</div>
  </div>

  <div class="section">
    <h2>Temple Information</h2>
    <div class="card">Hanuman Mandir - Location: Center of Village</div>
  </div>

  <div class="section">
    <h2>Ceremonies</h2>
    <div class="card">Ram Navami - 17 April</div>
    <div class="card">Diwali Celebration - 4 Nov</div>
  </div>

  <div class="section">
    <h2>Fundraisers</h2>
    <div class="card">Mandir Renovation - ₹25000 collected</div>
    <div class="card">Community Hall Paint - ₹12000 needed</div>
  </div>

  <div class="section">
    <h2>Social Feed</h2>
    <div class="card">Apurv posted: "New event coming soon!"</div>
    <div class="card">Ravi shared photo from Holi 🌈</div>
  </div>
</main>

<footer>
  Powered by Dharam Pipra Community
</footer>

<audio autoplay loop>
  <source src="hanuman_chalisa_instrumental.mp3" type="audio/mpeg" />
</audio>

<script>
  window.onload = function () {
    setTimeout(() => {
      document.getElementById('splash').style.display = 'none';
    }, 3000);
  };

  function switchLang(lang) {
    alert('Language switched to: ' + lang);
    // Add actual translations if needed
  }
</script>

  </body>
</html>
