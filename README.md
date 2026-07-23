<svg width="1180" height="610" viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg">
<defs>
  <clipPath id="canvasClip"><rect x="0" y="0" width="1180" height="610" rx="28"/></clipPath>
  <clipPath id="leftClip"><rect x="32" y="32" width="440" height="546" rx="20"/></clipPath>

  <radialGradient id="blob1" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#10B981" stop-opacity="0.35"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="blob2" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#14B8A6" stop-opacity="0.28"/>
    <stop offset="100%" stop-color="#14B8A6" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="blob3" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#34D399" stop-opacity="0.22"/>
    <stop offset="100%" stop-color="#34D399" stop-opacity="0"/>
  </radialGradient>

  <linearGradient id="asciiGrad" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#064E3B"/>
    <stop offset="45%" stop-color="#00FF7A"/>
    <stop offset="100%" stop-color="#6EE7B7"/>
    <animate attributeName="x1" values="0%;100%;0%" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="x2" values="100%;0%;100%" dur="6s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#00FF7A"/>
    <stop offset="100%" stop-color="#6EE7B7"/>
  </linearGradient>

  <linearGradient id="borderShimmer" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#FFFFFF" stop-opacity="0"/>
    <stop offset="50%" stop-color="#00FF7A" stop-opacity="0.55"/>
    <stop offset="100%" stop-color="#FFFFFF" stop-opacity="0"/>
    <animateTransform attributeName="gradientTransform" type="translate" values="-1180 0;1180 0;-1180 0" dur="7s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="scanGrad" x1="0%" y1="0%" x2="0%" y2="100%">
    <stop offset="0%" stop-color="#00FF7A" stop-opacity="0"/>
    <stop offset="50%" stop-color="#00FF7A" stop-opacity="0.18"/>
    <stop offset="100%" stop-color="#00FF7A" stop-opacity="0"/>
  </linearGradient>

  <filter id="glowSoft" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="3" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
  <filter id="glowStrong" x="-100%" y="-100%" width="300%" height="300%">
    <feGaussianBlur stdDeviation="14"/>
  </filter>
  <filter id="noiseFilter" x="0" y="0" width="100%" height="100%">
    <feTurbulence type="fractalNoise" baseFrequency="0.85" numOctaves="2" stitchTiles="stitch" result="n"/>
    <feColorMatrix in="n" type="matrix" values="0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 0.025 0"/>
  </filter>
</defs>

