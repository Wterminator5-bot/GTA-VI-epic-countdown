# GTA-VI-epic-countdown
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GTA VI Release Countdown - Live Vice City Edition</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Plus+Jakarta+Sans:wght@300;400;600;800&family=Pinyon+Script&display=swap" rel="stylesheet">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            digital: ['"Orbitron"', 'sans-serif'],
            cursive: ['"Pinyon Script"', 'cursive'],
          },
          colors: {
            gtaPink: '#ff007f',
            gtaBlue: '#00f0ff',
            gtaPurple: '#3b0066',
            gtaOrange: '#ff5e00',
            gtaYellow: '#ffea00',
          }
        }
      }
    }
  </script>
  <style>
    ::-webkit-scrollbar{width:6px}::-webkit-scrollbar-track{background:rgba(15,10,25,.6)}
    ::-webkit-scrollbar-thumb{background:#ff007f;border-radius:3px}
    @keyframes synthGrid{0%{background-position:0 0}100%{background-position:0 100%}}
    @keyframes neonPulse{0%,100%{filter:drop-shadow(0 0 10px rgba(255,0,127,.8)) drop-shadow(0 0 25px rgba(255,0,127,.4))}50%{filter:drop-shadow(0 0 20px rgba(255,0,127,1)) drop-shadow(0 0 40px rgba(255,0,127,.6))}}
    @keyframes blueNeonPulse{0%,100%{filter:drop-shadow(0 0 10px rgba(0,240,255,.7))}50%{filter:drop-shadow(0 0 22px rgba(0,240,255,.95))}}
    @keyframes sunGlow{0%,100%{transform:scale(1);filter:drop-shadow(0 0 30px rgba(255,94,0,.6))}50%{transform:scale(1.03);filter:drop-shadow(0 0 50px rgba(255,0,127,.8))}}
    @keyframes palmSway{0%,100%{transform:rotate(0)}50%{transform:rotate(2deg)}}
    @keyframes scanline{0%{transform:translateY(-100%)}100%{transform:translateY(100%)}}
    @keyframes textShimmer{0%{text-shadow:0 0 4px #fff,0 0 12px #ff007f,0 0 30px #ff007f}50%{text-shadow:0 0 8px #fff,0 0 20px #00f0ff,0 0 40px #00f0ff}100%{text-shadow:0 0 4px #fff,0 0 12px #ff007f,0 0 30px #ff007f}}
    .synth-grid{background-size:50px 50px;background-image:linear-gradient(to right,rgba(255,0,127,.15) 1px,transparent 1px),linear-gradient(to bottom,rgba(255,0,127,.15) 1px,transparent 1px);animation:synthGrid 18s linear infinite}
    .sun-gradient{background:linear-gradient(to bottom,#ffea00 0%,#ff5e00 40%,#ff007f 80%,transparent 100%)}
    .retro-scanlines{background:linear-gradient(rgba(18,10,36,0) 50%,rgba(0,0,0,.3) 50%);background-size:100% 4px}
    .neon-border-pink{box-shadow:0 0 15px rgba(255,0,127,.4),inset 0 0 15px rgba(255,0,127,.2);border:1px solid rgba(255,0,127,.6)}
    .neon-border-blue{box-shadow:0 0 15px rgba(0,240,255,.4),inset 0 0 15px rgba(0,240,255,.2);border:1px solid rgba(0,240,255,.6)}
    .glitch-hover:hover{animation:glitch .3s linear infinite}
    @keyframes glitch{0%{transform:translate(0)}20%{transform:translate(-2px,2px)}40%{transform:translate(-2px,-2px)}60%{transform:translate(2px,2px)}80%{transform:translate(2px,-2px)}100%{transform:translate(0)}}
  </style>
</head>
<body class="bg-[#0b0518] text-white font-sans min-h-screen overflow-x-hidden relative selection:bg-gtaPink selection:text-white">

<div class="fixed inset-0 z-0 overflow-hidden pointer-events-none">
  <div class="absolute inset-0 bg-gradient-to-b from-[#0f0426] via-[#2a0845] to-[#040112]"></div>
  <div class="absolute inset-0 bg-gradient-to-b from-transparent to-[#100329]">
    <div class="absolute left-1/2 bottom-[20%] -translate-x-1/2 w-[90vw] h-[90vw] max-w-[550px] max-h-[550px] rounded-full sun-gradient" style="animation:sunGlow 8s ease-in-out infinite">
      <div class="w-full h-full flex flex-col justify-end pb-4 space-y-2 md:space-y-3">
        <div class="bg-[#0b0518] h-1 opacity-40"></div><div class="bg-[#0b0518] h-2 opacity-50"></div>
        <div class="bg-[#0b0518] h-3 opacity-60"></div><div class="bg-[#0b0518] h-4 opacity-75"></div>
        <div class="bg-[#0b0518] h-6 opacity-90"></div><div class="bg-[#0b0518] h-10 opacity-100"></div>
      </div>
    </div>
  </div>
  <div class="absolute bottom-0 left-0 w-full h-[40vh] origin-top transform [perspective:400px] [rotateX:65deg] overflow-hidden"><div class="absolute inset-0 synth-grid"></div></div>
  <div id="leftPalm" class="absolute bottom-[-20px] left-[-50px] md:left-[-10px] w-[200px] md:w-[350px] opacity-40 md:opacity-75 z-10 select-none pointer-events-none" style="animation:palmSway 10s ease-in-out infinite">
    <svg viewBox="0 0 100 120" fill="currentColor" class="text-gtaPurple filter drop-shadow-[0_0_20px_rgba(59,0,102,.8)]"><path d="M10,120 Q20,60 45,20 Q48,15 45,10 Q40,5 30,15 C25,12 15,22 10,35 C12,40 18,35 22,30 C12,42 2,55 5,75 C10,75 16,65 25,52 C15,68 8,85 22,95 C25,90 26,80 27,70 C24,88 28,105 45,115 C42,100 38,90 35,80 Z"/><path d="M0,120 Q10,70 25,40 Q35,30 20,20 C10,25 5,45 2,65" opacity=".8"/></svg>
  </div>
  <div id="rightPalm" class="absolute bottom-[-20px] right-[-50px] md:right-[-10px] w-[200px] md:w-[350px] opacity-40 md:opacity-75 z-10 select-none pointer-events-none" style="animation:palmSway 12s ease-in-out infinite">
    <svg viewBox="0 0 100 120" fill="currentColor" class="text-[#1a0033] filter drop-shadow-[0_0_25px_rgba(255,0,127,.3)]"><path d="M90,120 Q80,60 55,20 Q52,15 55,10 Q60,5 70,15 C75,12 85,22 90,35 C88,40 82,35 78,30 C88,42 98,55 95,75 C90,75 84,65 75,52 C85,68 92,85 78,95 C75,90 74,80 73,70 C76,88 72,105 55,115 C58,100 62,90 65,80 Z"/></svg>
  </div>
  <canvas id="ambientParticles" class="absolute inset-0 w-full h-full"></canvas>
  <div class="absolute bottom-[2%] left-0 w-full h-1 overflow-hidden opacity-40"><div id="retroCar" class="absolute h-1 w-8 bg-gtaPink shadow-[0_0_10px_#ff007f] transition-all duration-[8000ms] ease-linear"></div></div>
  <div id="crtOverlay" class="absolute inset-0 retro-scanlines pointer-events-none z-50 opacity-40"></div>
  <div id="scanlineBeam" class="absolute inset-x-0 top-0 h-0.5 bg-white opacity-10 z-50" style="animation:scanline 6s linear infinite"></div>
</div>

<header class="relative z-10 max-w-7xl mx-auto px-4 py-4 flex flex-wrap justify-between items-center gap-4">
  <div class="flex items-center space-x-3">
    <div class="w-10 h-10 border-2 border-gtaPink rounded-tr-lg rounded-bl-lg rotate-45 flex items-center justify-center shadow-[0_0_10px_#ff007f]"><span class="-rotate-45 font-digital font-black text-gtaPink text-lg">VI</span></div>
    <div><h1 class="text-xs uppercase tracking-[.3em] text-gtaBlue font-bold">Rockstar Games</h1><p class="text-xs tracking-wider text-gray-400 font-digital">PRE-LAUNCH DESK</p></div>
  </div>

  <div class="flex flex-wrap items-center gap-3">
    <!-- LANGUAGE SELECTOR -->
    <div class="flex items-center gap-2 bg-black/60 backdrop-blur-md rounded-full px-3 py-2 border border-white/10">
      <span class="text-xs">🌐</span>
      <select id="languageSelect" onchange="setLanguage(this.value)" class="bg-transparent text-xs font-bold uppercase tracking-wider text-white outline-none cursor-pointer">
        <option value="en" class="bg-[#120721]">English</option>
        <option value="hu" class="bg-[#120721]">Magyar</option>
        <option value="it" class="bg-[#120721]">Italiano</option>
        <option value="de" class="bg-[#120721]">Deutsch</option>
      </select>
    </div>

    <div class="flex items-center gap-3 bg-black/60 backdrop-blur-md rounded-full px-4 py-2 border border-white/10 shadow-lg">
      <div class="flex items-center gap-2">
        <span class="relative flex h-2.5 w-2.5"><span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-gtaPink opacity-75"></span><span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-gtaPink"></span></span>
        <span data-i18n="radio" class="text-xs font-semibold tracking-wider text-gray-300 mr-2 uppercase">Synthwave Radio:</span>
      </div>
      <button onclick="toggleSynthAudio()" id="audioBtn" class="bg-gtaPink hover:bg-[#e60072] text-white text-xs px-3 py-1 rounded-full font-bold shadow-[0_0_10px_rgba(255,0,127,.5)] transition duration-200 uppercase flex items-center gap-1">🔊 <span data-i18n="playBeat">Play Beat</span></button>
      <div class="h-4 w-[1px] bg-white/20"></div>
      <div class="flex items-end gap-0.5 h-3"><div class="w-1 bg-gtaBlue rounded-full animate-pulse h-2"></div><div class="w-1 bg-gtaPink rounded-full animate-pulse h-3"></div><div class="w-1 bg-gtaYellow rounded-full animate-pulse h-1"></div><div class="w-1 bg-gtaBlue rounded-full animate-pulse h-2.5"></div></div>
    </div>
  </div>
</header>

<main class="relative z-10 max-w-7xl mx-auto px-4 pt-4 pb-20 flex flex-col items-center">
  <div class="text-center mt-6 mb-10 w-full relative">
    <div class="absolute -top-12 left-1/2 -translate-x-1/2 opacity-30 select-none text-gtaPink font-cursive text-7xl md:text-9xl pointer-events-none">Vice City</div>
    <div class="inline-block px-3 py-1 bg-gtaPink/10 border border-gtaPink/30 rounded-md mb-2"><span data-i18n="coordinates" class="text-gtaPink font-bold tracking-[.25em] text-xs uppercase animate-pulse">Leonida State Launch Coordinates Confirmed</span></div>
    <h2 class="text-5xl md:text-8xl font-black tracking-tighter uppercase relative select-none">
      <span class="block text-transparent bg-clip-text bg-gradient-to-r from-white via-gtaBlue to-gtaPink font-extrabold filter drop-shadow-[0_4px_12px_rgba(0,0,0,.8)]" style="animation:textShimmer 6s infinite">GTA VI</span>
      <span data-i18n="countdown" class="block text-xl md:text-3xl font-digital tracking-[.4em] text-gtaBlue font-bold mt-1 uppercase" style="animation:blueNeonPulse 4s infinite">Release Countdown</span>
    </h2>
    <p data-i18n="intro" class="text-gray-400 max-w-xl mx-auto mt-3 text-sm font-medium tracking-wide">Locking coordinates onto the most anticipated cultural event of the decade. Live tracking to November 19, 2026.</p>
  </div>

  <div class="w-full max-w-5xl rounded-3xl overflow-hidden bg-[#120721]/70 backdrop-blur-xl border-t-2 border-l-2 border-white/10 shadow-[0_30px_100px_rgba(0,0,0,.8)] p-6 md:p-10 mb-10 relative">
    <div class="absolute -top-16 -left-16 w-48 h-48 rounded-full bg-gtaPink/15 filter blur-3xl"></div><div class="absolute -bottom-16 -right-16 w-48 h-48 rounded-full bg-gtaBlue/15 filter blur-3xl"></div>
    <div class="flex justify-between items-center border-b border-white/5 pb-4 mb-8">
      <div class="flex items-center space-x-2 text-xs md:text-sm text-gray-400 font-mono"><span class="w-2.5 h-2.5 bg-red-600 rounded-full animate-ping"></span><span><span data-i18n="target">TARGET:</span> <strong>NOV 19, 2026 00:00:00 UTC</strong></span></div>
      <div class="hidden md:flex items-center space-x-4"><span data-i18n="speculation" class="text-xs text-gtaPink uppercase font-bold tracking-widest bg-gtaPink/10 px-2 py-0.5 rounded border border-gtaPink/20">Official Speculation Target</span><span class="text-xs text-gray-400 font-digital" id="gmtDisplay">GMT: Loading...</span></div>
    </div>

    <div class="grid grid-cols-2 md:grid-cols-5 gap-4 md:gap-6">
      <div class="bg-black/40 rounded-2xl p-4 md:p-6 text-center border border-white/5 shadow-inner hover:border-gtaPink/30 transition-all duration-300 group"><div data-i18n="days" class="text-xs font-semibold tracking-widest text-gtaPink uppercase">Days</div><div class="text-4xl md:text-6xl font-black font-digital mt-2 text-white" id="daysBox">000</div><div data-i18n="daysLeft" class="text-[9px] uppercase tracking-widest text-gray-500 mt-2">Days Left</div></div>
      <div class="bg-black/40 rounded-2xl p-4 md:p-6 text-center border border-white/5 shadow-inner hover:border-gtaBlue/30 transition-all duration-300 group"><div data-i18n="hours" class="text-xs font-semibold tracking-widest text-gtaBlue uppercase">Hours</div><div class="text-4xl md:text-6xl font-black font-digital mt-2 text-white" id="hoursBox">00</div><div data-i18n="hourCycles" class="text-[9px] uppercase tracking-widest text-gray-500 mt-2">Hour Cycles</div></div>
      <div class="bg-black/40 rounded-2xl p-4 md:p-6 text-center border border-white/5 shadow-inner hover:border-gtaPink/30 transition-all duration-300 group"><div data-i18n="minutes" class="text-xs font-semibold tracking-widest text-gtaPink uppercase">Minutes</div><div class="text-4xl md:text-6xl font-black font-digital mt-2 text-white" id="minsBox">00</div><div data-i18n="minuteMarks" class="text-[9px] uppercase tracking-widest text-gray-500 mt-2">Minute Marks</div></div>
      <div class="bg-black/40 rounded-2xl p-4 md:p-6 text-center border border-white/5 shadow-inner hover:border-gtaBlue/30 transition-all duration-300 group"><div data-i18n="seconds" class="text-xs font-semibold tracking-widest text-gtaBlue uppercase">Seconds</div><div class="text-4xl md:text-6xl font-black font-digital mt-2 text-white" id="secsBox">00</div><div data-i18n="secondsClock" class="text-[9px] uppercase tracking-widest text-gray-500 mt-2">Seconds Clock</div></div>
      <div class="col-span-2 md:col-span-1 bg-gradient-to-br from-gtaPink/10 to-gtaBlue/10 rounded-2xl p-4 md:p-6 text-center border border-white/10 shadow-lg relative overflow-hidden group"><div data-i18n="msPrecision" class="text-xs font-bold tracking-widest text-gtaYellow uppercase">Ms Precision</div><div class="text-4xl md:text-5xl font-black font-digital mt-3 text-gtaYellow" id="msBox">000</div><div data-i18n="millisecondLoop" class="text-[9px] uppercase tracking-widest text-gray-400 mt-2">Millisecond Loop</div></div>
    </div>

    <div class="mt-8 pt-6 border-t border-white/5">
      <div class="flex justify-between items-center mb-2"><span data-i18n="progress" class="text-xs uppercase font-bold tracking-widest text-gray-400">Time Travel Distance Progression</span><span class="text-xs font-digital text-gtaPink font-bold" id="percentComplete">Calculating...</span></div>
      <div class="w-full bg-black/50 rounded-full h-3 border border-white/10 overflow-hidden relative p-[2px]"><div id="progBar" class="bg-gradient-to-r from-gtaBlue via-gtaPink to-gtaYellow h-full rounded-full shadow-[0_0_8px_#ff007f] transition-all duration-1000" style="width:0%"></div></div>
      <div class="flex justify-between items-center mt-2 text-[10px] text-gray-500 font-mono"><span data-i18n="departed">DEPARTED: ANNOUNCEMENT (DEC 2023)</span><span data-i18n="arrival">ARRIVAL: CODENAME LUCIA & JASON</span></div>
    </div>
  </div>

  <div class="w-full max-w-5xl grid grid-cols-1 lg:grid-cols-3 gap-6">
    <div class="lg:col-span-1 bg-black/60 backdrop-blur-md rounded-2xl p-6 border border-white/5 flex flex-col justify-between">
      <div>
        <h3 data-i18n="atmosphere" class="text-lg font-bold uppercase tracking-wider text-gtaPink flex items-center gap-2 border-b border-white/5 pb-3">⚙ Atmosphere Customizer</h3>
        <p data-i18n="atmosphereDesc" class="text-xs text-gray-400 mt-2 mb-4">Fine-tune the neon lighting of the Leonida Vice Highway live simulation parameters.</p>
        <div class="space-y-4">
          <div class="flex justify-between items-center bg-white/5 rounded-xl p-3 border border-white/5"><div><div data-i18n="crt" class="text-xs font-bold uppercase tracking-wider text-gtaBlue">CRT Arcade Filter</div><div data-i18n="crtDesc" class="text-[10px] text-gray-400">Classic arcade overlay lines</div></div><button onclick="toggleScanlines()" id="scanlinesToggle" class="relative inline-flex h-6 w-11 rounded-full border-2 border-transparent bg-gtaPink"><span id="scanlinesKnob" class="pointer-events-none inline-block h-5 w-5 transform rounded-full bg-white shadow transition duration-200 translate-x-5"></span></button></div>
          <div class="bg-white/5 rounded-xl p-3 border border-white/5"><div class="flex justify-between items-center mb-1"><span data-i18n="palm" class="text-xs font-bold uppercase tracking-wider text-gtaBlue">Palm Tree Sway Wind Speed</span><span class="text-xs text-gtaPink font-digital" id="swaySpeedLabel">Medium</span></div><input type="range" min="1" max="3" value="2" oninput="changeSwaySpeed(this.value)" class="w-full h-1 bg-black rounded-lg appearance-none cursor-pointer accent-gtaPink"></div>
          <div class="bg-white/5 rounded-xl p-3 border border-white/5"><div class="flex justify-between items-center mb-1"><span data-i18n="highway" class="text-xs font-bold uppercase tracking-wider text-gtaBlue">Retro Highway Speed</span><span class="text-xs text-gtaPink font-digital" id="gridSpeedLabel">Fast</span></div><input type="range" min="1" max="3" value="3" oninput="changeGridSpeed(this.value)" class="w-full h-1 bg-black rounded-lg appearance-none cursor-pointer accent-gtaPink"></div>
        </div>
      </div>
      <div data-i18n="fireflies" class="mt-4 pt-4 border-t border-white/5 bg-gtaPink/10 text-gtaPink text-[10px] rounded p-2 text-center border border-gtaPink/20 font-bold uppercase tracking-wider animate-pulse">Double click background to spawn neon fireflies</div>
    </div>

    <div class="lg:col-span-2 bg-black/60 backdrop-blur-md rounded-2xl p-6 border border-white/5 flex flex-col justify-between">
      <div>
        <div class="flex justify-between items-start border-b border-white/5 pb-3">
          <h3 data-i18n="dossier" class="text-lg font-bold uppercase tracking-wider text-gtaBlue flex items-center gap-2">▣ Leonida Dossier Intelligence</h3>
          <div class="flex gap-1.5"><button onclick="selectPlatform('ps5')" id="platform-ps5" class="px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-gtaBlue bg-gtaBlue/20 text-white">PS5</button><button onclick="selectPlatform('xbox')" id="platform-xbox" class="px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-white/20 text-gray-400">XBOX SERIES X|S</button></div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4">
          <div class="space-y-3">
            <div class="border-l-2 border-gtaPink pl-3"><div data-i18n="location" class="text-[10px] uppercase text-gray-400 tracking-wider font-mono">Location</div><div class="text-sm font-bold tracking-wide">Vice City, Port Gellhorn & Leonida State</div></div>
            <div class="border-l-2 border-gtaBlue pl-3"><div data-i18n="protagonists" class="text-[10px] uppercase text-gray-400 tracking-wider font-mono">Main Protagonists</div><div class="text-sm font-bold tracking-wide">Lucia & Jason (Dynamic Duo Crime Partnership)</div></div>
            <div class="border-l-2 border-gtaYellow pl-3"><div data-i18n="innovation" class="text-[10px] uppercase text-gray-400 tracking-wider font-mono">Gameplay Innovation</div><div class="text-sm font-bold tracking-wide">Dynamic social media engine, realistic crowd ecosystems</div></div>
          </div>
          <div class="bg-black/40 rounded-xl p-4 border border-white/5 flex flex-col justify-between">
            <div><span data-i18n="preorderHub" class="text-[10px] uppercase font-bold tracking-widest text-gtaPink">Pre-order Hub Mockup</span><h4 data-i18n="secureSeat" class="text-sm font-bold mt-1 text-white">Secure Your Seat in Vice City</h4><p data-i18n="bonusDesc" class="text-[11px] text-gray-400 mt-1">Get custom vehicle modifications and exclusive safe-house bonuses upon retail verification.</p></div>
            <div class="mt-4 flex gap-2"><button onclick="showBonusModal()" data-i18n="bonusBtn" class="flex-1 bg-gradient-to-r from-gtaPink to-[#bb005e] text-white text-xs py-2 rounded font-bold uppercase tracking-wider">Check Bonus Perks</button><button onclick="toggleSoundEffect()" class="bg-white/5 p-2 rounded text-white border border-white/10">🔊</button></div>
          </div>
        </div>
      </div>

      <div class="mt-6 pt-4 border-t border-white/5">
        <div class="flex justify-between items-center mb-3"><span data-i18n="trailerFeed" class="text-xs uppercase font-bold tracking-widest text-gray-400">Official Trailer Intel Feed</span><span data-i18n="trailerCount" class="text-[10px] text-gtaBlue font-mono">2 Official Trailers / 1 Launch Showcase</span></div>
        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
          <div class="relative rounded-lg overflow-hidden border border-gtaPink/30 group cursor-pointer hover:scale-[1.02] transition-transform" onclick="openTrailerEmbed('QdBZY2fkU-0')"><div class="h-16 bg-gradient-to-r from-purple-950 to-pink-900 flex items-center justify-center relative overflow-hidden"><span data-i18n="trailer1" class="text-[9px] font-digital text-gtaPink tracking-widest z-10 font-bold uppercase bg-black/60 px-1.5 py-0.5 rounded">WATCH TRAILER 1</span><div class="absolute inset-0 synth-grid opacity-30"></div></div><div class="absolute bottom-1 left-2 right-2 z-20 flex justify-between items-center"><span data-i18n="trailer1Name" class="text-[8px] text-gray-300 font-bold tracking-wide truncate">Lucia and Jason Introduction</span><span class="text-[7px] bg-gtaPink px-1 rounded text-white font-bold">250M+ Views</span></div></div>
          <div class="relative rounded-lg overflow-hidden border border-gtaBlue/60 group cursor-pointer hover:scale-[1.02] transition-transform" onclick="openTrailerEmbed('VQRLujxTm3c')"><div class="h-16 bg-gradient-to-r from-[#031c30] to-[#04445c] flex items-center justify-center relative overflow-hidden"><span data-i18n="trailer2" class="text-[9px] font-digital text-gtaBlue tracking-widest z-10 font-bold uppercase bg-black/60 px-1.5 py-0.5 rounded">WATCH TRAILER 2</span><div class="absolute inset-0 synth-grid opacity-20"></div></div><div class="absolute bottom-1 left-2 right-2 z-20 flex justify-between items-center"><span data-i18n="trailer2Name" class="text-[8px] text-gray-300 font-bold tracking-wide truncate">"New Beginnings" Leonida</span><span class="text-[7px] bg-gtaBlue px-1 rounded text-black font-bold">Official Release</span></div></div>

          <!-- LAUNCH SHOWCASE: requested Netflix link -->
          <a href="https://www.netflix.com/us/title/83035795?s=i&trkid=13747225&shareType=Title&shareUuid=D15257EA-132F-4DFB-800F-40A5BAE48E22&trg=cp&unifiedEntityIdEncoded=Video%3A83035795&vlang=en" target="_blank" rel="noopener noreferrer" class="relative rounded-lg overflow-hidden border border-gtaYellow/50 group hover:scale-[1.02] transition-all duration-300 block">
            <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent z-10"></div>
            <div class="h-16 bg-black/80 flex items-center justify-center relative">
              <span data-i18n="launchShowcase" class="text-[9px] font-digital text-gtaYellow tracking-widest z-20 font-bold uppercase bg-black/60 px-1.5 py-0.5 rounded">LAUNCH SHOWCASE ↗</span>
              <div class="absolute inset-0 flex items-center justify-center text-gtaYellow/20 text-xs font-mono">▶ OPEN</div>
            </div>
            <div class="absolute bottom-1 left-2 right-2 z-20"><span data-i18n="launchDesc" class="text-[8px] text-gtaYellow font-bold tracking-wide block truncate">Netflix Launch Showcase • Open link</span></div>
          </a>
        </div>
      </div>
    </div>
  </div>

  <div class="w-full max-w-5xl mt-8 bg-gradient-to-r from-gtaPink/10 via-[#1d0a2d] to-gtaBlue/10 p-4 rounded-xl border border-white/5 flex flex-wrap justify-between items-center gap-4 relative overflow-hidden">
    <div class="absolute top-0 left-0 w-2 h-full bg-gtaPink"></div><div class="flex items-center space-x-3 z-10"><span data-i18n="breaking" class="bg-gtaPink text-white text-[9px] font-black uppercase tracking-widest px-2 py-1 rounded">BREAKING NEWS</span><p class="text-xs text-gray-200 tracking-wide font-medium" id="breakingNewsFeed">"Leonida Coast Guard warns of highly dangerous neon sunsets and synthwave music storms..."</p></div><button onclick="shuffleNews()" data-i18n="nextAlert" class="text-[10px] text-gtaBlue uppercase font-bold tracking-widest border border-gtaBlue/30 px-3 py-1 rounded bg-gtaBlue/5">Next Alert</button>
  </div>
</main>

<div id="bonusModal" class="fixed inset-0 z-[100] flex items-center justify-center bg-black/80 backdrop-blur-md hidden">
  <div class="bg-[#120721] border-2 border-gtaPink rounded-3xl p-6 md:p-8 max-w-md w-full mx-4 shadow-[0_0_50px_rgba(255,0,127,.5)]">
    <div class="text-center"><div class="w-16 h-16 bg-gtaPink/10 border-2 border-gtaPink rounded-full flex items-center justify-center mx-auto mb-4 animate-bounce"><span class="text-gtaPink text-2xl">🎁</span></div>
      <h3 data-i18n="modalTitle" class="text-2xl font-digital font-black text-gtaPink uppercase tracking-widest">VP Pre-Launch Unlock</h3>
      <p data-i18n="modalText" class="text-gray-300 text-xs mt-3 leading-relaxed">Congratulations, Citizen of Leonida! You have unlocked digital access to the <strong class="text-gtaBlue">"Sunset Highway Pack"</strong> containing custom Vice Neon wrap aesthetics for performance vehicles and dynamic retro sunglasses for Lucia and Jason.</p>
      <div class="mt-6 p-3 bg-black/50 rounded-xl border border-white/5 text-left space-y-2"><div data-i18n="unlocks" class="text-[10px] text-gtaYellow uppercase font-bold tracking-wider">Unlocks included:</div><div data-i18n="unlock1" class="text-xs text-gray-300">✓ Leonida Pink custom wrap</div><div data-i18n="unlock2" class="text-xs text-gray-300">✓ Synth-wave interior lights</div><div data-i18n="unlock3" class="text-xs text-gray-300">✓ Dynamic 80s Soundtrack playlist add-on</div></div>
      <div class="mt-6 flex gap-3"><button onclick="closeBonusModal()" data-i18n="claim" class="flex-1 bg-gtaPink text-white text-xs font-bold uppercase py-3 rounded-xl">Claim for my Station</button><button onclick="closeBonusModal()" data-i18n="close" class="px-4 py-3 rounded-xl bg-white/5 text-xs font-bold uppercase text-gray-400">Close</button></div>
    </div>
  </div>
</div>

<div id="trailerModal" class="fixed inset-0 z-[100] flex items-center justify-center bg-black/90 backdrop-blur-md hidden">
  <div class="border border-white/10 rounded-3xl p-4 bg-[#120721] max-w-4xl w-full mx-4 shadow-2xl relative"><button onclick="closeTrailerEmbed()" data-i18n="closeVideo" class="absolute -top-10 right-0 text-white font-bold text-sm tracking-wider uppercase bg-black/40 px-3 py-1 rounded border border-white/10">✕ Close Video</button><div class="aspect-video rounded-2xl overflow-hidden bg-black"><iframe id="trailerIframe" class="w-full h-full" src="" title="GTA VI Trailer Player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div><div data-i18n="streamFooter" class="mt-3 text-center text-xs text-gray-400">Official Rockstar Games YouTube Stream • Powered by Leonida Intelligence Bureau</div></div>
</div>

<footer class="relative z-10 border-t border-white/5 bg-black/40 py-8 text-center text-xs text-gray-500"><div class="max-w-7xl mx-auto px-4 flex flex-col md:flex-row justify-between items-center gap-4"><div><span class="text-gtaPink font-bold">GTA VI RELEASE COUNTDOWN</span> <span>•</span> <span data-i18n="made">Made with retro passion for GTA Fans</span></div><p data-i18n="disclaimer" class="text-[10px]">Not affiliated with Rockstar Games, Take-Two Interactive, or any subsidiaries. Fan-made dynamic simulation.</p></div></footer>

<script>
const targetDate=new Date("2026-11-19T00:00:00Z").getTime();
const announcementDate=new Date("2023-12-05T14:00:00Z").getTime();
let isSynthPlaying=false,audioCtx=null,synthInterval=null,activePlatform='ps5',currentNewsIndex=0;

const translations={
en:{radio:"Synthwave Radio:",playBeat:"Play Beat",muteBeat:"Mute Beat",coordinates:"Leonida State Launch Coordinates Confirmed",countdown:"Release Countdown",intro:"Locking coordinates onto the most anticipated cultural event of the decade. Live tracking to November 19, 2026.",target:"TARGET:",speculation:"Official Speculation Target",days:"Days",daysLeft:"Days Left",hours:"Hours",hourCycles:"Hour Cycles",minutes:"Minutes",minuteMarks:"Minute Marks",seconds:"Seconds",secondsClock:"Seconds Clock",msPrecision:"Ms Precision",millisecondLoop:"Millisecond Loop",progress:"Time Travel Distance Progression",departed:"DEPARTED: ANNOUNCEMENT (DEC 2023)",arrival:"ARRIVAL: CODENAME LUCIA & JASON",atmosphere:"⚙ Atmosphere Customizer",atmosphereDesc:"Fine-tune the neon lighting of the Leonida Vice Highway live simulation parameters.",crt:"CRT Arcade Filter",crtDesc:"Classic arcade overlay lines",palm:"Palm Tree Sway Wind Speed",highway:"Retro Highway Speed",fireflies:"Double click background to spawn neon fireflies",dossier:"▣ Leonida Dossier Intelligence",location:"Location",protagonists:"Main Protagonists",innovation:"Gameplay Innovation",preorderHub:"Pre-order Hub Mockup",secureSeat:"Secure Your Seat in Vice City",bonusDesc:"Get custom vehicle modifications and exclusive safe-house bonuses upon retail verification.",bonusBtn:"Check Bonus Perks",trailerFeed:"Official Trailer Intel Feed",trailerCount:"2 Official Trailers / 1 Launch Showcase",trailer1:"WATCH TRAILER 1",trailer1Name:"Lucia and Jason Introduction",trailer2:"WATCH TRAILER 2",trailer2Name:'"New Beginnings" Leonida',launchShowcase:"LAUNCH SHOWCASE ↗",launchDesc:"Netflix Launch Showcase • Open link",breaking:"BREAKING NEWS",nextAlert:"Next Alert",modalTitle:"VP Pre-Launch Unlock",modalText:'Congratulations, Citizen of Leonida! You have unlocked digital access to the "Sunset Highway Pack" containing custom Vice Neon wrap aesthetics for performance vehicles and dynamic retro sunglasses for Lucia and Jason.',unlocks:"Unlocks included:",unlock1:"✓ Leonida Pink custom wrap",unlock2:"✓ Synth-wave interior lights",unlock3:"✓ Dynamic 80s Soundtrack playlist add-on",claim:"Claim for my Station",close:"Close",closeVideo:"✕ Close Video",streamFooter:"Official Rockstar Games YouTube Stream • Powered by Leonida Intelligence Bureau",made:"Made with retro passion for GTA Fans",disclaimer:"Not affiliated with Rockstar Games, Take-Two Interactive, or any subsidiaries. Fan-made dynamic simulation."},
hu:{radio:"Synthwave rádió:",playBeat:"Lejátszás",muteBeat:"Némítás",coordinates:"Leonida állam indulási koordinátái megerősítve",countdown:"Megjelenési visszaszámlálás",intro:"Rögzítjük a koordinátákat az évtized egyik legjobban várt kulturális eseményére. Élő követés 2026. november 19-ig.",target:"CÉLPONT:",speculation:"Hivatalos spekulációs célpont",days:"Nap",daysLeft:"Hátralévő napok",hours:"Óra",hourCycles:"Óraciklusok",minutes:"Perc",minuteMarks:"Percjelek",seconds:"Másodperc",secondsClock:"Másodpercóra",msPrecision:"Ms pontosság",millisecondLoop:"Milliszekundumos ciklus",progress:"Időutazási előrehaladás",departed:"INDULÁS: BEJELENTÉS (2023. DEC.)",arrival:"ÉRKEZÉS: LUCIA ÉS JASON",atmosphere:"⚙ Atmoszféra testreszabása",atmosphereDesc:"Állítsd be élőben a Leonida Vice Highway neonvilágítását.",crt:"CRT arcade szűrő",crtDesc:"Klasszikus arcade képernyővonalak",palm:"Pálmafák szélsebessége",highway:"Retro autópálya sebessége",fireflies:"Dupla kattintás a háttérre neon szentjánosbogarakhoz",dossier:"▣ Leonida dosszié",location:"Helyszín",protagonists:"Főszereplők",innovation:"Játékmenet-újdonság",preorderHub:"Előrendelési központ",secureSeat:"Foglalj helyet Vice Cityben",bonusDesc:"Szerezz egyedi járműmódosításokat és exkluzív rejtekhely-bónuszokat.",bonusBtn:"Bónuszok megtekintése",trailerFeed:"Hivatalos trailer információk",trailerCount:"2 hivatalos trailer / 1 Launch Showcase",trailer1:"1. TRAILER",trailer1Name:"Lucia és Jason bemutatkozása",trailer2:"2. TRAILER",trailer2Name:'„Új kezdetek” – Leonida',launchShowcase:"LAUNCH SHOWCASE ↗",launchDesc:"Netflix Launch Showcase • Link megnyitása",breaking:"FRISS HÍR",nextAlert:"Következő riasztás",modalTitle:"VP előzetes feloldás",modalText:"Gratulálunk, Leonida polgára! Feloldottad a Sunset Highway Pack digitális hozzáférését.",unlocks:"Feloldások:",unlock1:"✓ Leonida Pink egyedi fólia",unlock2:"✓ Synthwave belső fények",unlock3:"✓ Dinamikus 80-as évekbeli zenei bővítés",claim:"Igénylés",close:"Bezárás",closeVideo:"✕ Videó bezárása",streamFooter:"Hivatalos Rockstar Games YouTube-adás • Leonida Intelligence Bureau",made:"Retro szenvedéllyel GTA-rajongóknak",disclaimer:"Nem áll kapcsolatban a Rockstar Games-szel, a Take-Two Interactive-val vagy leányvállalataikkal. Rajongói dinamikus szimuláció."},
it:{radio:"Radio Synthwave:",playBeat:"Riproduci",muteBeat:"Muta",coordinates:"Coordinate di lancio dello Stato di Leonida confermate",countdown:"Conto alla rovescia",intro:"Coordinate bloccate sull'evento culturale più atteso del decennio. Monitoraggio fino al 19 novembre 2026.",target:"OBIETTIVO:",speculation:"Obiettivo speculativo ufficiale",days:"Giorni",daysLeft:"Giorni rimanenti",hours:"Ore",hourCycles:"Cicli orari",minutes:"Minuti",minuteMarks:"Indicatori minuti",seconds:"Secondi",secondsClock:"Orologio dei secondi",msPrecision:"Precisione Ms",millisecondLoop:"Ciclo millisecondi",progress:"Progressione del viaggio nel tempo",departed:"PARTENZA: ANNUNCIO (DIC. 2023)",arrival:"ARRIVO: LUCIA E JASON",atmosphere:"⚙ Personalizza atmosfera",atmosphereDesc:"Regola l'illuminazione neon dell'autostrada di Vice City.",crt:"Filtro arcade CRT",crtDesc:"Linee classiche da sala giochi",palm:"Velocità del vento sulle palme",highway:"Velocità autostrada retro",fireflies:"Doppio clic sullo sfondo per creare lucciole neon",dossier:"▣ Dossier Leonida",location:"Località",protagonists:"Protagonisti principali",innovation:"Innovazione gameplay",preorderHub:"Hub preordine",secureSeat:"Prenota il tuo posto a Vice City",bonusDesc:"Ottieni modifiche veicolo personalizzate e bonus esclusivi.",bonusBtn:"Controlla bonus",trailerFeed:"Feed trailer ufficiali",trailerCount:"2 trailer ufficiali / 1 Launch Showcase",trailer1:"TRAILER 1",trailer1Name:"Introduzione di Lucia e Jason",trailer2:"TRAILER 2",trailer2Name:'"Nuovi inizi" Leonida',launchShowcase:"LAUNCH SHOWCASE ↗",launchDesc:"Netflix Launch Showcase • Apri link",breaking:"ULTIME NOTIZIE",nextAlert:"Prossimo avviso",modalTitle:"Sblocco pre-lancio VP",modalText:"Congratulazioni, cittadino di Leonida! Hai sbloccato l'accesso digitale al Sunset Highway Pack.",unlocks:"Sblocchi inclusi:",unlock1:"✓ Livrea personalizzata Leonida Pink",unlock2:"✓ Luci interne synthwave",unlock3:"✓ Aggiunta playlist anni '80",claim:"Riscatta",close:"Chiudi",closeVideo:"✕ Chiudi video",streamFooter:"Stream YouTube ufficiale Rockstar Games • Leonida Intelligence Bureau",made:"Creato con passione retro per i fan di GTA",disclaimer:"Non affiliato a Rockstar Games, Take-Two Interactive o società controllate. Simulazione dinamica fan-made."},
de:{radio:"Synthwave-Radio:",playBeat:"Beat abspielen",muteBeat:"Beat stumm",coordinates:"Startkoordinaten von Leonida State bestätigt",countdown:"Release-Countdown",intro:"Koordinaten für das meist erwartete Kulturevent des Jahrzehnts erfasst. Live-Tracking bis zum 19. November 2026.",target:"ZIEL:",speculation:"Offizielles Spekulationsziel",days:"Tage",daysLeft:"Verbleibende Tage",hours:"Stunden",hourCycles:"Stundenzyklen",minutes:"Minuten",minuteMarks:"Minutenmarken",seconds:"Sekunden",secondsClock:"Sekundenuhr",msPrecision:"Ms-Präzision",millisecondLoop:"Millisekunden-Zyklus",progress:"Zeitreise-Fortschritt",departed:"START: ANKÜNDIGUNG (DEZ. 2023)",arrival:"ANKUNFT: LUCIA & JASON",atmosphere:"⚙ Atmosphäre anpassen",atmosphereDesc:"Neonbeleuchtung der Leonida Vice Highway Live-Simulation anpassen.",crt:"CRT-Arcade-Filter",crtDesc:"Klassische Arcade-Overlay-Linien",palm:"Windgeschwindigkeit der Palmen",highway:"Retro-Highway-Geschwindigkeit",fireflies:"Doppelklick auf den Hintergrund für Neon-Glühwürmchen",dossier:"▣ Leonida-Dossier",location:"Ort",protagonists:"Hauptfiguren",innovation:"Gameplay-Innovation",preorderHub:"Vorbestellungs-Hub",secureSeat:"Sichere dir deinen Platz in Vice City",bonusDesc:"Erhalte individuelle Fahrzeugmods und exklusive Safehouse-Boni.",bonusBtn:"Bonus ansehen",trailerFeed:"Offizieller Trailer-Feed",trailerCount:"2 offizielle Trailer / 1 Launch Showcase",trailer1:"TRAILER 1",trailer1Name:"Einführung von Lucia und Jason",trailer2:"TRAILER 2",trailer2Name:'"Neue Anfänge" Leonida',launchShowcase:"LAUNCH SHOWCASE ↗",launchDesc:"Netflix Launch Showcase • Link öffnen",breaking:"EILMELDUNG",nextAlert:"Nächste Meldung",modalTitle:"VP Pre-Launch-Freischaltung",modalText:"Glückwunsch, Bürger von Leonida! Du hast digitalen Zugang zum Sunset Highway Pack freigeschaltet.",unlocks:"Enthalten:",unlock1:"✓ Leonida Pink Sonderlackierung",unlock2:"✓ Synthwave-Innenbeleuchtung",unlock3:"✓ Dynamische 80er-Soundtrack-Erweiterung",claim:"Einlösen",close:"Schließen",closeVideo:"✕ Video schließen",streamFooter:"Offizieller Rockstar Games YouTube-Stream • Leonida Intelligence Bureau",made:"Mit Retro-Leidenschaft für GTA-Fans erstellt",disclaimer:"Nicht mit Rockstar Games, Take-Two Interactive oder deren Tochtergesellschaften verbunden. Fan-made dynamische Simulation."}
};

function setLanguage(lang){
  const t=translations[lang]||translations.en;
  document.documentElement.lang=lang;
  document.querySelectorAll("[data-i18n]").forEach(el=>{const key=el.dataset.i18n;if(t[key]!==undefined)el.innerText=t[key]});
  const btnText=document.querySelector("#audioBtn span");
  if(btnText)btnText.innerText=isSynthPlaying?t.muteBeat:t.playBeat;
  localStorage.setItem("gtaCountdownLanguage",lang);
}
const savedLang=localStorage.getItem("gtaCountdownLanguage")||"en";
document.getElementById("languageSelect").value=savedLang;
setLanguage(savedLang);

const daysBox=document.getElementById("daysBox"),hoursBox=document.getElementById("hoursBox"),minsBox=document.getElementById("minsBox"),secsBox=document.getElementById("secsBox"),msBox=document.getElementById("msBox"),gmtDisplay=document.getElementById("gmtDisplay"),percentCompleteDisplay=document.getElementById("percentComplete"),progBar=document.getElementById("progBar");
function updateCountdown(){
 const distance=targetDate-Date.now();
 if(distance<0){daysBox.innerText=hoursBox.innerText=minsBox.innerText=secsBox.innerText="00";msBox.innerText="000";percentCompleteDisplay.innerText="100.0000%";progBar.style.width="100%";gmtDisplay.innerText="LAUNCH EVENT IN PROGRESS!";return}
 daysBox.innerText=String(Math.floor(distance/86400000)).padStart(3,"0");
 hoursBox.innerText=String(Math.floor(distance%86400000/3600000)).padStart(2,"0");
 minsBox.innerText=String(Math.floor(distance%3600000/60000)).padStart(2,"0");
 secsBox.innerText=String(Math.floor(distance%60000/1000)).padStart(2,"0");
 msBox.innerText=String(distance%1000).padStart(3,"0");
 gmtDisplay.innerText=`YOUR TIME: ${new Date().toUTCString().replace("GMT","UTC")}`;
 let percent=(Date.now()-announcementDate)/(targetDate-announcementDate)*100;percent=Math.max(0,Math.min(100,percent));percentCompleteDisplay.innerText=percent.toFixed(6)+"%";progBar.style.width=percent+"%";
}
setInterval(updateCountdown,37);updateCountdown();

const newsHeadlines=[
"Leonida Coast Guard warns of highly dangerous neon sunsets and synthwave music storms...",
"Grand Theft Auto VI features unprecedented custom density and vibrant night life in Vice City.",
"Lucia and Jason spotted drifting neon sports cars down Port Gellhorn ocean side boulevard.",
"Vice City local radio hosts declare synthetic beats the official sound of winter season.",
"Fans expect groundbreaking artificial intelligence behavior from Rockstar Games next masterpiece."
];
function shuffleNews(){currentNewsIndex=(currentNewsIndex+1)%newsHeadlines.length;const f=document.getElementById("breakingNewsFeed");f.style.opacity=0;setTimeout(()=>{f.innerText=`"${newsHeadlines[currentNewsIndex]}"`;f.style.opacity=1;triggerSoundEffect(520,.08)},150)}

function toggleScanlines(){const crt=document.getElementById("crtOverlay"),beam=document.getElementById("scanlineBeam"),knob=document.getElementById("scanlinesKnob"),btn=document.getElementById("scanlinesToggle");const hidden=crt.classList.toggle("hidden");beam.classList.toggle("hidden",hidden);knob.classList.toggle("translate-x-0",hidden);knob.classList.toggle("translate-x-5",!hidden);btn.classList.toggle("bg-gray-700",hidden);btn.classList.toggle("bg-gtaPink",!hidden);triggerSoundEffect(300,.1)}
function changeSwaySpeed(v){const l=document.getElementById("leftPalm"),r=document.getElementById("rightPalm"),label=document.getElementById("swaySpeedLabel");const d=v==="1"?["18s","22s","Calm"]:v==="3"?["4s","5s","Turbulent Coast"]:["10s","12s","Medium"];l.style.animationDuration=d[0];r.style.animationDuration=d[1];label.innerText=d[2];triggerSoundEffect(440,.05)}
function changeGridSpeed(v){const g=document.querySelector(".synth-grid"),label=document.getElementById("gridSpeedLabel");const d=v==="1"?["40s","Sunset Coast"]:v==="2"?["25s","Standard Highway"]:["12s","Vice Nitro Rush"];label.innerText=d[1];if(g)g.style.animationDuration=d[0];triggerSoundEffect(600,.05)}
function selectPlatform(p){activePlatform=p;const a=document.getElementById("platform-ps5"),b=document.getElementById("platform-xbox");a.className=p==="ps5"?"px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-gtaBlue bg-gtaBlue/20 text-white":"px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-white/10 text-gray-400";b.className=p==="xbox"?"px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-gtaPink bg-gtaPink/20 text-white":"px-2.5 py-0.5 rounded text-[10px] font-bold tracking-widest border border-white/10 text-gray-400";triggerSoundEffect(p==="ps5"?700:600,.08)}
function showBonusModal(){document.getElementById("bonusModal").classList.remove("hidden");triggerSoundEffect(523.25,.15)}
function closeBonusModal(){document.getElementById("bonusModal").classList.add("hidden");triggerSoundEffect(392,.1)}
function openTrailerEmbed(id){document.getElementById("trailerIframe").src=`https://www.youtube.com/embed/${id}?autoplay=1`;document.getElementById("trailerModal").classList.remove("hidden");if(isSynthPlaying)toggleSynthAudio()}
function closeTrailerEmbed(){document.getElementById("trailerIframe").src="";document.getElementById("trailerModal").classList.add("hidden");triggerSoundEffect(300,.1)}

function initAudioContext(){if(!audioCtx)audioCtx=new(window.AudioContext||window.webkitAudioContext)()}
function triggerSoundEffect(freq,duration){try{initAudioContext();if(audioCtx.state==="suspended")audioCtx.resume();const o=audioCtx.createOscillator(),g=audioCtx.createGain();o.type="triangle";o.frequency.setValueAtTime(freq,audioCtx.currentTime);g.gain.setValueAtTime(.04,audioCtx.currentTime);g.gain.exponentialRampToValueAtTime(.001,audioCtx.currentTime+duration);o.connect(g);g.connect(audioCtx.destination);o.start();o.stop(audioCtx.currentTime+duration)}catch(e){}}
function toggleSoundEffect(){triggerSoundEffect(880,.2)}
function toggleSynthAudio(){
 initAudioContext();const btn=document.getElementById("audioBtn"),t=translations[document.documentElement.lang]||translations.en;
 if(isSynthPlaying){clearInterval(synthInterval);isSynthPlaying=false;btn.querySelector("span").innerText=t.playBeat;btn.classList.remove("bg-gtaBlue");btn.classList.add("bg-gtaPink");triggerSoundEffect(220,.3);return}
 if(audioCtx.state==="suspended")audioCtx.resume();isSynthPlaying=true;btn.querySelector("span").innerText=t.muteBeat;btn.classList.remove("bg-gtaPink");btn.classList.add("bg-gtaBlue");
 let step=0;const bass=[110,110,110,110,87.31,87.31,87.31,87.31,130.81,130.81,130.81,130.81,98,98,98,98],melody=[220,261.63,329.63,440,174.61,220,261.63,349.23,261.63,329.63,392,523.25,196,246.94,293.66,392];
 synthInterval=setInterval(()=>{const b=audioCtx.createOscillator(),g=audioCtx.createGain();b.type="sawtooth";b.frequency.value=bass[step%16];g.gain.setValueAtTime(.06,audioCtx.currentTime);g.gain.exponentialRampToValueAtTime(.001,audioCtx.currentTime+.22);b.connect(g);g.connect(audioCtx.destination);b.start();b.stop(audioCtx.currentTime+.24);if(step%2===0){const o=audioCtx.createOscillator(),gg=audioCtx.createGain();o.type="triangle";o.frequency.value=melody[step%16];gg.gain.setValueAtTime(.03,audioCtx.currentTime);gg.gain.exponentialRampToValueAtTime(.001,audioCtx.currentTime+.15);o.connect(gg);gg.connect(audioCtx.destination);o.start();o.stop(audioCtx.currentTime+.2)}step++},160)
}

const canvas=document.getElementById("ambientParticles"),ctx=canvas.getContext("2d");let particles=[],customSpawnedParticles=[];
function resizeCanvas(){canvas.width=innerWidth;canvas.height=innerHeight}addEventListener("resize",resizeCanvas);resizeCanvas();
class Particle{constructor(x,y){this.x=x??Math.random()*canvas.width;this.y=y??Math.random()*canvas.height;this.size=Math.random()*2+1;this.speedX=(Math.random()-.5)*1.5;this.speedY=-(Math.random()*1.5+.5);this.color=Math.random()>.5?"#ff007f":"#00f0ff";this.alpha=1;this.fadeSpeed=Math.random()*.005+.003}update(){this.x+=this.speedX;this.y+=this.speedY;this.alpha-=this.fadeSpeed}draw(){ctx.save();ctx.globalAlpha=this.alpha;ctx.shadowBlur=8;ctx.shadowColor=this.color;ctx.fillStyle=this.color;ctx.beginPath();ctx.arc(this.x,this.y,this.size,0,Math.PI*2);ctx.fill();ctx.restore()}}
for(let i=0;i<40;i++)particles.push(new Particle());
function animateParticles(){ctx.clearRect(0,0,canvas.width,canvas.height);particles.forEach((p,i)=>{p.update();p.draw();if(p.alpha<=0||p.y<0)particles[i]=new Particle()});customSpawnedParticles.forEach((p,i)=>{p.update();p.draw();if(p.alpha<=0||p.y<0)customSpawnedParticles.splice(i,1)});requestAnimationFrame(animateParticles)}animateParticles();
document.addEventListener("dblclick",e=>{for(let i=0;i<15;i++)customSpawnedParticles.push(new Particle(e.clientX,e.clientY))});
document.addEventListener("touchstart",e=>{if(e.touches?.[0]&&!e.target.closest("button")&&!e.target.closest("#bonusModal"))for(let i=0;i<8;i++)customSpawnedParticles.push(new Particle(e.touches[0].clientX,e.touches[0].clientY))});

const retroCar=document.getElementById("retroCar");
function driveRetroCar(){const duration=Math.random()*4000+6000;retroCar.style.transitionDuration=`${duration}ms`;retroCar.style.left="100%";setTimeout(()=>{retroCar.style.transitionDuration="0ms";retroCar.style.left="-40px";const pink=Math.random()>.5;retroCar.style.backgroundColor=pink?"#ff007f":"#00f0ff";retroCar.style.boxShadow=pink?"0 0 10px #ff007f":"0 0 10px #00f0ff";setTimeout(driveRetroCar,Math.random()*4000+1000)},duration+50)}driveRetroCar();
</script>
</body>
</html>
