<div align="center">

  <!-- 1. HERO BANNER: FREEDOM + ANIMATED BLUE CRESCENT & STAR -->
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 420" width="100%" style="background:#0d1117; border-radius:16px; border:1px solid #00a3e0; box-shadow: 0 0 25px rgba(0, 163, 224, 0.6);">
    <defs>
      <!-- Background Grid -->
      <pattern id="grid" width="30" height="30" patternUnits="userSpaceOnUse">
        <path d="M 30 0 L 0 0 0 30" fill="none" stroke="#00a3e0" stroke-width="0.5" opacity="0.15"/>
      </pattern>

      <!-- Neon Glow Filter -->
      <filter id="neonGlow" x="-30%" y="-30%" width="160%" height="160%">
        <feGaussianBlur stdDeviation="8" result="blur" />
        <feMerge>
          <feMergeNode in="blur" />
          <feMergeNode in="blur" />
          <feMergeNode in="SourceGraphic" />
        </feMerge>
      </filter>

      <!-- Blue Glow Gradient -->
      <linearGradient id="blueGlowGrad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#00f2fe" />
        <stop offset="50%" stop-color="#00a3e0" />
        <stop offset="100%" stop-color="#0066ff" />
      </linearGradient>
    </defs>

    <!-- Background Layer -->
    <rect width="900" height="420" fill="#061826" rx="16"/>
    <rect width="900" height="420" fill="url(#grid)" rx="16"/>

    <!-- Top Badge: AVAILABLE FOR COLLABORATION -->
    <g transform="translate(50, 40)">
      <rect x="0" y="0" width="250" height="30" rx="15" fill="#00a3e0" opacity="0.2" stroke="#00a3e0" stroke-width="1"/>
      <circle cx="20" cy="15" r="4" fill="#00f2fe">
        <animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite" />
      </circle>
      <text x="32" y="19" fill="#00f2fe" font-family="'Segoe UI', Roboto, sans-serif" font-size="11" font-weight="bold" letter-spacing="1">AVAILABLE FOR COLLABORATION</text>
    </g>

    <!-- Subtitle: HELLO WORLD, IT IS -->
    <text x="50" y="110" fill="#00f2fe" font-family="'JetBrains Mono', monospace" font-size="14" font-weight="bold" letter-spacing="2">
      ⚡ HELLO WORLD, IT IS
    </text>

    <!-- MAIN FREEDOM TITLE -->
    <text x="50" y="180" fill="url(#blueGlowGrad)" font-family="'Impact', 'Arial Black', sans-serif" font-size="75" font-weight="900" letter-spacing="4" filter="url(#neonGlow)">
      FREEDOM
      <animate attributeName="opacity" values="0.85;1;0.85" dur="3s" repeatCount="indefinite" />
    </text>

    <!-- Description Lines -->
    <text x="50" y="225" fill="#cbd5e1" font-family="'Segoe UI', Roboto, sans-serif" font-size="15">
      Building open, decentralized, and elegant software experiences.
    </text>
    <text x="50" y="250" fill="#cbd5e1" font-family="'Segoe UI', Roboto, sans-serif" font-size="15">
      Empowering innovation through clean code and modern technology.
    </text>

    <!-- Skill Tags -->
    <g transform="translate(50, 280)">
      <rect x="0" y="0" width="120" height="32" rx="6" fill="#091b29" stroke="#00a3e0" stroke-width="1" opacity="0.8"/>
      <text x="60" y="21" fill="#00f2fe" font-family="monospace" font-size="12" text-anchor="middle">&lt;CleanCode /&gt;</text>

      <rect x="130" y="0" width="110" height="32" rx="6" fill="#091b29" stroke="#00a3e0" stroke-width="1" opacity="0.8"/>
      <text x="185" y="21" fill="#00f2fe" font-family="sans-serif" font-size="12" text-anchor="middle">Modern Web</text>

      <rect x="250" y="0" width="110" height="32" rx="6" fill="#091b29" stroke="#0066ff" stroke-width="1" opacity="0.8"/>
      <text x="305" y="21" fill="#93c5fd" font-family="sans-serif" font-size="12" text-anchor="middle">Open Source</text>
    </g>

    <!-- RIGHT SIDE: ANIMATED BLUE UYGHUR CRESCENT & STAR -->
    <g transform="translate(680, 200)" filter="url(#neonGlow)">
      <!-- Floating Movement -->
      <animateTransform attributeName="transform" type="translate" values="680,190; 680,210; 680,190" dur="5s" repeatCount="indefinite"/>

      <!-- Rotating Outer Radar Rings -->
      <circle cx="0" cy="0" r="100" fill="none" stroke="#00a3e0" stroke-width="1" opacity="0.25"/>
      <circle cx="0" cy="0" r="80" fill="none" stroke="#00a3e0" stroke-width="1.5" stroke-dasharray="6,10" opacity="0.5">
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="25s" repeatCount="indefinite"/>
      </circle>

      <!-- Crescent Moon (ئاي) -->
      <path d="M 15 -60 A 60 60 0 1 0 15 60 A 48 48 0 1 1 15 -60 Z" fill="url(#blueGlowGrad)" />

      <!-- Spinning Star (يۇلتۇز) -->
      <g transform="translate(35, -5)">
        <polygon points="12,-16 15,-3 28,0 18,8 21,20 12,13 3,20 6,8 -4,0 9,-3" fill="url(#blueGlowGrad)">
          <animateTransform attributeName="transform" type="rotate" from="0" to="360" cx="12" cy="0" dur="15s" repeatCount="indefinite"/>
        </polygon>
      </g>
    </g>

    <!-- Bottom Status Text -->
    <text x="50" y="385" fill="#00f2fe" font-family="monospace" font-size="11" opacity="0.9">• SYS.STATUS // ONLINE &amp; CREATING</text>
    <text x="850" y="385" fill="#94a3b8" font-family="monospace" font-size="11" text-anchor="end">EAST TURKESTAN // 2026</text>
  </svg>

  <br/><br/>

  <!-- 2. LIVE BADGES -->
  <p align="center">
    <img src="https://komarev.com/ghpvc/?username=Uy-Freedom&label=PROFILE%20VIEWS&color=00a3e0&style=for-the-badge&labelColor=161b22" alt="Views" />
    <img src="https://img.shields.io/github/followers/Uy-Freedom?label=FOLLOWERS&style=for-the-badge&color=0066ff&labelColor=161b22&logo=github" alt="Followers" />
    <img src="https://img.shields.io/badge/STATUS-ACTIVELY%20CODING-10b981?style=for-the-badge&labelColor=161b22" alt="Status" />
  </p>

