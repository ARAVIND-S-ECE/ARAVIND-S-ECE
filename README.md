<svg viewBox="0 0 1200 2800" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="headerGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#667eea;stop-opacity:1">
        <animate attributeName="stop-color" values="#667eea;#764ba2;#667eea" dur="4s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" style="stop-color:#764ba2;stop-opacity:1">
        <animate attributeName="stop-color" values="#764ba2;#f093fb;#764ba2" dur="4s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    
    <linearGradient id="cardGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1a2e;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#16213e;stop-opacity:1"/>
    </linearGradient>

    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <linearGradient id="skillGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#00ff88;stop-opacity:1"/>
    </linearGradient>
  </defs>

  <!-- Background -->
  <rect width="1200" height="2800" fill="#0d1117"/>
  
  <!-- Animated particles -->
  <circle cx="100" cy="100" r="2" fill="#667eea" opacity="0.6">
    <animate attributeName="cy" values="100;800;100" dur="15s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.2;0.6" dur="15s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1000" cy="200" r="2" fill="#f093fb" opacity="0.6">
    <animate attributeName="cy" values="200;900;200" dur="20s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.2;0.6" dur="20s" repeatCount="indefinite"/>
  </circle>
  <circle cx="300" cy="400" r="2" fill="#00d4ff" opacity="0.6">
    <animate attributeName="cy" values="400;1100;400" dur="18s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.2;0.6" dur="18s" repeatCount="indefinite"/>
  </circle>

  <!-- Header Wave -->
  <path d="M 0 80 Q 300 20 600 80 T 1200 80 L 1200 0 L 0 0 Z" fill="url(#headerGradient)">
    <animate attributeName="d" 
      values="M 0 80 Q 300 20 600 80 T 1200 80 L 1200 0 L 0 0 Z;
              M 0 80 Q 300 140 600 80 T 1200 80 L 1200 0 L 0 0 Z;
              M 0 80 Q 300 20 600 80 T 1200 80 L 1200 0 L 0 0 Z"
      dur="6s" repeatCount="indefinite"/>
  </path>

  <!-- Title -->
  <text x="600" y="140" font-family="'Segoe UI', Arial, sans-serif" font-size="48" font-weight="bold" fill="#ffffff" text-anchor="middle">
    Hi 👋, I'm Vishnuvel R
  </text>

  <!-- Subtitle with typing animation -->
  <text x="600" y="190" font-family="'Courier New', monospace" font-size="20" fill="#00ff88" text-anchor="middle" filter="url(#glow)">
    <tspan>Software Developer &amp; Embedded Systems Enthusiast</tspan>
  </text>

  <!-- Role Cards -->
  <rect x="100" y="240" width="1000" height="100" rx="15" fill="url(#cardGradient)" opacity="0.9"/>
  <text x="600" y="275" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0" text-anchor="middle">
    Intern @ L&amp;T (SDLC, ERP) &amp; Audi (Diagnostics, ODIS, VAS)
  </text>
  <text x="600" y="310" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0" text-anchor="middle">
    AUTOSAR Trained (EB Tresos, ARTOP, CANdb++)
  </text>

  <!-- Skills Section Header -->
  <text x="100" y="400" font-family="Arial, sans-serif" font-size="32" font-weight="bold" fill="#ffffff">
    💻 Skill Set
  </text>
  
  <!-- Programming Languages -->
  <rect x="100" y="430" width="330" height="200" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" repeatCount="indefinite"/>
  </rect>
  <text x="265" y="465" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#00d4ff" text-anchor="middle">
    Programming Languages
  </text>
  
  <!-- C Badge -->
  <rect x="140" y="490" width="80" height="35" rx="8" fill="#555555"/>
  <circle cx="160" cy="507" r="8" fill="#A8B9CC"/>
  <text x="185" y="512" font-family="Arial, sans-serif" font-size="14" fill="#ffffff">C</text>
  
  <!-- Embedded C Badge -->
  <rect x="140" y="540" width="130" height="35" rx="8" fill="#555555"/>
  <circle cx="160" cy="557" r="8" fill="#00599C"/>
  <text x="185" y="562" font-family="Arial, sans-serif" font-size="14" fill="#ffffff">Embedded C</text>
  
  <!-- Java Badge -->
  <rect x="290" y="490" width="90" height="35" rx="8" fill="#555555"/>
  <circle cx="310" cy="507" r="8" fill="#007396"/>
  <text x="335" y="512" font-family="Arial, sans-serif" font-size="14" fill="#ffffff">Java</text>

  <!-- Web & Backend -->
  <rect x="460" y="430" width="330" height="200" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" begin="0.5s" repeatCount="indefinite"/>
  </rect>
  <text x="625" y="465" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#00d4ff" text-anchor="middle">
    Web &amp; Backend
  </text>
  
  <!-- Web Tech Badges Row 1 -->
  <rect x="490" y="490" width="75" height="30" rx="6" fill="#E34F26"/>
  <text x="527" y="510" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">HTML</text>
  
  <rect x="575" y="490" width="65" height="30" rx="6" fill="#1572B6"/>
  <text x="607" y="510" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">CSS</text>
  
  <rect x="650" y="490" width="50" height="30" rx="6" fill="#F7DF1E"/>
  <text x="675" y="510" font-family="Arial, sans-serif" font-size="13" fill="#000000" text-anchor="middle">JS</text>
  
  <rect x="710" y="490" width="70" height="30" rx="6" fill="#61DAFB"/>
  <text x="745" y="510" font-family="Arial, sans-serif" font-size="13" fill="#000000" text-anchor="middle">React</text>

  <!-- Row 2 -->
  <rect x="490" y="535" width="100" height="30" rx="6" fill="#38B2AC"/>
  <text x="540" y="555" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Tailwind</text>
  
  <rect x="600" y="535" width="60" height="30" rx="6" fill="#646CFF"/>
  <text x="630" y="555" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Vite</text>
  
  <rect x="670" y="535" width="80" height="30" rx="6" fill="#000000"/>
  <text x="710" y="555" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Three.js</text>

  <!-- Row 3 -->
  <rect x="490" y="580" width="80" height="30" rx="6" fill="#4479A1"/>
  <text x="530" y="600" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">MySQL</text>
  
  <rect x="580" y="580" width="100" height="30" rx="6" fill="#3ECF8E"/>
  <text x="630" y="600" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Supabase</text>

  <!-- Tools & Platforms -->
  <rect x="820" y="430" width="280" height="200" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" begin="1s" repeatCount="indefinite"/>
  </rect>
  <text x="960" y="465" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#00d4ff" text-anchor="middle">
    Tools / Platforms
  </text>
  
  <rect x="850" y="490" width="85" height="30" rx="6" fill="#FB7A24"/>
  <text x="892" y="510" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">XAMPP</text>
  
  <rect x="945" y="490" width="130" height="30" rx="6" fill="#D22128"/>
  <text x="1010" y="510" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Apache Tomcat</text>
  
  <rect x="850" y="535" width="80" height="30" rx="6" fill="#430098"/>
  <text x="890" y="555" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Heroku</text>
  
  <rect x="940" y="535" width="90" height="30" rx="6" fill="#FF4B4B"/>
  <text x="985" y="555" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">Streamlit</text>
  
  <rect x="850" y="580" width="90" height="30" rx="6" fill="#5C3EE8"/>
  <text x="895" y="600" font-family="Arial, sans-serif" font-size="13" fill="#ffffff" text-anchor="middle">OpenCV</text>

  <!-- Microcontrollers -->
  <rect x="100" y="660" width="520" height="180" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <text x="360" y="695" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#00d4ff" text-anchor="middle">
    🔧 Microcontrollers / Boards
  </text>
  
  <rect x="140" y="720" width="80" height="35" rx="8" fill="#03234B"/>
  <text x="180" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">STM32</text>
  
  <rect x="235" y="720" width="80" height="35" rx="8" fill="#E7352C"/>
  <text x="275" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">ESP32</text>
  
  <rect x="330" y="720" width="120" height="35" rx="8" fill="#C51A4A"/>
  <text x="390" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">Raspberry Pi</text>
  
  <rect x="465" y="720" width="120" height="35" rx="8" fill="#76B900"/>
  <text x="525" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">Jetson Nano</text>
  
  <rect x="235" y="775" width="70" height="35" rx="8" fill="#555555"/>
  <text x="270" y="797" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">8051</text>

  <!-- Automotive Expertise -->
  <rect x="650" y="660" width="450" height="180" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" begin="2s" repeatCount="indefinite"/>
  </rect>
  <text x="875" y="695" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#00d4ff" text-anchor="middle">
    🚗 Automotive Expertise
  </text>
  
  <rect x="690" y="720" width="160" height="35" rx="8" fill="#0066CC"/>
  <text x="770" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">Classic AUTOSAR</text>
  
  <rect x="865" y="720" width="100" height="35" rx="8" fill="#FF6B35"/>
  <text x="915" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">EBtresos</text>
  
  <rect x="980" y="720" width="80" height="35" rx="8" fill="#4CAF50"/>
  <text x="1020" y="742" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">Artop</text>
  
  <rect x="690" y="775" width="100" height="35" rx="8" fill="#9C27B0"/>
  <text x="740" y="797" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">CANdb+</text>
  
  <rect x="805" y="775" width="180" height="35" rx="8" fill="#FF9800"/>
  <text x="895" y="797" font-family="Arial, sans-serif" font-size="14" fill="#ffffff" text-anchor="middle">Vehicle Diagnostics</text>

  <!-- Achievements Section -->
  <text x="100" y="910" font-family="Arial, sans-serif" font-size="32" font-weight="bold" fill="#ffffff">
    🏆 Achievements
  </text>

  <!-- Achievement 1 -->
  <rect x="100" y="940" width="1000" height="120" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="4s" repeatCount="indefinite"/>
  </rect>
  <circle cx="150" cy="1000" r="30" fill="#FFD700" filter="url(#glow)">
    <animate attributeName="r" values="30;32;30" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="150" y="1010" font-family="Arial, sans-serif" font-size="24" fill="#000000" text-anchor="middle">🥈</text>
  <text x="210" y="985" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#ffffff">
    Runner-up – Startup Arena
  </text>
  <text x="210" y="1015" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0">
    Pragyan'24, NIT Trichy • $250 Award
  </text>

  <!-- Achievement 2 -->
  <rect x="100" y="1080" width="1000" height="120" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="4s" begin="1s" repeatCount="indefinite"/>
  </rect>
  <circle cx="150" cy="1140" r="30" fill="#00A4EF" filter="url(#glow)">
    <animate attributeName="r" values="30;32;30" dur="2s" begin="1s" repeatCount="indefinite"/>
  </circle>
  <text x="150" y="1150" font-family="Arial, sans-serif" font-size="24" fill="#ffffff" text-anchor="middle">🏅</text>
  <text x="210" y="1125" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#ffffff">
    Top 7 Teams – Microsoft Imagine Cup
  </text>
  <text x="210" y="1155" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0">
    India Region • $500 Award
  </text>

  <!-- Achievement 3 -->
  <rect x="100" y="1220" width="1000" height="120" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="4s" begin="2s" repeatCount="indefinite"/>
  </rect>
  <circle cx="150" cy="1280" r="30" fill="#667eea" filter="url(#glow)">
    <animate attributeName="r" values="30;32;30" dur="2s" begin="2s" repeatCount="indefinite"/>
  </circle>
  <text x="150" y="1290" font-family="Arial, sans-serif" font-size="24" fill="#ffffff" text-anchor="middle">🎯</text>
  <text x="210" y="1265" font-family="Arial, sans-serif" font-size="20" font-weight="bold" fill="#ffffff">
    Sponsorship Head – Electrothon 2024
  </text>
  <text x="210" y="1295" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0">
    24-Hour Hackathon at CIT
  </text>

  <!-- Achievement 4 -->
  <rect x="100" y="1360" width="480" height="100" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="4s" begin="3s" repeatCount="indefinite"/>
  </rect>
  <circle cx="150" cy="1410" r="25" fill="#0066CC" filter="url(#glow)">
    <animate attributeName="r" values="25;27;25" dur="2s" begin="3s" repeatCount="indefinite"/>
  </circle>
  <text x="150" y="1418" font-family="Arial, sans-serif" font-size="20" fill="#ffffff" text-anchor="middle">📜</text>
  <text x="200" y="1405" font-family="Arial, sans-serif" font-size="18" font-weight="bold" fill="#ffffff">
    Classic AUTOSAR Training
  </text>
  <text x="200" y="1430" font-family="Arial, sans-serif" font-size="15" fill="#a0a0a0">
    Completed from Ancit
  </text>

  <!-- Achievement 5 -->
  <rect x="620" y="1360" width="480" height="100" rx="15" fill="url(#cardGradient)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="4s" begin="3.5s" repeatCount="indefinite"/>
  </rect>
  <circle cx="670" cy="1410" r="25" fill="#0077B5" filter="url(#glow)">
    <animate attributeName="r" values="25;27;25" dur="2s" begin="3.5s" repeatCount="indefinite"/>
  </circle>
  <text x="670" y="1418" font-family="Arial, sans-serif" font-size="20" fill="#ffffff" text-anchor="middle">💼</text>
  <text x="720" y="1405" font-family="Arial, sans-serif" font-size="18" font-weight="bold" fill="#ffffff">
    1K+ Followers on LinkedIn
  </text>
  <text x="720" y="1430" font-family="Arial, sans-serif" font-size="15" fill="#a0a0a0">
    Tech &amp; Innovation Content
  </text>

  <!-- Animated Coding Icon -->
  <g transform="translate(450, 1550)">
    <!-- Laptop Screen -->
    <rect x="0" y="40" width="300" height="180" rx="10" fill="#1a1a2e" stroke="url(#skillGradient)" stroke-width="3"/>
    
    <!-- Code Lines with animation -->
    <line x1="20" y1="80" x2="100" y2="80" stroke="#00ff88" stroke-width="3" opacity="0">
      <animate attributeName="opacity" values="0;1;1" dur="0.5s" begin="0s" fill="freeze"/>
    </line>
    <line x1="40" y1="105" x2="140" y2="105" stroke="#00d4ff" stroke-width="3" opacity="0">
      <animate attributeName="opacity" values="0;1;1" dur="0.5s" begin="0.5s" fill="freeze"/>
    </line>
    <line x1="40" y1="130" x2="180" y2="130" stroke="#f093fb" stroke-width="3" opacity="0">
      <animate attributeName="opacity" values="0;1;1" dur="0.5s" begin="1s" fill="freeze"/>
    </line>
    <line x1="20" y1="155" x2="120" y2="155" stroke="#00ff88" stroke-width="3" opacity="0">
      <animate attributeName="opacity" values="0;1;1" dur="0.5s" begin="1.5s" fill="freeze"/>
    </line>
    <line x1="40" y1="180" x2="160" y2="180" stroke="#00d4ff" stroke-width="3" opacity="0">
      <animate attributeName="opacity" values="0;1;1" dur="0.5s" begin="2s" fill="freeze"/>
    </line>
    
    <!-- Laptop Base -->
    <path d="M -30 220 L 330 220 L 310 250 L -10 250 Z" fill="#2a2a3e" stroke="url(#skillGradient)" stroke-width="2"/>
    
    <!-- Cursor Blinking -->
    <rect x="190" y="175" width="3" height="15" fill="#00ff88">
      <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Footer Wave -->
  <path d="M 0 2720 Q 300 2660 600 2720 T 1200 2720 L 1200 2800 L 0 2800 Z" fill="url(#headerGradient)" opacity="0.5">
    <animate attributeName="d" 
      values="M 0 2720 Q 300 2660 600 2720 T 1200 2720 L 1200 2800 L 0 2800 Z;
              M 0 2720 Q 300 2780 600 2720 T 1200 2720 L 1200 2800 L 0 2800 Z;
              M 0 2720 Q 300 2660 600 2720 T 1200 2720 L 1200 2800 L 0 2800 Z"
      dur="6s" repeatCount="indefinite"/>
  </path>

  <!-- Contact Section -->
  <text x="600" y="2670" font-family="Arial, sans-serif" font-size="24" font-weight="bold" fill="#ffffff" text-anchor="middle">
    Let's Connect! 🚀
  </text>
  <text x="600" y="2710" font-family="Arial, sans-serif" font-size="16" fill="#a0a0a0" text-anchor="middle">
    Open to opportunities in Embedded Systems, AUTOSAR &amp; Software Development
  </text>
</svg>
