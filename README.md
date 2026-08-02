<svg width="1200" height="300" viewBox="0 0 1200 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="bg" cx="50%" cy="50%" r="75%">
      <stop offset="0%" stop-color="#1a0022"/>
      <stop offset="55%" stop-color="#0a0008"/>
      <stop offset="100%" stop-color="#000000"/>
    </radialGradient>
    <linearGradient id="webLine" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#6A0DAD" stop-opacity="0.9"/>
      <stop offset="100%" stop-color="#FF3131" stop-opacity="0.35"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="softGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="2"/>
    </filter>
  </defs>

  <rect width="1200" height="300" fill="url(#bg)"/>

  <!-- Corner web: top-left -->
  <g stroke="url(#webLine)" stroke-width="1" fill="none" opacity="0.55">
    <line x1="0" y1="0" x2="260" y2="0"/>
    <line x1="0" y1="0" x2="0" y2="220"/>
    <line x1="0" y1="0" x2="180" y2="180"/>
    <line x1="0" y1="0" x2="260" y2="90"/>
    <line x1="0" y1="0" x2="90" y2="220"/>
    <path d="M 40 0 Q 40 40 0 40" />
    <path d="M 90 0 Q 90 90 0 90" />
    <path d="M 150 0 Q 150 150 0 150" />
    <path d="M 220 0 Q 220 220 0 220" />
  </g>

  <!-- Corner web: top-right -->
  <g stroke="url(#webLine)" stroke-width="1" fill="none" opacity="0.55">
    <line x1="1200" y1="0" x2="940" y2="0"/>
    <line x1="1200" y1="0" x2="1200" y2="220"/>
    <line x1="1200" y1="0" x2="1020" y2="180"/>
    <line x1="1200" y1="0" x2="940" y2="90"/>
    <line x1="1200" y1="0" x2="1110" y2="220"/>
    <path d="M 1160 0 Q 1160 40 1200 40" />
    <path d="M 1110 0 Q 1110 90 1200 90" />
    <path d="M 1050 0 Q 1050 150 1200 150" />
    <path d="M 980 0 Q 980 220 1200 220" />
  </g>

  <!-- Corner web: bottom-left -->
  <g stroke="url(#webLine)" stroke-width="1" fill="none" opacity="0.4">
    <line x1="0" y1="300" x2="220" y2="300"/>
    <line x1="0" y1="300" x2="0" y2="120"/>
    <line x1="0" y1="300" x2="150" y2="160"/>
    <path d="M 30 300 Q 30 270 0 270" />
    <path d="M 90 300 Q 90 220 0 220" />
    <path d="M 160 300 Q 160 170 0 170" />
  </g>

  <!-- Corner web: bottom-right -->
  <g stroke="url(#webLine)" stroke-width="1" fill="none" opacity="0.4">
    <line x1="1200" y1="300" x2="980" y2="300"/>
    <line x1="1200" y1="300" x2="1200" y2="120"/>
    <line x1="1200" y1="300" x2="1050" y2="160"/>
    <path d="M 1170 300 Q 1170 270 1200 270" />
    <path d="M 1110 300 Q 1110 220 1200 220" />
    <path d="M 1040 300 Q 1040 170 1200 170" />
  </g>

  <!-- Hanging thread + spider (top right, animated bob) -->
  <g>
    <line x1="1000" y1="0" x2="1000" y2="58" stroke="#B48EAD" stroke-width="1" opacity="0.8"/>
    <g id="spider" transform="translate(1000,68)">
      <animateTransform attributeName="transform" type="translate"
        values="1000,68; 1000,78; 1000,68" dur="3.2s" repeatCount="indefinite" additive="sum"/>
      <!-- legs -->
      <g stroke="#FF3131" stroke-width="2" fill="none" opacity="0.9">
        <path d="M -14 -4 Q -22 -10 -30 -14"/>
        <path d="M -14 2 Q -24 4 -32 6"/>
        <path d="M -14 8 Q -22 14 -28 22"/>
        <path d="M -12 12 Q -18 20 -22 28"/>
        <path d="M 14 -4 Q 22 -10 30 -14"/>
        <path d="M 14 2 Q 24 4 32 6"/>
        <path d="M 14 8 Q 22 14 28 22"/>
        <path d="M 12 12 Q 18 20 22 28"/>
      </g>
      <!-- body -->
      <ellipse cx="0" cy="10" rx="9" ry="11" fill="#0D0D0D" stroke="#FF3131" stroke-width="1.5"/>
      <circle cx="0" cy="-5" r="6" fill="#0D0D0D" stroke="#FF3131" stroke-width="1.5"/>
      <circle cx="-2.5" cy="-6" r="1.2" fill="#FF3131"/>
      <circle cx="2.5" cy="-6" r="1.2" fill="#FF3131"/>
    </g>
  </g>

  <!-- Title -->
  <text x="600" y="150" text-anchor="middle" font-family="Poppins, Verdana, sans-serif"
        font-size="54" font-weight="700" fill="#FF3131" filter="url(#glow)">
    YASH SUNSARIYA
    <animate attributeName="opacity" values="0.75;1;0.75" dur="2.5s" repeatCount="indefinite"/>
  </text>

  <!-- Subtitle -->
  <text x="600" y="195" text-anchor="middle" font-family="Poppins, Verdana, sans-serif"
        font-size="20" fill="#B48EAD" filter="url(#softGlow)">
    🕷️ Spinning Code Into Digital Webs 🕸️
  </text>

  <!-- small web accents near title -->
  <g stroke="#6A0DAD" stroke-width="1" fill="none" opacity="0.35">
    <path d="M 300 220 Q 360 200 420 220"/>
    <path d="M 300 220 Q 360 240 420 220"/>
    <path d="M 780 220 Q 840 200 900 220"/>
    <path d="M 780 220 Q 840 240 900 220"/>
  </g>
</svg>
