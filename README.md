<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1180 610" width="100%" height="100%">
  <defs>
    <linearGradient id="bg-grad-light" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#FFFFFF" />
      <stop offset="100%" stop-color="#F1F5F9" />
    </linearGradient>
    
    <linearGradient id="accent-grad-light" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#2563EB" />
      <stop offset="50%" stop-color="#06B6D4" />
      <stop offset="100%" stop-color="#10B981" />
      <animateTransform attributeName="gradientTransform" type="rotate" from="0 590 305" to="360 590 305" dur="15s" repeatCount="indefinite" />
    </linearGradient>

    <linearGradient id="ascii-grad-light" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#2563EB" />
      <stop offset="100%" stop-color="#06B6D4" />
      <animate attributeName="y1" values="0%;25%;0%" dur="8s" repeatCount="indefinite" />
    </linearGradient>

    <linearGradient id="panel-border-light" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(15,23,42,0.08)" />
      <stop offset="50%" stop-color="rgba(6,182,212,0.2)" />
      <stop offset="100%" stop-color="rgba(15,23,42,0.03)" />
      <animateTransform attributeName="gradientTransform" type="translate" values="-1000 0; 1000 0" dur="6s" repeatCount="indefinite" />
    </linearGradient>

    <filter id="glow-light" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>

    <filter id="subtle-glow-light" x="-10%" y="-10%" width="120%" height="120%">
      <feGaussianBlur stdDeviation="2" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>

    <filter id="noise-light" x="0%" y="0%" width="100%" height="100%">
      <feTurbulence type="fractalNoise" baseFrequency="0.9" numOctaves="2" stitchTiles="stitch" result="noise" />
      <feColorMatrix type="matrix" values="0 0 0 0 0  0 0 0 0 0  0 0 0 0 0  0 0 0 0.02 0" />
      <feComposite operator="in" in2="SourceGraphic" />
    </filter>

    <style>
      @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&amp;family=Plus+Jakarta+Sans:wght@400;600;800&amp;display=swap');
      .sans { font-family: 'Plus Jakarta Sans', -apple-system, sans-serif; }
      .mono { font-family: 'JetBrains Mono', monospace; }
      .text-main-light { fill: #0F172A; }
      .text-muted-light { fill: #475569; }
      
      /* Micro-interactions & Core Animations */
      .pill-light { transition: all 0.3s ease; cursor: pointer; }
      .pill-light:hover { filter: url(#subtle-glow-light); }
    </style>
  </defs>

  <rect width="1180" height="610" rx="24" fill="url(#bg-grad-light)" />
  
  <circle cx="200" cy="150" r="250" fill="#60A5FA" opacity="0.08" filter="url(#glow-light)">
    <animate attributeName="cy" values="150;180;150" dur="10s" repeatCount="indefinite" />
  </circle>
  <circle cx="950" cy="450" r="300" fill="#34D399" opacity="0.06" filter="url(#glow-light)">
    <animate attributeName="cx" values="950;910;950" dur="12s" repeatCount="indefinite" />
  </circle>

  <g opacity="0.4">
    <circle cx="150" cy="450" r="2" fill="#2563EB"><animate attributeName="cy" values="450;420;450" dur="5s" repeatCount="indefinite" /><animate attributeName="opacity" values="0.2;0.8;0.2" dur="5s" repeatCount="indefinite" /></circle>
    <circle cx="550" cy="120" r="1.5" fill="#06B6D4"><animate attributeName="cy" values="120;90;120" dur="7s" repeatCount="indefinite" /><animate attributeName="opacity" values="0.1;0.7;0.1" dur="7s" repeatCount="indefinite" /></circle>
  </g>

  <rect width="1180" height="610" rx="24" filter="url(#noise-light)" pointer-events="none" />

  <g transform="translate(60, 50)">
    <animateTransform attributeName="transform" type="translate" values="60,47; 60,53; 60,47" dur="6s" repeatCount="indefinite" type="translate" />
    
    <circle cx="190" cy="240" r="160" fill="none" stroke="url(#accent-grad-light)" stroke-width="1.5" opacity="0.1" stroke-dasharray="10 15" />
    
    <g fill="url(#ascii-grad-light)" class="mono" font-size="11" font-weight="bold" letter-spacing="4">
      <text x="40" y="100" opacity="0"><animate attributeName="opacity" to="1" begin="0.2s" fill="freeze"/>▖__▟▛┗▝▞▘   ▜▙ __▖</text>
      <text x="40" y="120" opacity="0"><animate attributeName="opacity" to="1" begin="0.4s" fill="freeze"/>◢▛▘       ▝▜◣</text>
      <text x="40" y="140" opacity="0"><animate attributeName="opacity" to="1" begin="0.6s" fill="freeze"/>▞▘  Option   ▝▚</text>
      <text x="40" y="160" opacity="0"><animate attributeName="opacity" to="1" begin="0.8s" fill="freeze"/>▌  ◢▅◣  ◢▅◣  ▐</text>
      <text x="40" y="180" opacity="0"><animate attributeName="opacity" to="1" begin="1.0s" fill="freeze"/>▌  ▕▋▏  ▕▋▏  ▐</text>
      <text x="40" y="200" opacity="0"><animate attributeName="opacity" to="1" begin="1.2s" fill="freeze"/>▚   ▔   ▔   ▞</text>
      <text x="40" y="220" opacity="0"><animate attributeName="opacity" to="1" begin="1.4s" fill="freeze"/> Matrx  ▼  Init </text>
      <text x="40" y="240" opacity="0"><animate attributeName="opacity" to="1" begin="1.6s" fill="freeze"/>▝▚  ▗▟▙▖  ▞▘</text>
      <text x="40" y="260" opacity="0"><animate attributeName="opacity" to="1" begin="1.8s" fill="freeze"/>  ▔◥▘  ▝◤▔ </text>
      <text x="40" y="280" opacity="0"><animate attributeName="opacity" to="1" begin="2.0s" fill="freeze"/>    █  █    </text>
      <text x="40" y="300" opacity="0"><animate attributeName="opacity" to="1" begin="2.2s" fill="freeze"/>   ◢▛  ▜◣   </text>
    </g>

    <line x1="30" y1="60" x2="350" y2="60" stroke="#2563EB" stroke-width="1" opacity="0.15">
      <animate attributeName="y1" values="60;360;60" dur="4s" repeatCount="indefinite" />
      <animate attributeName="y2" values="60;360;60" dur="4s" repeatCount="indefinite" />
    </line>

    <rect x="40" y="330" width="12" height="4" fill="#2563EB" opacity="1">
      <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
    </rect>
    <text x="60" y="334" fill="#475569" class="mono" font-size="10" letter-spacing="1">SYS_STATUS: SECURE</text>
  </g>

  <g transform="translate(460, 50)">
    <rect width="660" height="510" rx="16" fill="#F8FAFC" opacity="0.9" filter="drop-shadow(0 20px 25px rgba(15,23,42,0.05))" />
    <rect width="660" height="510" rx="16" fill="none" stroke="url(#panel-border-light)" stroke-width="1.5" />

    <g transform="translate(24, 24)">
      <circle cx="0" cy="0" r="6" fill="#EF4444" opacity="0.8" />
      <circle cx="20" cy="0" r="6" fill="#F59E0B" opacity="0.8" />
      <circle cx="40" cy="0" r="6" fill="#10B981" opacity="0.8" />
      <text x="80" y="5" class="mono" font-size="11" fill="#94A3B8" letter-spacing="1">bash://developer-profile/core</text>
    </g>
    
    <line x1="0" y1="48" x2="660" y2="48" stroke="rgba(15,23,42,0.05)" stroke-width="1" />

    <g transform="translate(32, 90)">
      <text x="0" y="0" class="sans" font-size="22" font-weight="600" fill="#475569">Hi 👋</text>
      <text x="0" y="36" class="sans" font-size="38" font-weight="800" fill="#0F172A">I'm <tspan fill="url(#accent-grad-light)">Alex Obsidian</tspan></text>

      <g transform="translate(0, 75)">
        <text x="0" y="0" class="mono" font-size="18" font-weight="700" fill="#2563EB">
          <tspan>> </tspan>
          <animate attributeName="opacity" values="1;1;0;0;0;0;0;0" dur="12s" repeatCount="indefinite" />
          <tspan fill="#0F172A">Full Stack Engineer</tspan>
        </text>
        <text x="22" y="0" class="mono" font-size="18" font-weight="700" fill="#10B981" opacity="0">
          <animate attributeName="opacity" values="0;0;1;1;0;0;0;0" dur="12s" repeatCount="indefinite" />
          <tspan fill="#0F172A">AI Engineering Enthusiast</tspan>
        </text>
        <text x="22" y="0" class="mono" font-size="18" font-weight="700" fill="#06B6D4" opacity="0">
          <animate attributeName="opacity" values="0;0;0;0;1;1;0;0" dur="12s" repeatCount="indefinite" />
          <tspan fill="#0F172A">Open Source Contributor</tspan>
        </text>

        <rect x="290" y="-16" width="10" height="20" fill="#2563EB">
          <animate attributeName="x" values="230;300;280;230" dur="12s" repeatCount="indefinite" />
          <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite" />
        </rect>
      </g>

      <g transform="translate(0, 120)" class="mono" font-size="13">
        <g opacity="0" transform="translate(0,0)">
          <animate attributeName="opacity" to="1" begin="0.5s" fill="freeze" />
          <text x="0" y="0" class="text-muted-light">📍 Location:</text>
          <text x="140" y="0" class="text-main-light">San Francisco, CA (Remote)</text>
        </g>
        <g opacity="0" transform="translate(0,24)">
          <animate attributeName="opacity" to="1" begin="0.8s" fill="freeze" />
          <text x="0" y="0" class="text-muted-light">🎓 Education:</text>
          <text x="140" y="0" class="text-main-light">B.S. Computer Science</text>
        </g>
        <g opacity="0" transform="translate(0,48)">
          <animate attributeName="opacity" to="1" begin="1.1s" fill="freeze" />
          <text x="0" y="0" class="text-muted-light">🚀 Current Focus:</text>
          <text x="140" y="0" class="text-main-light">Next.js Architecture &amp; LLM Agents</text>
        </g>
        <g opacity="0" transform="translate(0,72)">
          <animate attributeName="opacity" to="1" begin="1.4s" fill="freeze" />
          <text x="0" y="0" class="text-muted-light">🌐 Portfolio:</text>
          <text x="140" y="0" fill="#2563EB" font-weight="bold">obsidian.dev</text>
        </g>
      </g>

      <g transform="translate(0, 245)">
        <text x="0" y="0" class="sans" font-size="14" font-weight="600" fill="#475569" letter-spacing="1">TECHNICAL STACK</text>
        
        <g transform="translate(0, 16)">
          <g transform="translate(0,0)" class="pill-light">
            <rect width="70" height="28" rx="14" fill="#E2E8F0" stroke="rgba(37,99,235,0.2)" stroke-width="1"/>
            <text x="35" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#2563EB">React</text>
          </g>
          <g transform="translate(80,0)" class="pill-light">
            <rect width="80" height="28" rx="14" fill="#E2E8F0" stroke="rgba(15,23,42,0.1)" stroke-width="1"/>
            <text x="40" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#0F172A">Next.js</text>
          </g>
          <g transform="translate(170,0)" class="pill-light">
            <rect width="95" height="28" rx="14" fill="#E2E8F0" stroke="rgba(37,99,235,0.2)" stroke-width="1"/>
            <text x="47.5" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#1E40AF">TypeScript</text>
          </g>
          <g transform="translate(275,0)" class="pill-light">
            <rect width="80" height="28" rx="14" fill="#E2E8F0" stroke="rgba(16,185,129,0.2)" stroke-width="1"/>
            <text x="40" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#065F46">Node.js</text>
          </g>
          <g transform="translate(365,0)" class="pill-light">
            <rect width="80" height="28" rx="14" fill="#E2E8F0" stroke="rgba(234,179,8,0.3)" stroke-width="1"/>
            <text x="40" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#854D0E">Python</text>
          </g>
        </g>

        <g transform="translate(0, 56)">
          <g transform="translate(0,0)" class="pill-light">
            <rect width="80" height="28" rx="14" fill="#E2E8F0" stroke="rgba(37,99,235,0.2)" stroke-width="1"/>
            <text x="40" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#2563EB">Docker</text>
          </g>
          <g transform="translate(90,0)" class="pill-light">
            <rect width="65" height="28" rx="14" fill="#E2E8F0" stroke="rgba(249,115,22,0.3)" stroke-width="1"/>
            <text x="32.5" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#C2410C">AWS</text>
          </g>
          <g transform="translate(165,0)" class="pill-light">
            <rect width="90" height="28" rx="14" fill="#E2E8F0" stroke="rgba(37,99,235,0.2)" stroke-width="1"/>
            <text x="45" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#1E40AF">Postgres</text>
          </g>
          <g transform="translate(265,0)" class="pill-light">
            <rect width="85" height="28" rx="14" fill="#E2E8F0" stroke="rgba(6,182,212,0.3)" stroke-width="1"/>
            <text x="42.5" y="18" text-anchor="middle" class="sans" font-size="11" font-weight="600" fill="#0369A1">Tailwind</text>
          </g>
        </g>
      </g>

      <g transform="translate(0, 365)">
        <line x1="0" y1="0" x2="596" y2="0" stroke="rgba(15,23,42,0.06)" stroke-width="1" />
        
        <g transform="translate(0, 20)">
          <g transform="translate(0,0)" class="pill-light">
            <circle cx="16" cy="16" r="16" fill="#E2E8F0" />
            <path d="M16 5C9.9 5 5 9.9 5 16c0 4.9 3.2 9 7.6 10.5.5.1.7-.2.7-.5v-1.9c-3.1.7-3.7-1.5-3.7-1.5-.5-1.3-1.2-1.7-1.2-1.7-1-.7.1-.7.1-.7 1.1.1 1.7 1.2 1.7 1.2 1.0 1.7 2.6 1.2 3.3.9.1-.7.4-1.2.7-1.5-2.5-.3-5.1-1.2-5.1-5.5 0-1.2.4-2.2 1.2-3-.1-.3-.5-1.4.1-3 0 0 .9-.3 3 1.1.9-.2 1.8-.4 2.8-.4s1.9.2 2.8.4c2.1-1.4 3-1.1 3-1.1.6 1.6.2 2.7.1 3 .7.8 1.2 1.8 1.2 3 0 4.3-2.6 5.2-5.2 5.5.4.3.8 1.1.8 2.2v3.3c0 .3.2.6.7.5C23.8 25 27 20.9 27 16c0-6.1-4.9-11-11-11z" fill="#0F172A" />
          </g>
          
          <g transform="translate(48,0)" class="pill-light">
            <circle cx="16" cy="16" r="16" fill="#E2E8F0" />
            <path d="M10 9H14V23H10V9ZM12 4C13.4 4 14.5 5.1 14.5 6.5C14.5 7.9 13.4 9 12 9C10.6 9 9.5 7.9 9.5 6.5C9.5 5.1 10.6 4 12 4ZM16 9H20V11H20.2C20.8 9.8 22.2 8.7 24.5 8.7C28.8 8.7 30 11.2 30 15.5V23H26V16.5C26 14.2 25.2 12.8 23 12.8C21.2 12.8 20.2 14 19.8 15.2C19.6 15.7 19.5 16.3 19.5 17V23H15.5V9H16Z" fill="#2563EB" transform="translate(3,3) scale(0.8)"/>
          </g>

          <g transform="translate(96,0)" class="pill-light">
            <circle cx="16" cy="16" r="16" fill="#E2E8F0" />
            <path d="M18.2 14.2L25.3 6H23.6L17.4 13.2L12.5 6H6.8L14.2 16.8L6.8 25.4H8.5L15 17.8L20.2 25.4H25.9L18.2 14.2ZM15.8 16.9L15 15.8L8.9 7.2H11.5L16.5 14.2L17.3 15.3L23.6 24.3H21L15.8 16.9Z" fill="#0F172A" transform="translate(3,3) scale(0.8)"/>
          </g>
        </g>
      </g>
    </g>
  </g>
</svg>