<g clip-path="url(#canvasClip)">
  <rect x="0" y="0" width="1180" height="610" fill="#030712"/>
  <rect x="0" y="0" width="1180" height="610" filter="url(#noiseFilter)"/>

  <circle cx="150" cy="90" r="220" fill="url(#blob1)">
    <animateTransform attributeName="transform" type="translate" values="0 0;30 20;0 0" dur="10s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1020" cy="150" r="260" fill="url(#blob2)">
    <animateTransform attributeName="transform" type="translate" values="0 0;-25 25;0 0" dur="12s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="560" r="240" fill="url(#blob3)">
    <animateTransform attributeName="transform" type="translate" values="0 0;20 -20;0 0" dur="9s" repeatCount="indefinite"/>
  </circle>

  <!-- floating particles -->
  <g fill="#6EE7B7">
    <circle cx="120" cy="500" r="1.6" opacity="0.6"><animateMotion path="M0,0 C10,-30 -10,-60 0,-90" dur="8s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;0.7;0" dur="8s" repeatCount="indefinite"/></circle>
    <circle cx="980" cy="480" r="1.8" opacity="0.5"><animateMotion path="M0,0 C-15,-25 15,-55 0,-80" dur="9.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;0.6;0" dur="9.5s" repeatCount="indefinite"/></circle>
    <circle cx="600" cy="60" r="1.4" opacity="0.5"><animateMotion path="M0,0 C12,20 -8,45 5,70" dur="7s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;0.6;0" dur="7s" repeatCount="indefinite"/></circle>
    <circle cx="1080" cy="300" r="1.5" opacity="0.5"><animateMotion path="M0,0 C-10,15 10,35 -5,55" dur="10s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;0.55;0" dur="10s" repeatCount="indefinite"/></circle>
    <circle cx="60" cy="250" r="1.5" opacity="0.5"><animateMotion path="M0,0 C8,-18 -12,-32 4,-50" dur="8.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0;0.6;0" dur="8.5s" repeatCount="indefinite"/></circle>
  </g>

  <!-- ================= LEFT: ASCII PORTRAIT PANEL ================= -->
  <g>
    <rect x="32" y="32" width="440" height="546" rx="20" fill="#0F172A" fill-opacity="0.55"/>
    <rect x="32" y="32" width="440" height="546" rx="20" fill="none" stroke="#FFFFFF" stroke-opacity="0.08"/>
    <rect x="32" y="32" width="440" height="546" rx="20" fill="none" stroke="url(#borderShimmer)" stroke-width="1.4"/>

    <g clip-path="url(#leftClip)">
      <!-- scanline sweep -->
      <rect x="32" y="0" width="440" height="60" fill="url(#scanGrad)">
        <animate attributeName="y" values="32;548;32" dur="6s" repeatCount="indefinite"/>
      </rect>

      <text x="64" y="66" font-family="Fira Code, Consolas, monospace" font-size="12" fill="#94A3B8">$ cat identity.ascii</text>

      <g filter="url(#glowSoft)">
        <g font-family="Fira Code, Consolas, monospace" font-size="14" fill="url(#asciiGrad)">
          <animateTransform attributeName="transform" type="translate" values="0 0;0 -6;0 0" dur="5s" repeatCount="indefinite" additive="sum"/>
          <text x="70" y="104"  opacity="0"><animate attributeName="opacity" begin="0.0s"  dur="0.4s" fill="freeze" values="0;1"/>     ┌───────────────────────┐</text>
          <text x="70" y="128" opacity="0"><animate attributeName="opacity" begin="0.15s" dur="0.4s" fill="freeze" values="0;1"/>     │  ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  │</text>
          <text x="70" y="152" opacity="0"><animate attributeName="opacity" begin="0.30s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓▓░░░░░░░░░░░░░░░░▓▓ │</text>
          <text x="70" y="176" opacity="0"><animate attributeName="opacity" begin="0.45s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓░░  ▓▓▓▓▓▓▓▓▓▓  ░░▓ │</text>
          <text x="70" y="200" opacity="0"><animate attributeName="opacity" begin="0.60s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓░░  ▓▓  0x9  ▓▓ ░░▓ │</text>
          <text x="70" y="224" opacity="0"><animate attributeName="opacity" begin="0.75s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓░░  ▓  MAGE  ▓  ░░▓ │</text>
          <text x="70" y="248" opacity="0"><animate attributeName="opacity" begin="0.90s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓░░  ▓▓▓▓▓▓▓▓▓▓  ░░▓ │</text>
          <text x="70" y="272" opacity="0"><animate attributeName="opacity" begin="1.05s" dur="0.4s" fill="freeze" values="0;1"/>     │ ▓▓░░░░░░░░░░░░░░░░▓▓ │</text>
          <text x="70" y="296" opacity="0"><animate attributeName="opacity" begin="1.20s" dur="0.4s" fill="freeze" values="0;1"/>     │  ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  │</text>
          <text x="70" y="320" opacity="0"><animate attributeName="opacity" begin="1.35s" dur="0.4s" fill="freeze" values="0;1"/>     └───────────────────────┘</text>
          <text x="70" y="356" opacity="0" font-size="18" font-weight="700"><animate attributeName="opacity" begin="1.55s" dur="0.4s" fill="freeze" values="0;1"/>     K A R A N   R J</text>
          <text x="70" y="380" opacity="0" font-size="12"><animate attributeName="opacity" begin="1.70s" dur="0.4s" fill="freeze" values="0;1"/>     zoro_rj // purple teamer</text>
        </g>
      </g>

      <text x="70" y="530" font-family="Fira Code, Consolas, monospace" font-size="13" fill="#6EE7B7" opacity="0"><animate attributeName="opacity" begin="1.9s" dur="0.4s" fill="freeze" values="0;1"/>root@wano-arc:~$<tspan fill="#00FF7A"> _</tspan></text>
      <rect x="204" y="518" width="9" height="16" fill="#00FF7A" opacity="0">
        <animate attributeName="opacity" begin="1.9s" values="0;1;1;0;0" keyTimes="0;0.001;0.5;0.51;1" dur="1s" repeatCount="indefinite"/>
      </rect>
    </g>
  </g>

  <!-- ================= RIGHT: TERMINAL PANEL ================= -->
  <g>
    <rect x="492" y="32" width="656" height="546" rx="20" fill="#0F172A" fill-opacity="0.55"/>
    <rect x="492" y="32" width="656" height="546" rx="20" fill="none" stroke="#FFFFFF" stroke-opacity="0.08"/>
    <rect x="492" y="32" width="656" height="546" rx="20" fill="none" stroke="url(#borderShimmer)" stroke-width="1.4"/>

    <!-- title bar -->
    <line x1="492" y1="72" x2="1148" y2="72" stroke="#FFFFFF" stroke-opacity="0.06"/>
    <circle cx="516" cy="52" r="6" fill="#FF5F56"/>
    <circle cx="536" cy="52" r="6" fill="#FFBD2E"/>
    <circle cx="556" cy="52" r="6" fill="#27C93F"/>
    <text x="580" y="57" font-family="Fira Code, Consolas, monospace" font-size="13" fill="#94A3B8">karan@wano — zsh</text>

    <!-- greeting: typing reveal via clip -->
    <clipPath id="greetClip"><rect x="524" y="90" width="0" height="46"><animate attributeName="width" begin="0.2s" dur="1s" fill="freeze" values="0;420"/></rect></clipPath>
    <text x="524" y="122" clip-path="url(#greetClip)" font-family="-apple-system, Segoe UI, Inter, sans-serif" font-size="30" font-weight="700" fill="#F8FAFC">Hi 👋 I'm Karan RJ</text>

    <!-- rotating role carousel -->
    <g font-family="Fira Code, Consolas, monospace" font-size="18" fill="url(#accentGrad)">
      <g opacity="0"><animate attributeName="opacity" dur="15s" repeatCount="indefinite" keyTimes="0;0;0.02;0.18;0.2;1" values="0;0;1;1;0;0"/><text x="524" y="160">&gt; Security Researcher</text></g>
      <g opacity="0"><animate attributeName="opacity" dur="15s" repeatCount="indefinite" keyTimes="0;0.2;0.22;0.38;0.4;1" values="0;0;1;1;0;0"/><text x="524" y="160">&gt; DevSecOps Engineer</text></g>
      <g opacity="0"><animate attributeName="opacity" dur="15s" repeatCount="indefinite" keyTimes="0;0.4;0.42;0.58;0.6;1" values="0;0;1;1;0;0"/><text x="524" y="160">&gt; Full-Stack Developer</text></g>
      <g opacity="0"><animate attributeName="opacity" dur="15s" repeatCount="indefinite" keyTimes="0;0.6;0.62;0.78;0.8;1" values="0;0;1;1;0;0"/><text x="524" y="160">&gt; Purple Teamer</text></g>
      <g opacity="0"><animate attributeName="opacity" dur="15s" repeatCount="indefinite" keyTimes="0;0.8;0.82;0.98;1;1" values="0;0;1;1;0;0"/><text x="524" y="160">&gt; CTF Player</text></g>
    </g>
    <rect x="760" y="146" width="9" height="18" fill="#00FF7A">
      <animate attributeName="opacity" values="1;1;0;0;1" keyTimes="0;0.4;0.41;0.9;1" dur="1s" repeatCount="indefinite"/>
    </rect>

    <line x1="524" y1="184" x2="1116" y2="184" stroke="#FFFFFF" stroke-opacity="0.08"/>

    <!-- sequential info reveal -->
    <g font-family="-apple-system, Segoe UI, Inter, sans-serif" font-size="14">
      <g opacity="0"><animate attributeName="opacity" begin="0.4s" dur="0.5s" fill="freeze" values="0;1"/>
        <animateTransform attributeName="transform" begin="0.4s" dur="0.5s" fill="freeze" type="translate" values="-14 0;0 0"/>
        <text x="524" y="216" fill="#6EE7B7">📍</text>
        <text x="550" y="216" fill="#94A3B8">Location</text>
        <text x="660" y="216" fill="#F8FAFC">Coimbatore, India — Wano Arc</text>
      </g>
      <g opacity="0"><animate attributeName="opacity" begin="0.65s" dur="0.5s" fill="freeze" values="0;1"/>
        <animateTransform attributeName="transform" begin="0.65s" dur="0.5s" fill="freeze" type="translate" values="-14 0;0 0"/>
        <text x="524" y="248" fill="#6EE7B7">🎓</text>
        <text x="550" y="248" fill="#94A3B8">Education</text>
        <text x="660" y="248" fill="#F8FAFC">B.Tech CSE (Cybersecurity), Sri Shakthi IET</text>
      </g>
      <g opacity="0"><animate attributeName="opacity" begin="0.9s" dur="0.5s" fill="freeze" values="0;1"/>
        <animateTransform attributeName="transform" begin="0.9s" dur="0.5s" fill="freeze" type="translate" values="-14 0;0 0"/>
        <text x="524" y="280" fill="#6EE7B7">🛠️</text>
        <text x="550" y="280" fill="#94A3B8">Focus</text>
        <text x="660" y="280" fill="#F8FAFC">Secure full-stack systems + purple-team tooling</text>
      </g>
      <g opacity="0"><animate attributeName="opacity" begin="1.15s" dur="0.5s" fill="freeze" values="0;1"/>
        <animateTransform attributeName="transform" begin="1.15s" dur="0.5s" fill="freeze" type="translate" values="-14 0;0 0"/>
        <text x="524" y="312" fill="#6EE7B7">🌐</text>
        <text x="550" y="312" fill="#94A3B8">Portfolio</text>
        <text x="660" y="312" fill="#F8FAFC">rj-karan.github.io/zoroStack</text>
      </g>
      <g opacity="0"><animate attributeName="opacity" begin="1.4s" dur="0.5s" fill="freeze" values="0;1"/>
        <animateTransform attributeName="transform" begin="1.4s" dur="0.5s" fill="freeze" type="translate" values="-14 0;0 0"/>
        <text x="524" y="344" fill="#6EE7B7">✉️</text>
        <text x="550" y="344" fill="#94A3B8">Email</text>
        <text x="660" y="344" fill="#F8FAFC">rjkaran418@gmail.com</text>
      </g>
    </g>

    <!-- skills -->
    <text x="524" y="398" font-family="-apple-system, Segoe UI, Inter, sans-serif" font-size="14" font-weight="700" fill="#F8FAFC">Skills</text>

    <g font-family="Fira Code, Consolas, monospace" font-size="12.5">
      <!-- row 1 -->
      <g>
        <rect x="524" y="410" width="78"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="524" y="410" width="78"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="0s" repeatCount="indefinite"/></rect>
        <text x="563" y="430" fill="#F8FAFC" text-anchor="middle">Python</text>

        <rect x="612" y="410" width="90"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="612" y="410" width="90"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="0.3s" repeatCount="indefinite"/></rect>
        <text x="657" y="430" fill="#F8FAFC" text-anchor="middle">FastAPI</text>

        <rect x="712" y="410" width="72"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="712" y="410" width="72"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="0.6s" repeatCount="indefinite"/></rect>
        <text x="748" y="430" fill="#F8FAFC" text-anchor="middle">React</text>

        <rect x="794" y="410" width="118" height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="794" y="410" width="118" height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="0.9s" repeatCount="indefinite"/></rect>
        <text x="853" y="430" fill="#F8FAFC" text-anchor="middle">TypeScript</text>

        <rect x="922" y="410" width="72"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="922" y="410" width="72"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="1.2s" repeatCount="indefinite"/></rect>
        <text x="958" y="430" fill="#F8FAFC" text-anchor="middle">MySQL</text>
      </g>
      <!-- row 2 -->
      <g>
        <rect x="524" y="452" width="78"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="524" y="452" width="78"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="1.5s" repeatCount="indefinite"/></rect>
        <text x="563" y="472" fill="#F8FAFC" text-anchor="middle">Docker</text>

        <rect x="612" y="452" width="118" height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="612" y="452" width="118" height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="1.8s" repeatCount="indefinite"/></rect>
        <text x="671" y="472" fill="#F8FAFC" text-anchor="middle">Kali Linux</text>

        <rect x="740" y="452" width="118" height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="740" y="452" width="118" height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="2.1s" repeatCount="indefinite"/></rect>
        <text x="799" y="472" fill="#F8FAFC" text-anchor="middle">Burp Suite</text>

        <rect x="868" y="452" width="60"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="868" y="452" width="60"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="2.4s" repeatCount="indefinite"/></rect>
        <text x="898" y="472" fill="#F8FAFC" text-anchor="middle">AWS</text>

        <rect x="938" y="452" width="60"  height="30" rx="15" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.45"/>
        <rect x="938" y="452" width="60"  height="30" rx="15" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.5"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3s" begin="2.7s" repeatCount="indefinite"/></rect>
        <text x="968" y="472" fill="#F8FAFC" text-anchor="middle">Git</text>
      </g>
    </g>

    <!-- social icons -->
    <g font-family="-apple-system, Segoe UI, Inter, sans-serif">
      <g>
        <circle cx="670" cy="536" r="18" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.5"/>
        <circle cx="670" cy="536" r="18" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.4"><animate attributeName="opacity" values="0.2;0.55;0.2" dur="3.4s" repeatCount="indefinite"/></circle>
        <text x="670" y="541" text-anchor="middle" font-size="13" fill="#F8FAFC" font-weight="600">GH</text>
        <text x="670" y="568" text-anchor="middle" font-size="10" fill="#94A3B8">GitHub</text>
      </g>
      <g>
        <circle cx="770" cy="536" r="18" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.5"/>
        <circle cx="770" cy="536" r="18" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.4"><animate attributeName="opacity" values="0.2;0.55;0.2" dur="3.4s" begin="0.4s" repeatCount="indefinite"/></circle>
        <text x="770" y="541" text-anchor="middle" font-size="13" fill="#F8FAFC" font-weight="600">in</text>
        <text x="770" y="568" text-anchor="middle" font-size="10" fill="#94A3B8">LinkedIn</text>
      </g>
      <g>
        <circle cx="870" cy="536" r="18" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.5"/>
        <circle cx="870" cy="536" r="18" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.4"><animate attributeName="opacity" values="0.2;0.55;0.2" dur="3.4s" begin="0.8s" repeatCount="indefinite"/></circle>
        <text x="870" y="541" text-anchor="middle" font-size="13" fill="#F8FAFC" font-weight="600">X</text>
        <text x="870" y="568" text-anchor="middle" font-size="10" fill="#94A3B8">Twitter</text>
      </g>
      <g>
        <circle cx="970" cy="536" r="18" fill="#0F172A" fill-opacity="0.7" stroke="#00FF7A" stroke-opacity="0.5"/>
        <circle cx="970" cy="536" r="18" fill="none" stroke="#00FF7A" filter="url(#glowSoft)" opacity="0.4"><animate attributeName="opacity" values="0.2;0.55;0.2" dur="3.4s" begin="1.2s" repeatCount="indefinite"/></circle>
        <text x="970" y="541" text-anchor="middle" font-size="12" fill="#F8FAFC" font-weight="600">🌐</text>
        <text x="970" y="568" text-anchor="middle" font-size="10" fill="#94A3B8">Portfolio</text>
      </g>
    </g>
  </g>

  <!-- outer frame highlight -->
  <rect x="1" y="1" width="1178" height="608" rx="27" fill="none" stroke="#00FF7A" stroke-opacity="0.10"/>
</g>
</svg>
