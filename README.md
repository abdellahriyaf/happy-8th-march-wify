<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>لحبيبتي • 8 مارس</title>
  <!-- Font Awesome for icons & elegant Arabic fonts -->
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

    .floating-icons i {
      position: absolute;
      color: rgba(255, 180, 180, 0.5);
      font-size: 2rem;
      animation: float 14s infinite ease-in-out;
      filter: drop-shadow(0 5px 8px #ffc0c0);
    }

    @keyframes float {
      0% { transform: translateY(110vh) rotate(0deg) scale(0.8); opacity: 0; }
      20% { opacity: 0.8; }
      80% { opacity: 0.6; }
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
      margin-bottom: 1.5rem;
      text-shadow: 2px 2px 0 #ffd8d8;
    }

    .flower-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      width: 100%;
    }

    /* improved SVG flower */
    svg {
      width: 480px;
      height: 480px;
      filter: drop-shadow(0 12px 20px #ffb3b3);
      margin: 10px 0;
    }

    .petal {
      transition: transform 0.2s, filter 0.2s;
      cursor: pointer;
    }

    .petal:hover {
      transform: scale(1.08);
      filter: brightness(1.1) saturate(1.3);
    }

    .center-circle {
      pointer-events: none; /* so clicks pass through to petals */
    }

    .role-message {
      font-size: 2.5rem;
      font-weight: 600;
      color: #a04848;
      background: rgba(255, 240, 240, 0.8);
      backdrop-filter: blur(10px);
      padding: 1.5rem 3rem;
      border-radius: 100px;
      margin-top: 30px;
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

    .deco-line {
      margin: 1rem 0;
      font-size: 2rem;
      color: #ffb6c1;
    }

    /* responsive */
    @media (max-width: 600px) {
      h1 { font-size: 2.5rem; }
      .message { font-size: 1.3rem; }
      svg { width: 350px; height: 350px; }
      .role-message { font-size: 1.8rem; }
    }
  </style>
</head>
<body>
  <!-- floating background icons (wife version: includes bunny/rabbit) -->
  <div class="floating-icons">
    <i class="fas fa-heart" style="top: 10%; left: 5%; animation-delay: 0s;"></i>
    <i class="fas fa-heart" style="top: 70%; left: 85%; animation-delay: 3s;"></i>
    <i class="fas fa-butterfly" style="top: 20%; left: 80%; animation-delay: 1s; color: #fbb8c6;"></i>
    <i class="fas fa-butterfly" style="top: 85%; left: 15%; animation-delay: 5s;"></i>
    <i class="fas fa-rabbit" style="top: 40%; left: 20%; animation-delay: 2s; color: #f9cdcd;"></i>
    <i class="fas fa-rabbit" style="top: 55%; left: 70%; animation-delay: 4s; color: #f9cdcd;"></i>
    <i class="fas fa-feather" style="top: 15%; left: 45%; animation-delay: 2.5s;"></i>
    <i class="fas fa-feather" style="top: 75%; left: 40%; animation-delay: 3.5s;"></i>
    <i class="fas fa-heart" style="top: 30%; left: 30%; animation-delay: 1.2s;"></i>
    <i class="fas fa-heart" style="top: 90%; left: 60%; animation-delay: 6s;"></i>
  </div>

  <!-- SECTION 1: HOMEPAGE CONGRATULATIONS (updated to habibati) -->
  <section class="section-1" id="home">
    <div class="content-box">
      <div class="deco-line">
        <i class="fas fa-heart"></i> <i class="fas fa-butterfly"></i> <i class="fas fa-rabbit"></i> <i class="fas fa-flower"></i>
      </div>
      <h1>يوم المرأة العالمي</h1>
      <div class="subtitle">إلى حبيبتي</div>  <!-- changed from ملكتي to حبيبتي, but keeping queen optional; you can revert if you like -->
      <div class="message">
        <i class="fas fa-quote-right"></i> 
        حبيبتي .. أنتِ العالم كله، وأنتِ كل شيء. فيكِ وجدت الحبيبة، الأم، الأخت، والابنة. بكِ يكتمل قلبي وترتاح روحي. كل عام وأنتِ نور حياتي.
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

  <!-- SECTION 2: IMPROVED FLOWER WITH ROLES (habibati version) -->
  <section class="section-2" id="flower-section">
    <h2 class="flower-title">أنتِ كل هذه الأدوار</h2>
    <div class="flower-container">
      <!-- SVG flower with 5 petals + non-clickable center -->
      <svg viewBox="0 0 400 400" id="flowerSvg">
        <!-- define gradients for petals -->
        <defs>
          <radialGradient id="petalGrad1" cx="30%" cy="30%" r="70%">
            <stop offset="0%" stop-color="#fbc1c1" />
            <stop offset="100%" stop-color="#f7a1a1" />
          </radialGradient>
          <radialGradient id="petalGrad2" cx="30%" cy="30%" r="70%">
            <stop offset="0%" stop-color="#fad2d2" />
            <stop offset="100%" stop-color="#f5a9a9" />
          </radialGradient>
          <radialGradient id="petalGrad3" cx="30%" cy="30%" r="70%">
            <stop offset="0%" stop-color="#f8c8c8" />
            <stop offset="100%" stop-color="#f09d9d" />
          </radialGradient>
          <radialGradient id="petalGrad4" cx="30%" cy="30%" r="70%">
            <stop offset="0%" stop-color="#f9bdbd" />
            <stop offset="100%" stop-color="#e99090" />
          </radialGradient>
          <radialGradient id="petalGrad5" cx="30%" cy="30%" r="70%">
            <stop offset="0%" stop-color="#f9afaf" />
            <stop offset="100%" stop-color="#e68383" />
          </radialGradient>
        </defs>

        <!-- petals placed in a circle with larger radius to reduce overlap and distinct click areas -->
        <!-- petal 1 (habibati) changed from wife to حبيبتي -->
        <circle class="petal" data-role="حبيبتي" cx="200" cy="200" r="55" fill="url(#petalGrad1)" transform="rotate(0,200,200) translate(0,-130)" opacity="0.95" />
        <!-- petal 2 -->
        <circle class="petal" data-role="الأم" cx="200" cy="200" r="55" fill="url(#petalGrad2)" transform="rotate(72,200,200) translate(0,-130)" opacity="0.95" />
        <!-- petal 3 -->
        <circle class="petal" data-role="الأخت" cx="200" cy="200" r="55" fill="url(#petalGrad3)" transform="rotate(144,200,200) translate(0,-130)" opacity="0.95" />
        <!-- petal 4 -->
        <circle class="petal" data-role="الابنة" cx="200" cy="200" r="55" fill="url(#petalGrad4)" transform="rotate(216,200,200) translate(0,-130)" opacity="0.95" />
        <!-- petal 5 - we still need 5 roles; we'll use "الحبيبة" but careful not duplicate; maybe use "الصديقة" or keep "الحبيبة" as second? Since we already have حبيبتي as primary, we can set the remaining to other roles: الحبيبة (the lover) is similar but we can use "الصديقة" (friend) or "الملكة" (queen). Let's use "الصديقة" to keep variety. -->
        <circle class="petal" data-role="الصديقة" cx="200" cy="200" r="55" fill="url(#petalGrad5)" transform="rotate(288,200,200) translate(0,-130)" opacity="0.95" />

        <!-- decorative center (stamen) - not clickable -->
        <circle class="center-circle" cx="200" cy="200" r="60" fill="#ffe1e1" stroke="#fbb5b5" stroke-width="3" />
        <circle class="center-circle" cx="200" cy="200" r="40" fill="#ffe8e8" />
        <text class="center-circle" x="200" y="215" text-anchor="middle" fill="#a15454" font-size="30" font-family="Cairo" dy=".3em">❤️</text>
      </svg>

      <div class="role-message" id="roleDisplay">إضغط على بتلة</div>
    </div>
    <div style="margin-top: 30px; color: #b47373; font-size: 1.8rem;">
      <i class="fas fa-butterfly"></i>   <i class="fas fa-heart"></i>   <i class="fas fa-rabbit"></i>
    </div>
  </section>

  <script>
    (function() {
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
      });

      // set default message
      roleDisplay.textContent = '🌸 إضغط على بتلة 🌸';
    })();
  </script>

  <!-- ensure icons display correctly -->
  <style>
    .fa-rabbit:before { content: "\f807"; } /* FontAwesome 6 rabbit */
    .fa-butterfly:before { content: "\e800"; } 
    .fa-feather:before { content: "\f52d"; }
  </style>
</body>
</html>
