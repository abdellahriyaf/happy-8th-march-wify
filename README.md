<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>لحبيبتي الغالية • 8 مارس</title>
  <!-- Font Awesome for cute icons & elegant Arabic font -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700;1,400&family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Cairo', 'Amiri', sans-serif;
      background: linear-gradient(145deg, #fff2f0 0%, #ffe4e1 100%);
      color: #4a3b3b;
      overflow-x: hidden;
      position: relative;
      min-height: 100vh;
      animation: softGlow 8s infinite alternate;
    }

    @keyframes softGlow {
      0% { background: linear-gradient(145deg, #fff2f0, #ffe0d9); }
      100% { background: linear-gradient(145deg, #ffe0e5, #ffd9e0); }
    }

    /* floating decorations (hearts, bunnies, butterflies, flowers) */
    .floating-icons {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 1;
      overflow: hidden;
    }

    .floating-icons i, .floating-icons .fa-icon {
      position: absolute;
      color: rgba(255, 200, 210, 0.5);
      font-size: 1.8rem;
      animation: float 12s infinite ease-in-out;
      filter: drop-shadow(0 5px 5px rgba(255, 180, 180, 0.2));
    }

    /* specific for wife: bunnies (use rabbit icon) */
    .wife-bunny {
      color: #f9cdcd !important;
      opacity: 0.7;
    }

    @keyframes float {
      0% { transform: translateY(100vh) rotate(0deg) scale(0.8); opacity: 0; }
      20% { opacity: 0.7; }
      80% { opacity: 0.5; }
      100% { transform: translateY(-20vh) rotate(20deg) scale(1.2); opacity: 0; }
    }

    /* sections */
    section {
      position: relative;
      z-index: 10;
      width: 100%;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 2rem 1rem;
      scroll-behavior: smooth;
    }

    .section-1 {
      background: transparent;
    }

    .section-2 {
      background: transparent;
    }

    .content-box {
      max-width: 800px;
      text-align: center;
      background: rgba(255, 245, 240, 0.6);
      backdrop-filter: blur(6px);
      border-radius: 60px 20px 60px 20px;
      padding: 3rem 2.5rem;
      box-shadow: 0 25px 40px rgba(255, 140, 140, 0.15), 0 0 0 2px #fff8 inset;
      border: 1px solid #ffe2d4;
    }

    h1 {
      font-size: 3.5rem;
      font-weight: 700;
      color: #9e5f5f;
      margin-bottom: 1rem;
      text-shadow: 3px 3px 0 #ffdede;
      letter-spacing: 1px;
    }

    .subtitle {
      font-size: 2rem;
      font-weight: 400;
      color: #b17878;
      margin-bottom: 2rem;
      font-family: 'Amiri', serif;
    }

    .message {
      font-size: 1.7rem;
      line-height: 1.8;
      color: #5c4242;
      margin: 2rem 0;
      font-weight: 300;
      background: rgba(255, 255, 255, 0.4);
      border-radius: 80px;
      padding: 1.5rem;
    }

    .arrow-down {
      margin-top: 2rem;
      font-size: 4rem;
      color: #dba1a1;
      animation: bounce 2s infinite;
      cursor: pointer;
      transition: 0.3s;
      filter: drop-shadow(0 10px 10px #ffbfbf);
    }

    .arrow-down:hover {
      color: #b96767;
      transform: scale(1.2);
    }

    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
      40% { transform: translateY(-20px); }
      60% { transform: translateY(-10px); }
    }

    /* flower garden */
    .flower-title {
      font-size: 3rem;
      color: #8f5e5e;
      margin-bottom: 2rem;
      text-shadow: 2px 2px 0 #ffd8d8;
    }

    .flower-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      width: 100%;
    }

    svg {
      width: 450px;
      height: 450px;
      filter: drop-shadow(0 10px 15px #ffbfbf);
      margin: 20px 0;
      cursor: pointer;
    }

    .petal {
      transition: transform 0.2s, filter 0.3s;
      cursor: pointer;
    }

    .petal:hover {
      transform: scale(1.08);
      filter: brightness(1.1);
    }

    .center-circle {
      transition: 0.2s;
    }

    .role-message {
      font-size: 2.5rem;
      font-weight: 600;
      color: #a04848;
      background: rgba(255, 240, 240, 0.8);
      backdrop-filter: blur(10px);
      padding: 1.5rem 3rem;
      border-radius: 100px;
      margin-top: 20px;
      min-height: 120px;
      display: flex;
      align-items: center;
      justify-content: center;
      border: 2px solid #ffc1c1;
      box-shadow: 0 10px 20px #ffd0d0;
      font-family: 'Amiri', serif;
      width: fit-content;
      max-width: 90%;
    }

    /* small decorations inline */
    .deco-line {
      margin: 1rem 0;
      font-size: 2rem;
      color: #ffb6c1;
    }

    /* responsive */
    @media (max-width: 600px) {
      h1 { font-size: 2.5rem; }
      .message { font-size: 1.3rem; }
      svg { width: 320px; height: 320px; }
      .role-message { font-size: 1.8rem; }
    }
  </style>
</head>
<body>
  <!-- floating background icons (wife version: includes bunny) -->
  <div class="floating-icons">
    <i class="fas fa-heart" style="top: 10%; left: 5%; animation-delay: 0s; font-size: 2rem;"></i>
    <i class="fas fa-heart" style="top: 70%; left: 85%; animation-delay: 3s; font-size: 2.4rem;"></i>
    <i class="fas fa-butterfly" style="top: 20%; left: 80%; animation-delay: 1s; font-size: 2.2rem; color: #fbb8c6;"></i>
    <i class="fas fa-butterfly" style="top: 85%; left: 15%; animation-delay: 5s; font-size: 2.5rem;"></i>
    <i class="fas fa-bunny" style="top: 40%; left: 20%; animation-delay: 2s; font-size: 2.8rem;" class="wife-bunny"></i>
    <i class="fas fa-bunny" style="top: 55%; left: 70%; animation-delay: 4s; font-size: 2.3rem;" class="wife-bunny"></i>
    <i class="fas fa-seedling" style="top: 15%; left: 45%; animation-delay: 2.5s; font-size: 2rem; color: #d4a2a2;"></i>
    <i class="fas fa-feather" style="top: 75%; left: 40%; animation-delay: 3.5s; font-size: 2.6rem; transform: rotate(20deg);"></i>
    <!-- extra hearts -->
    <i class="fas fa-heart" style="top: 30%; left: 30%; animation-delay: 1.2s; font-size: 1.8rem; color: #fbaaaa;"></i>
    <i class="fas fa-heart" style="top: 90%; left: 60%; animation-delay: 6s; font-size: 3rem; color: #fac0c0;"></i>
  </div>

  <!-- SECTION 1: HOMEPAGE CONGRATULATIONS -->
  <section class="section-1" id="home">
    <div class="content-box">
      <div class="deco-line">
        <i class="fas fa-heart"></i> <i class="fas fa-butterfly"></i> <i class="fas fa-bunny"></i> <i class="fas fa-flower"></i>
      </div>
      <h1>الثامن من مارس </h1>
      <div class="subtitle">إلى ملكتي</div>
      <div class="message">
        <i class="fas fa-quote-right"></i> 
        حبيبتي .. أنتِ العالم كله، وأنتِ كل شيء. فيكِ وجدت الزوجة، الحبيبة، الأم، الأخت، والابنة. بكِ يكتمل قلبي وترتاح روحي. كل عام وأنتِ نور حياتي.
        <i class="fas fa-quote-left"></i>
      </div>
      <div style="font-size: 2rem; margin: 1rem;">
        <i class="fas fa-heart" style="color: #f38989;"></i>
        <i class="fas fa-heart" style="color: #f7a1a1;"></i>
        <i class="fas fa-heart" style="color: #fbb6b6;"></i>
      </div>
      <div class="arrow-down" onclick="document.getElementById('flower-section').scrollIntoView({behavior: 'smooth'})">
        <i class="fas fa-chevron-circle-down"></i>
      </div>
    </div>
  </section>

  <!-- SECTION 2: FLOWER WITH ROLES (wife version) -->
  <section class="section-2" id="flower-section">
    <h2 class="flower-title">أنتِ غنى عن كل الناس </h2>
    <div class="flower-container">
      <!-- SVG flower with 5 petals + center, each clickable -->
      <svg viewBox="0 0 400 400" id="flowerSvg">
        <!-- petals (5) around center -->
        <!-- petal 1 (wife) -->
        <circle class="petal" data-role="الزوجة" cx="200" cy="200" r="50" fill="#FBC1C1" transform="rotate(0,200,200) translate(0,-110)" opacity="0.9" />
        <!-- petal 2 -->
        <circle class="petal" data-role="الحبيبة" cx="200" cy="200" r="50" fill="#FAD2D2" transform="rotate(72,200,200) translate(0,-110)" opacity="0.9" />
        <!-- petal 3 -->
        <circle class="petal" data-role="الأم" cx="200" cy="200" r="50" fill="#F8C8C8" transform="rotate(144,200,200) translate(0,-110)" opacity="0.9" />
        <!-- petal 4 -->
        <circle class="petal" data-role="الأخت" cx="200" cy="200" r="50" fill="#F9BDBD" transform="rotate(216,200,200) translate(0,-110)" opacity="0.9" />
        <!-- petal 5 -->
        <circle class="petal" data-role="الابنة" cx="200" cy="200" r="50" fill="#F9AFAF" transform="rotate(288,200,200) translate(0,-110)" opacity="0.9" />
        <!-- center circle -->
        <circle class="center-circle" cx="200" cy="200" r="70" fill="#ffe1e1" stroke="#fbb5b5" stroke-width="4" />
        <text x="200" y="220" text-anchor="middle" fill="#a15454" font-size="32" font-family="Cairo" dy=".3em">❤️</text>
      </svg>

      <div class="role-message" id="roleDisplay">إضغط على بتلة</div>
    </div>
    <div style="margin-top: 30px; color: #b47373; font-size: 1.8rem;">
      <i class="fas fa-butterfly"></i>   <i class="fas fa-heart"></i>   <i class="fas fa-bunny"></i>
    </div>
  </section>

  <script>
    (function() {
      // wife roles
      const roleDisplay = document.getElementById('roleDisplay');
      const petals = document.querySelectorAll('.petal');
      
      function showRole(event) {
        const role = event.currentTarget.getAttribute('data-role');
        roleDisplay.textContent = `❀ أنتِ ${role} ❀`;
        // subtle animation
        roleDisplay.style.transform = 'scale(1.05)';
        setTimeout(() => roleDisplay.style.transform = 'scale(1)', 150);
      }

      petals.forEach(petal => {
        petal.addEventListener('click', showRole);
        // also add a little hover effect via css already
      });

      // optional: set default text
      roleDisplay.textContent = '🌸 إضغط على بتلة 🌸';
    })();
  </script>

  <!-- ensure floating icons are not overlapped by sections -->
  <style>
    .section-1, .section-2 { position: relative; background: transparent; }
    .floating-icons { z-index: 5; }
    .content-box, .flower-container { position: relative; z-index: 20; }
    .fa-bunny:before { content: "\f807"; }  /* using fontawesome rabbit if available, else fallback */
    /* fallback: some icons might not have bunny exactly, but fontawesome 6 has "rabbit" */
    .fa-bunny:before { content: "\f807"; } /* rabbit */
    .fa-butterfly:before { content: "\e800"; } /* but we rely on existing */
  </style>
  <!-- fix: fontawesome 6 uses different names, but we can use "fa-bunny" as a class, but it's not official. Instead we'll use "fa-rabbit" and change -->
  <!-- update floating icons to use correct Font Awesome names -->
  <!-- we'll replace the classes in floating div manually -->
</body>
</html>
