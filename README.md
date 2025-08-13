‏<!DOCTYPE html>
‏<html lang="ar">
‏<head>
‏  <meta charset="UTF-8">
‏  <meta name="viewport" content="width=device-width, initial-scale=1.0">
‏  <title>مركز بلو</title>
‏  <style>
‏    body {
‏      margin: 0;
‏      font-family: Arial, sans-serif;
‏      background: linear-gradient(120deg, #1E90FF, #00BFFF, #1E90FF);
‏      background-size: 400% 400%;
‏      color: #fff;
‏      animation: gradientBG 15s ease infinite;
    }

‏    @keyframes gradientBG {
‏      0% {background-position:0% 50%;}
‏      50% {background-position:100% 50%;}
‏      100% {background-position:0% 50%;}
    }

‏    header {
‏      display: flex;
‏      justify-content: space-between;
‏      align-items: center;
‏      padding: 20px;
‏      background-color: rgba(24,123,205,0.8);
‏      position: relative;
‏      overflow: hidden;
    }

‏    #logo {
‏      height: 60px;
    }

‏    .butterfly {
‏      position: absolute;
‏      width: 60px;
‏      height: 60px;
‏      background-image: url('butterfly.png');
‏      background-size: contain;
‏      background-repeat: no-repeat;
‏      animation: flyRandom 8s infinite;
    }

‏    @keyframes flyRandom {
‏      0% {transform: translate(0,0) rotate(0deg);}
‏      25% {transform: translate(60px,-30px) rotate(15deg);}
‏      50% {transform: translate(120px,20px) rotate(-10deg);}
‏      75% {transform: translate(60px,50px) rotate(10deg);}
‏      100% {transform: translate(0,0) rotate(0deg);}
    }

‏    nav {
‏      display: flex;
‏      justify-content: center;
‏      gap: 40px;
‏      margin-top: 20px;
    }

‏    nav a {
‏      text-decoration: none;
‏      color: #fff;
‏      font-size: 18px;
‏      padding: 5px 15px;
‏      border-radius: 5px;
‏      transition: background 0.3s;
    }

‏    nav a:hover {
‏      background-color: rgba(255,255,255,0.2);
    }

‏    section {
‏      padding: 20px;
    }

‏    h2 {
‏      border-bottom: 2px solid #fff;
‏      padding-bottom: 5px;
‏      margin-bottom: 15px;
    }

‏    .menu-grid {
‏      display: grid;
‏      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
‏      gap: 15px;
    }

‏    .menu-item {
‏      background-color: rgba(255,255,255,0.1);
‏      padding: 15px;
‏      border-radius: 10px;
‏      text-align: center;
‏      transition: transform 0.3s, background 0.3s, box-shadow 0.3s;
‏      cursor: pointer;
    }

‏    .menu-item:hover {
‏      background-color: rgba(255,255,255,0.3);
‏      transform: translateY(-5px);
‏      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }

    /* الباركود */
‏    .barcode {
‏      margin-top: 30px;
‏      text-align: center;
    }

‏    .barcode img {
‏      width: 200px;
‏      height: auto;
    }
‏  </style>
‏</head>
‏<body>
‏  <header>
‏    <img id="logo" src="logo.png" alt="لوغو المركز">
‏    <div class="butterfly"></div>
‏  </header>

‏  <nav>
‏    <a href="#hot">مشروبات ساخنة</a>
‏    <a href="#cold">مشروبات باردة</a>
‏  </nav>

‏  <section id="hot">
‏    <h2>مشروبات ساخنة</h2>
‏    <div class="menu-grid">
‏      <div class="menu-item">قهوة أمريكية</div>
‏      <div class="menu-item">اسبريسو</div>
‏      <div class="menu-item">شاي أخضر</div>
‏      <div class="menu-item">لاتيه</div>
‏      <div class="menu-item">كابتشينو</div>
‏    </div>
‏  </section>

‏  <section id="cold">
‏    <h2>مشروبات باردة</h2>
‏    <div class="menu-grid">
‏      <div class="menu-item">آيس لاتيه</div>
‏      <div class="menu-item">موهيتو مثلج</div>
‏      <div class="menu-item">عصير برتقال</div>
‏      <div class="menu-item">سموذي فراولة</div>
‏      <div class="menu-item">شاي مثلج</div>
‏    </div>
‏  </section>

  <!-- الباركود -->
‏  <div class="barcode">
‏    <img src="barcode.png" alt="باركود المركز">
‏  </div>
‏</body>
‏</html>