</div>

<br/>

<!-- 3. ABOUT ME -->
### 👤 About Freedom
- 🌙 **Developing modern digital products with a focus on freedom, decentralization, and privacy.**
- 🚀 **Building scalable web applications, UI/UX designs, and cloud infrastructure.**
- 🌱 **Continuous learner in AI models, Web3 technologies, and interactive visual designs.**
- 💬 **Let's collaborate on high-impact open-source projects!**

<br/>

<!-- 4. TECH STACK -->
### ⚡ Tech Stack & Tools
<p align="left">
  <img src="https://img.shields.io/badge/React.js-00d2ff?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/JavaScript%2FTS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-38bdf8?style=for-the-badge&logo=tailwindcss&logoColor=black" />
  <img src="https://img.shields.io/badge/Node.js-22c55e?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Git%20%26%20GitHub-f97316?style=for-the-badge&logo=git&logoColor=white" />
</p>

<br/>

<!-- 5. GITHUB STATISTICS -->
### 📊 GitHub Statistics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Uy-Freedom&show_icons=true&theme=tokyonight&bg_color=090d16&title_color=00f2fe&text_color=cbd5e1&border_color=00a3e0" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Uy-Freedom&layout=compact&theme=tokyonight&bg_color=090d16&title_color=00f2fe&text_color=cbd5e1&border_color=00a3e0" width="48%" />
</p>
