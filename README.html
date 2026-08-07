<---# b.tech-1st-year-2026--->
<---07-08-2006, today we have to make a virtual pet using ai tools(gpt/claude)--->
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Pixel Cat Companion</title>
<style>
  html, body {
    margin: 0;
    padding: 0;
    height: 100%;
    overflow: hidden;
    --sky-top: #7ec8e3;
    --sky-bottom: #bfe8f0;
    --grass-top: #9fd88a;
    --grass-bottom: #6fbf5f;
    background: linear-gradient(to bottom, var(--sky-top) 0%, var(--sky-bottom) 55%, var(--grass-top) 55%, var(--grass-bottom) 100%);
    font-family: 'Courier New', monospace;
    cursor: default;
  }

 #hint {
    position: fixed;
    top: 18px;
    left: 50%;
    transform: translateX(-50%);
    background: rgba(20, 20, 30, 0.55);
    color: #fff;
    padding: 8px 16px;
    border-radius: 8px;
    font-size: 13px;
    letter-spacing: 0.3px;
    text-align: center;
    pointer-events: none;
    z-index: 10000;
    transition: opacity 0.3s ease;
  }

  #shadow {
    position: fixed;
    width: 60px;
    height: 14px;
    background: rgba(10, 10, 10, 0.28);
    border-radius: 50%;
    filter: blur(1px);
    pointer-events: none;
    z-index: 9998;
  }

  #catCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 9999;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  #yarnCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 9999;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  #fishCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 9999;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  #handCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 10002;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  #sceneryCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 2;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  #nightOverlay {
    position: fixed;
    left: 0;
    top: 55%;
    width: 100%;
    height: 45%;
    background: rgba(6, 10, 28, 0);
    pointer-events: none;
    z-index: 3;
  }

  #cloudCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 0;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  .butterfly-canvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 40;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  .autoCatCanvas {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    z-index: 9990;
    image-rendering: pixelated;
    image-rendering: -moz-crisp-edges;
    image-rendering: crisp-edges;
  }

  .autoCatShadow {
    position: fixed;
    width: 48px;
    height: 11px;
    background: rgba(10, 10, 10, 0.26);
    border-radius: 50%;
    filter: blur(1px);
    pointer-events: none;
    z-index: 9989;
  }

  .floaty {
    position: fixed;
    color: #ffffff;
    font-weight: bold;
    font-size: 18px;
    text-shadow: 0 0 3px #000, 0 0 1px #000;
    pointer-events: none;
    z-index: 10001;
    animation: floatUp 1.6s ease-out forwards;
  }

  @keyframes floatUp {
    0%   { opacity: 0; transform: translateY(0) scale(0.7); }
    15%  { opacity: 1; }
    100% { opacity: 0; transform: translateY(-45px) scale(1.3); }
  }

  #panel {
    position: fixed;
    bottom: 22px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 10px;
    z-index: 10000;
  }

  #panel button {
    font-family: 'Courier New', monospace;
    font-size: 14px;
    font-weight: bold;
    padding: 10px 16px;
    border: 2px solid #4a2f2c;
    border-radius: 10px;
    background: #fff6ee;
    color: #4a2f2c;
    cursor: pointer;
    box-shadow: 0 3px 0 #4a2f2c;
    transition: transform 0.08s ease, box-shadow 0.08s ease, background 0.15s ease;
  }

  #panel button:hover {
    background: #ffe4ee;
  }

  #panel button:active {
    transform: translateY(3px);
    box-shadow: 0 0 0 #4a2f2c;
  }

  #panel button.active {
    background: #cdb9ae;
    color: #fff6ee;
  }
</style>
</head>
<body>

<div id="hint">Move your mouse to lead the cat around, or use the buttons to feed it, pet it, or have it stay put.</div>
<canvas id="cloudCanvas"></canvas>
<canvas id="sceneryCanvas"></canvas>
<div id="nightOverlay"></div>
<div id="shadow"></div>
<canvas id="catCanvas"></canvas>
<canvas id="yarnCanvas"></canvas>
<canvas id="fishCanvas"></canvas>
<canvas id="handCanvas"></canvas>

<div id="panel">
  <button id="feedBtn" type="button">🐟 Feed</button>
  <button id="petBtn" type="button">✋ Pet</button>
  <button id="playBtn" type="button">🧶 Play</button>
  <button id="stayBtn" type="button">📍 Stay Here</button>
</div>


<script>
(function () {
  "use strict";

  /* ---------------------------------------------------------
     PIXEL ART DATA
     Each frame is an array of row-strings. Each character is
     one "pixel". '.' = transparent, everything else is looked
     up in COLORS below.
  --------------------------------------------------------- */

  const COLORS = {
    K: "#4a2f2c", // dark maroon outline
    F: "#cdb9ae", // taupe/grey fur
    D: "#a68f86", // darker tabby stripe & tail
    W: "#fdf6f0", // white/cream chest
    P: "#f4b6c8"  // pink ears & nose
  };

  const YARN_COLORS = {
    Y: "#d94f4f", // yarn red
    S: "#a63636"  // yarn shade / cross lines
  };

  const YARN_BALL = [
    "..YYY..",
    ".YSYSY.",
    "YSYYYSY",
    "YYYSYYY",
    "YSYYYSY",
    ".YSYSY.",
    "..YYY.."
  ];

  const FISH_COLORS = {
    O: "#f2914a", // fish body
    D: "#c9642a", // fin / tail shade
    E: "#2a2a2a"  // eye
  };

  const FISH = [
    "...OOOO..",
    "..OOOOOOD",
    ".OOOOEOOD",
    "..OOOOOOD",
    "...OOOO.."
  ];

  const HAND_COLORS = {
    S: "#e8b48c", // skin
    O: "#a9765a"  // outline / shading
  };

  const HAND = [
    ".OOOOO.",
    "OSSSSSO",
    "OSSSSSO",
    "OSSSSSO",
    ".OOOOO.",
    "...O..."
  ];

  // Sitting, tail curled out to the side, pink ears & nose,
  // soft grey-taupe tabby fur — inspired by the reference photo's
  // palette and pose (an original drawing, not a pixel copy of it).
  const SIT = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    "DK.....KFFWWWWFFK.",
    "KD.....KFFWWWWFFK.",
    "KDDDDDDDKKFFFFKK..",
    ".KKKKKKK.........."
  ];

  const SLEEP = SIT; // same pose; distinguished by the bob & "z" animation

  const WALK_A = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    ".......KF......FK.",
    "........K.FFFF.K..",
    ".........K....K..."
  ];

  const WALK_B = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    ".......KFFWWWWFFK.",
    "........K......K..",
    ".........K....K..."
  ];

  const PIXEL = 4.5;    // px size of a single "pixel" (0.5x scale)
  const GRID_W = 18;
  const GRID_H = 13;
  const CAT_W = GRID_W * PIXEL;
  const CAT_H = GRID_H * PIXEL;

  /* ---------------------------------------------------------
     CANVAS SETUP
  --------------------------------------------------------- */

  const canvas = document.getElementById("catCanvas");
  const ctx = canvas.getContext("2d");

  const yarnCanvas = document.getElementById("yarnCanvas");
  const yarnCtx = yarnCanvas.getContext("2d");
  const YARN_PIXEL = 6;
  yarnCanvas.width = YARN_BALL[0].length * YARN_PIXEL;
  yarnCanvas.height = YARN_BALL.length * YARN_PIXEL;

  const fishCanvas = document.getElementById("fishCanvas");
  const fishCtx = fishCanvas.getContext("2d");
  const FISH_PIXEL = 6;
  fishCanvas.width = FISH[0].length * FISH_PIXEL;
  fishCanvas.height = FISH.length * FISH_PIXEL;
  fishCanvas.style.transformOrigin = "50% 50%";

  const handCanvas = document.getElementById("handCanvas");
  const handCtx = handCanvas.getContext("2d");
  const HAND_PIXEL = 7;
  handCanvas.width = HAND[0].length * HAND_PIXEL;
  handCanvas.height = HAND.length * HAND_PIXEL;

  // Give the canvas some breathing room around the sprite so
  // flipping (scaleX) and the bob animation never clip.
  const PAD = 10;
  canvas.width = CAT_W + PAD * 2;
  canvas.height = CAT_H + PAD * 2;

  function drawGrid(targetCtx, rows, colors, pixelSize) {
    for (let r = 0; r < rows.length; r++) {
      const row = rows[r];
      for (let c = 0; c < row.length; c++) {
        const color = colors[row[c]];
        if (color) {
          targetCtx.fillStyle = color;
          targetCtx.fillRect(c * pixelSize, r * pixelSize, pixelSize, pixelSize);
        }
      }
    }
  }

  function drawYarnBall() {
    yarnCtx.clearRect(0, 0, yarnCanvas.width, yarnCanvas.height);
    drawGrid(yarnCtx, YARN_BALL, YARN_COLORS, YARN_PIXEL);
  }

  // Fish and hand sprites don't change shape frame to frame, so draw
  // them once and animate position/scale via CSS instead of redrawing.
  drawGrid(fishCtx, FISH, FISH_COLORS, FISH_PIXEL);
  drawGrid(handCtx, HAND, HAND_COLORS, HAND_PIXEL);

  function drawFrame(rows, flip) {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    ctx.save();
    if (flip === -1) {
      ctx.translate(canvas.width, 0);
      ctx.scale(-1, 1);
    }
    for (let r = 0; r < rows.length; r++) {
      const row = rows[r];
      for (let c = 0; c < row.length; c++) {
        const ch = row[c];
        const color = COLORS[ch];
        if (color) {
          ctx.fillStyle = color;
          ctx.fillRect(PAD + c * PIXEL, PAD + r * PIXEL, PIXEL, PIXEL);
        }
      }
    }
    ctx.restore();
  }

  /* ---------------------------------------------------------
     STATE
  --------------------------------------------------------- */

  const hint = document.getElementById("hint");
  const groundShadow = document.getElementById("shadow");
  const feedBtn = document.getElementById("feedBtn");
  const petBtn = document.getElementById("petBtn");
  const playBtn = document.getElementById("playBtn");
  const stayBtn = document.getElementById("stayBtn");

  let mouse = { x: window.innerWidth / 2, y: window.innerHeight / 2 };
  let pos = { x: mouse.x - CAT_W / 2, y: mouse.y - CAT_H / 2 };
  let facing = 1;
  let lastInput = Date.now();
  let state = "sit"; // 'walk' | 'sit' | 'sleep' | 'eating' | 'petting' | 'playing'
  let lastZ = 0;

  let pinned = false;        // when true, the cat stays put instead of chasing the cursor
  let action = null;         // 'eating' | 'petting' | 'playing' | null — temporary override
  let actionUntil = 0;
  let lastActionParticle = 0;
  let playStart = 0;
  let eatStart = 0;
  let petStart = 0;

  const REACH_DIST = 55;   // how close the cat needs to get before it stops chasing
  const IDLE_MS = 4000;    // how long with no input before the cat falls asleep
  const EASE = 0.035;      // follow smoothing (lower = slower cat)

  function registerInput(x, y) {
    if (typeof x === "number") { mouse.x = x; mouse.y = y; }
    lastInput = Date.now();
    if (hint) hint.style.opacity = "1";
  }

  window.addEventListener("mousemove", (e) => registerInput(e.clientX, e.clientY));
  window.addEventListener("mousedown", () => registerInput());
  window.addEventListener("keydown", () => registerInput());
  window.addEventListener("touchmove", (e) => {
    if (e.touches && e.touches.length > 0) {
      registerInput(e.touches[0].clientX, e.touches[0].clientY);
    }
  }, { passive: true });
  window.addEventListener("touchstart", (e) => {
    if (e.touches && e.touches.length > 0) {
      registerInput(e.touches[0].clientX, e.touches[0].clientY);
    }
  }, { passive: true });

  function spawnFloaty(text, xOffset) {
    const el = document.createElement("div");
    el.className = "floaty";
    el.textContent = text;
    el.style.left = (pos.x + CAT_W / 2 - 8 + (xOffset || 0) + Math.random() * 10) + "px";
    el.style.top = (pos.y - 6) + "px";
    document.body.appendChild(el);
    el.addEventListener("animationend", () => el.remove());
  }

  function startAction(name, durationMs) {
    registerInput();          // wakes the cat up and counts as activity
    action = name;
    actionUntil = Date.now() + durationMs;
    lastActionParticle = 0;   // spawn a particle right away
    if (name === "playing") playStart = Date.now();
    if (name === "eating") eatStart = Date.now();
    if (name === "petting") petStart = Date.now();
  }

  feedBtn.addEventListener("click", () => startAction("eating", 1400));
  petBtn.addEventListener("click", () => startAction("petting", 1000));
  playBtn.addEventListener("click", () => startAction("playing", 2600));

  function togglePinned() {
    pinned = !pinned;
    registerInput();
    stayBtn.textContent = pinned ? "🚶 Let Go" : "📍 Stay Here";
    stayBtn.classList.toggle("active", pinned);
  }

  stayBtn.addEventListener("click", togglePinned);
  window.addEventListener("dblclick", (e) => {
    if (e.target.closest && e.target.closest("#panel")) return;
    togglePinned();
  });



  /* ---------------------------------------------------------
     MAIN LOOP
  --------------------------------------------------------- */

  function tick() {
    const now = Date.now();
    const idle = (now - lastInput) > IDLE_MS;

    if (action && now < actionUntil) {
      // Feeding / petting overrides normal movement for a moment.
      state = action;
    } else {
      action = null;

      if (pinned) {
        // Cat stays exactly where it is; only idle/sleep still applies.
        state = idle ? "sleep" : "sit";
      } else {
        const targetX = mouse.x - CAT_W / 2;
        const targetY = mouse.y - CAT_H / 2 + 8;
        const catCenterX = pos.x + CAT_W / 2;
        const catCenterY = pos.y + CAT_H / 2;
        const dist = Math.hypot(mouse.x - catCenterX, mouse.y - catCenterY);

        if (dist > REACH_DIST) {
          const dx = targetX - pos.x;
          const dy = targetY - pos.y;
          pos.x += dx * EASE;
          pos.y += dy * EASE;
          if (Math.abs(dx) > 2) facing = dx < 0 ? -1 : 1;
          state = "walk";
        } else {
          state = idle ? "sleep" : "sit";
        }
      }
    }

    // choose frame
    let frame;
    let bob = 0;
    if (state === "walk") {
      frame = (Math.floor(now / 180) % 2 === 0) ? WALK_A : WALK_B;
    } else if (state === "sleep") {
      frame = SLEEP;
      bob = Math.sin(now / 300) * 2; // gentle breathing bob
      if (now - lastZ > 900) {
        lastZ = now;
        spawnFloaty("z", CAT_W / 2 - 10);
      }
    } else if (state === "eating") {
      frame = SIT;
      bob = Math.abs(Math.sin(now / 90)) * -2; // little munching bob
      if (now - lastActionParticle > 350) {
        lastActionParticle = now;
        spawnFloaty("🐟", -6);
      }
    } else if (state === "eating") {
      frame = SIT;
      bob = Math.abs(Math.sin(now / 90)) * -2; // little munching bob
      if (now - lastActionParticle > 350) {
        lastActionParticle = now;
        spawnFloaty("🐟", -6);
      }
    } else if (state === "petting") {
      frame = SIT;
      bob = Math.sin(now / 120) * 1.5; // happy wiggle
      if (now - lastActionParticle > 300) {
        lastActionParticle = now;
        spawnFloaty("💛", -6);
      }
    } else if (state === "playing") {
      const elapsed = now - playStart;
      frame = (Math.floor(elapsed / 160) % 2 === 0) ? WALK_A : WALK_B; // playful paw motion
      bob = Math.abs(Math.sin(elapsed / 140)) * -3; // energetic pounce bob
      if (now - lastActionParticle > 500) {
        lastActionParticle = now;
        spawnFloaty("🧶", -4);
      }
    } else {
      frame = SIT;
    }

    drawFrame(frame, facing);

    if (state === "eating") {
      const elapsed = now - eatStart;
      const nibbleShrink = Math.max(0.15, 1 - elapsed / 1400); // fish gets nibbled away
      const nibbleWiggle = Math.sin(elapsed / 70) * 2;
      const fishX = pos.x + CAT_W / 2 + facing * 16 - fishCanvas.width / 2;
      const fishY = pos.y + CAT_H * 0.6 + nibbleWiggle;
      fishCanvas.style.left = fishX + "px";
      fishCanvas.style.top = fishY + "px";
      fishCanvas.style.transform = `scale(${nibbleShrink})`;
      fishCanvas.style.display = "block";
    } else {
      fishCanvas.style.display = "none";
    }

    if (state === "petting") {
      const elapsed = now - petStart;
      const pat = Math.abs(Math.sin(elapsed / 150)) * 6; // gentle patting bounce
      const handX = pos.x + CAT_W / 2 - handCanvas.width / 2;
      const handY = pos.y - handCanvas.height * 0.55 + pat;
      handCanvas.style.left = handX + "px";
      handCanvas.style.top = handY + "px";
      handCanvas.style.display = "block";
    } else {
      handCanvas.style.display = "none";
    }

    if (state === "playing") {
      const elapsed = now - playStart;
      const swing = Math.sin(elapsed / 260) * 34; // ball swings side to side
      const bounce = Math.abs(Math.sin(elapsed / 210)) * -20; // ball bounces
      const ballX = pos.x + CAT_W / 2 + facing * 26 + swing - yarnCanvas.width / 2;
      const ballY = pos.y + CAT_H - 14 + bounce;
      drawYarnBall();
      yarnCanvas.style.left = ballX + "px";
      yarnCanvas.style.top = ballY + "px";
      yarnCanvas.style.display = "block";
    } else {
      yarnCanvas.style.display = "none";
    }

    canvas.style.left = (pos.x - PAD) + "px";
    canvas.style.top = (pos.y - PAD + bob) + "px";

    groundShadow.style.left = (pos.x + CAT_W / 2 - 30) + "px";
    groundShadow.style.top = (pos.y + CAT_H - 6) + "px";
    groundShadow.style.opacity = state === "sleep" ? "0.5" : "0.8";

    // fade the hint text away after the first bit of activity, then keep it subtle
    if (now - lastInput > IDLE_MS && hint) {
      hint.style.opacity = "0.35";
    }

    requestAnimationFrame(tick);
  }

  requestAnimationFrame(tick);
})();
</script>

<script>
(function () {
  "use strict";

  /* ---------------------------------------------------------
     PARK SCENERY: pixel-art trees & shrubs, plus butterflies
     that drift across the scene.
  --------------------------------------------------------- */

  const PLANT_COLORS = {
    L: "#5fa84f", // mid leaf green
    D: "#3f7a38", // dark leaf shade
    H: "#8fd67a", // leaf highlight
    T: "#6b4a3a"  // trunk brown
  };

  const TREE = [
    "...LLLLL...",
    "..LLLLLLL..",
    ".LLLDLDLLL.",
    "LLLDDDDDLLL",
    "LLLDLHLDLLL",
    ".LLDDDDDLL.",
    "..LLLLLLL..",
    "...LLLLL...",
    ".....T.....",
    ".....T.....",
    ".....T.....",
    ".....T....."
  ];

  const SHRUB = [
    "..LLL..",
    ".LLDLL.",
    "LLDDDLL",
    ".LLDLL.",
    "..LLL.."
  ];

  const SUN_COLORS = {
    Y: "#ffd94a", // sun body
    O: "#ffb703"  // ray tips
  };

  const SUN = [
    "....O.O....",
    ".....Y.....",
    "..YYYYYYY..",
    ".YYYYYYYYY.",
    "OYYYYYYYYYO",
    ".YYYYYYYYY.",
    "OYYYYYYYYYO",
    ".YYYYYYYYY.",
    "..YYYYYYY..",
    ".....Y.....",
    "....O.O...."
  ];

  const MOON_COLORS = {
    M: "#eef1fa", // moon body
    C: "#c9cee0"  // crater shade
  };

  const MOON = [
    "...MMMMM...",
    "..MMMMMMM..",
    ".MMMMMMMMM.",
    "MMMCMMMMMMM",
    "MMMMMMMMMMM",
    "MMMMMMMCMMM",
    "MMMMMMMMMMM",
    "MMCMMMMMMMM",
    ".MMMMMMMMM.",
    "..MMMMMMM..",
    "...MMMMM..."
  ];

  const CLOUD_COLORS = {
    W: "#ffffff", // cloud body
    G: "#e4eef2"  // cloud underside shadow
  };

  const CLOUD = [
    "....WWWW.....",
    "..WWWWWWWWW..",
    ".WWWWWWWWWWW.",
    "WWWWWWWWWWWWW",
    ".GGGGGGGGGGG."
  ];

  function drawPixelGrid(ctx, rows, colors, x, y, pixelSize) {
    for (let r = 0; r < rows.length; r++) {
      const row = rows[r];
      for (let c = 0; c < row.length; c++) {
        const color = colors[row[c]];
        if (color) {
          ctx.fillStyle = color;
          ctx.fillRect(Math.round(x + c * pixelSize), Math.round(y + r * pixelSize), pixelSize, pixelSize);
        }
      }
    }
  }

  function hexToRgb(hex) {
    const n = parseInt(hex.slice(1), 16);
    return [(n >> 16) & 255, (n >> 8) & 255, n & 255];
  }

  function lerpColor(hexA, hexB, t) {
    const a = hexToRgb(hexA);
    const b = hexToRgb(hexB);
    const r = Math.round(a[0] + (b[0] - a[0]) * t);
    const g = Math.round(a[1] + (b[1] - a[1]) * t);
    const bl = Math.round(a[2] + (b[2] - a[2]) * t);
    return `rgb(${r}, ${g}, ${bl})`;
  }

  const DAY_COLORS = { skyTop: "#7ec8e3", skyBottom: "#bfe8f0", grassTop: "#9fd88a", grassBottom: "#6fbf5f" };
  const NIGHT_COLORS = { skyTop: "#0a1030", skyBottom: "#1c2452", grassTop: "#152a12", grassBottom: "#0d1a0a" };
  const NIGHT_TRANSITION_MS = 5 * 60 * 1000; // fully night after 5 minutes
  const dayStartTime = performance.now();
  const rootStyle = document.documentElement.style;
  const nightOverlay = document.getElementById("nightOverlay");

  const STARS = Array.from({ length: 55 }, () => ({
    xPercent: Math.random(),
    yPercent: Math.random() * 0.5,
    size: 1 + Math.random() * 2,
    phase: Math.random() * Math.PI * 2,
    speed: 0.5 + Math.random() * 1.2
  }));

  function updateDayNight(now) {
    const progress = Math.min(1, (now - dayStartTime) / NIGHT_TRANSITION_MS);
    rootStyle.setProperty("--sky-top", lerpColor(DAY_COLORS.skyTop, NIGHT_COLORS.skyTop, progress));
    rootStyle.setProperty("--sky-bottom", lerpColor(DAY_COLORS.skyBottom, NIGHT_COLORS.skyBottom, progress));
    rootStyle.setProperty("--grass-top", lerpColor(DAY_COLORS.grassTop, NIGHT_COLORS.grassTop, progress));
    rootStyle.setProperty("--grass-bottom", lerpColor(DAY_COLORS.grassBottom, NIGHT_COLORS.grassBottom, progress));
    nightOverlay.style.background = `rgba(6, 10, 28, ${progress * 0.55})`;
    return progress;
  }

  // Layout of the park: spread across the width, with a little
  // scale variance so it doesn't feel perfectly uniform.
  const SCENERY_LAYOUT = [
    { type: "tree",  xPercent: 0.04, scale: 1.15 },
    { type: "shrub", xPercent: 0.13, scale: 1.0 },
    { type: "tree",  xPercent: 0.21, scale: 0.85 },
    { type: "shrub", xPercent: 0.32, scale: 1.2 },
    { type: "tree",  xPercent: 0.42, scale: 1.3 },
    { type: "shrub", xPercent: 0.53, scale: 0.9 },
    { type: "tree",  xPercent: 0.63, scale: 0.95 },
    { type: "shrub", xPercent: 0.71, scale: 1.05 },
    { type: "tree",  xPercent: 0.80, scale: 1.2 },
    { type: "shrub", xPercent: 0.89, scale: 1.0 },
    { type: "tree",  xPercent: 0.95, scale: 0.9 }
  ];

  const sceneryCanvas = document.getElementById("sceneryCanvas");
  const sceneryCtx = sceneryCanvas.getContext("2d");

  const cloudCanvas = document.getElementById("cloudCanvas");
  const cloudCtx = cloudCanvas.getContext("2d");

  const CLOUD_PIXEL = 5;
  const clouds = [
    { yPercent: 0.10, speed: 6,  scale: 1.2, x: 0 },
    { yPercent: 0.06, speed: 9,  scale: 0.8, x: 0 },
    { yPercent: 0.17, speed: 4.5, scale: 1.0, x: 0 },
    { yPercent: 0.22, speed: 7.5, scale: 0.65, x: 0 }
  ];
  let cloudsInitialized = false;
  let lastSkyFrameTime = 0;

  function layoutSky() {
    cloudCanvas.width = window.innerWidth;
    cloudCanvas.height = window.innerHeight;
    if (!cloudsInitialized) {
      // Spread clouds across (and a bit beyond) the screen on first layout.
      clouds.forEach((cloud, i) => {
        cloud.x = (window.innerWidth / clouds.length) * i + Math.random() * 80;
      });
      cloudsInitialized = true;
    }
  }

  function drawSky(now) {
    const dt = lastSkyFrameTime ? (now - lastSkyFrameTime) / 1000 : 0;
    lastSkyFrameTime = now;

    const progress = updateDayNight(now);

    const w = cloudCanvas.width;
    const h = cloudCanvas.height;
    cloudCtx.clearRect(0, 0, w, h);

    // Stars fade in as night falls, each twinkling slightly out of sync.
    if (progress > 0) {
      STARS.forEach((star) => {
        const twinkle = 0.55 + 0.45 * Math.sin(now / 600 * star.speed + star.phase);
        cloudCtx.globalAlpha = Math.max(0, progress * twinkle);
        cloudCtx.fillStyle = "#ffffff";
        cloudCtx.fillRect(star.xPercent * w, star.yPercent * h, star.size, star.size);
      });
      cloudCtx.globalAlpha = 1;
    }

    // Sun sets while the moon rises in over the same spot in the sky.
    const sunPixel = 7;
    const sunX = w * 0.86 - (SUN[0].length * sunPixel) / 2;
    const sunY = h * 0.10;

    if (progress < 1) {
      cloudCtx.globalAlpha = 1 - progress;
      drawPixelGrid(cloudCtx, SUN, SUN_COLORS, sunX, sunY, sunPixel);
      cloudCtx.globalAlpha = 1;
    }
    if (progress > 0) {
      cloudCtx.globalAlpha = progress;
      drawPixelGrid(cloudCtx, MOON, MOON_COLORS, sunX, sunY, sunPixel);
      cloudCtx.globalAlpha = 1;
    }

    clouds.forEach((cloud) => {
      const pixelSize = CLOUD_PIXEL * cloud.scale;
      const totalW = CLOUD[0].length * pixelSize;
      cloud.x += cloud.speed * dt;
      if (cloud.x > w + totalW) cloud.x = -totalW;
      const y = h * cloud.yPercent;
      cloudCtx.globalAlpha = 1 - progress * 0.35; // clouds dim a touch at night
      drawPixelGrid(cloudCtx, CLOUD, CLOUD_COLORS, cloud.x, y, pixelSize);
      cloudCtx.globalAlpha = 1;
    });
  }

  layoutSky();
  drawSky(performance.now());

  function drawScenery() {
    const w = window.innerWidth;
    const h = window.innerHeight;
    sceneryCanvas.width = w;
    sceneryCanvas.height = h;
    sceneryCtx.clearRect(0, 0, w, h);

    const grassY = h * 0.55; // matches the CSS gradient's sky/grass split

    SCENERY_LAYOUT.forEach((item) => {
      const basePixel = item.type === "tree" ? 7 : 6;
      const pixelSize = basePixel * item.scale;
      const grid = item.type === "tree" ? TREE : SHRUB;
      const gridW = grid[0].length;
      const gridH = grid.length;
      const totalW = gridW * pixelSize;
      const totalH = gridH * pixelSize;
      const x = w * item.xPercent - totalW / 2;
      const sinkIntoGrass = pixelSize * 1.5;
      const y = grassY + sinkIntoGrass - totalH;
      drawPixelGrid(sceneryCtx, grid, PLANT_COLORS, x, y, pixelSize);
    });
  }

  drawScenery();
  let resizeTimer = null;
  window.addEventListener("resize", () => {
    clearTimeout(resizeTimer);
    resizeTimer = setTimeout(() => {
      drawScenery();
      layoutSky();
    }, 120);
  });

  /* ---------------------------------------------------------
     BUTTERFLIES
  --------------------------------------------------------- */

  const BUTTERFLY_COLORS = {
    W: "#f2a541", // wing
    A: "#e0722a", // wing accent
    B: "#3a2a20"  // body
  };

  const WING_UP = [
    "W.B.W",
    ".WBW.",
    "..B..",
    ".ABA.",
    "A.B.A"
  ];

  const WING_DOWN = [
    ".....",
    "WWBWW",
    ".WBW.",
    "AABAA",
    "....."
  ];

  const BUTTERFLY_PIXEL = 4;
  const butterflies = [];
  const MAX_BUTTERFLIES = 2;

  function spawnButterfly() {
    if (butterflies.length >= MAX_BUTTERFLIES) return;

    const canvas = document.createElement("canvas");
    canvas.className = "butterfly-canvas";
    const gridW = WING_UP[0].length;
    const gridH = WING_UP.length;
    canvas.width = gridW * BUTTERFLY_PIXEL;
    canvas.height = gridH * BUTTERFLY_PIXEL;
    document.body.appendChild(canvas);
    const ctx = canvas.getContext("2d");

    const dir = Math.random() < 0.5 ? 1 : -1; // left-to-right or right-to-left
    const baseY = window.innerHeight * (0.12 + Math.random() * 0.32);
    const amplitude = 18 + Math.random() * 22;
    const duration = 11000 + Math.random() * 6000;
    const startTime = performance.now();
    const wobbleFreq = 2.5 + Math.random() * 1.5;

    butterflies.push({ canvas, ctx, dir, baseY, amplitude, duration, startTime, wobbleFreq, gridW, gridH });
  }

  function updateButterflies(now) {
    for (let i = butterflies.length - 1; i >= 0; i--) {
      const b = butterflies[i];
      const elapsed = now - b.startTime;
      const progress = elapsed / b.duration;

      if (progress >= 1) {
        b.canvas.remove();
        butterflies.splice(i, 1);
        continue;
      }

      const w = window.innerWidth;
      const spanStart = -40;
      const spanEnd = w + 40;
      const travel = b.dir === 1
        ? spanStart + progress * (spanEnd - spanStart)
        : spanEnd - progress * (spanEnd - spanStart);

      const y = b.baseY + Math.sin(progress * Math.PI * 2 * b.wobbleFreq) * b.amplitude;

      const flapFrame = Math.floor(elapsed / 110) % 2 === 0 ? WING_UP : WING_DOWN;
      b.ctx.clearRect(0, 0, b.canvas.width, b.canvas.height);
      b.ctx.save();
      if (b.dir === -1) {
        b.ctx.translate(b.canvas.width, 0);
        b.ctx.scale(-1, 1);
      }
      drawPixelGrid(b.ctx, flapFrame, BUTTERFLY_COLORS, 0, 0, BUTTERFLY_PIXEL);
      b.ctx.restore();

      b.canvas.style.left = travel + "px";
      b.canvas.style.top = y + "px";
    }
  }

  let lastSpawnCheck = 0;
  let nextSpawnDelay = 1500 + Math.random() * 2500;

  function sceneryTick(now) {
    drawSky(now);
    updateButterflies(now);

    if (now - lastSpawnCheck > nextSpawnDelay) {
      lastSpawnCheck = now;
      nextSpawnDelay = 4000 + Math.random() * 5000;
      spawnButterfly();
    }

    requestAnimationFrame(sceneryTick);
  }

  // Seed one butterfly shortly after load so the park feels alive right away.
  setTimeout(spawnButterfly, 800);
  requestAnimationFrame(sceneryTick);
})();
</script>

<script>
(function () {
  "use strict";

  /* ---------------------------------------------------------
     AUTONOMOUS CATS
     A handful of extra cats that wander the park on their own,
     each independently picking a spot to walk to and then
     sitting, sleeping, or playing for a while before moving on.
  --------------------------------------------------------- */

  const NUM_EXTRA_CATS = 3;
  const PIXEL = 4.5;
  const PAD = 10;

  const SIT = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    "DK.....KFFWWWWFFK.",
    "KD.....KFFWWWWFFK.",
    "KDDDDDDDKKFFFFKK..",
    ".KKKKKKK.........."
  ];

  const WALK_A = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    ".......KF......FK.",
    "........K.FFFF.K..",
    ".........K....K..."
  ];

  const WALK_B = [
    "........K......K..",
    ".......KKK....KKK.",
    ".......KPK....KPK.",
    "........KKKKKKKK..",
    ".......KFDFFFFDFK.",
    "......KFDFFDFFDFFK",
    "......KFDFFDFFDFFK",
    "......KFFFFPPFFFFK",
    ".......KFDFFFFDFK.",
    ".......KFFWWWWFFK.",
    "........K......K..",
    ".........K....K..."
  ];

  const GRID_W = 18;
  const GRID_H = 13;
  const CAT_W = GRID_W * PIXEL;
  const CAT_H = GRID_H * PIXEL;

  const BASE_COLORS = { K: "#4a2f2c", W: "#fdf6f0", P: "#f4b6c8" };
  const FUR_VARIANTS = [
    { F: "#b9c9d6", D: "#8fa3b3" }, // grey-blue
    { F: "#e0c9a6", D: "#c2a373" }, // tan/orange
    { F: "#3f3f3f", D: "#242424" }, // charcoal black
    { F: "#e8e2d8", D: "#c7bfae" }  // cream
  ];

  function drawCatFrame(ctx, canvas, rows, flip, colors) {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    ctx.save();
    if (flip === -1) {
      ctx.translate(canvas.width, 0);
      ctx.scale(-1, 1);
    }
    for (let r = 0; r < rows.length; r++) {
      const row = rows[r];
      for (let c = 0; c < row.length; c++) {
        const color = colors[row[c]];
        if (color) {
          ctx.fillStyle = color;
          ctx.fillRect(PAD + c * PIXEL, PAD + r * PIXEL, PIXEL, PIXEL);
        }
      }
    }
    ctx.restore();
  }

  function randRange(a, b) { return a + Math.random() * (b - a); }

  function createAutoCat(index) {
    const canvas = document.createElement("canvas");
    canvas.className = "autoCatCanvas";
    canvas.width = CAT_W + PAD * 2;
    canvas.height = CAT_H + PAD * 2;
    document.body.appendChild(canvas);
    const ctx = canvas.getContext("2d");

    const shadow = document.createElement("div");
    shadow.className = "autoCatShadow";
    document.body.appendChild(shadow);

    const colors = Object.assign({}, BASE_COLORS, FUR_VARIANTS[index % FUR_VARIANTS.length]);

    const pos = {
      x: randRange(20, Math.max(21, window.innerWidth - CAT_W - 20)),
      y: window.innerHeight * randRange(0.6, 0.9)
    };
    let facing = Math.random() < 0.5 ? 1 : -1;
    let state = "sit";
    const target = { x: pos.x, y: pos.y };
    let stateUntil = performance.now() + randRange(1000, 3000);
    const bobSeed = Math.random() * 1000;
    const speed = 0.02 + Math.random() * 0.015;

    function pickNewTarget() {
      target.x = randRange(20, Math.max(21, window.innerWidth - CAT_W - 20));
      target.y = window.innerHeight * randRange(0.58, 0.92);
    }

    function pickIdleAction() {
      const roll = Math.random();
      if (roll < 0.4) return "sit";
      if (roll < 0.7) return "sleep";
      return "play";
    }

    function update(now) {
      if (state === "walk") {
        const dx = target.x - pos.x;
        const dy = target.y - pos.y;
        const dist = Math.hypot(dx, dy);
        if (dist < 6) {
          state = pickIdleAction();
          stateUntil = now + randRange(2500, 6000);
        } else {
          pos.x += dx * speed;
          pos.y += dy * speed;
          if (Math.abs(dx) > 2) facing = dx < 0 ? -1 : 1;
        }
      } else if (now > stateUntil) {
        pickNewTarget();
        state = "walk";
      }

      let frame = SIT;
      let bob = 0;
      if (state === "walk") {
        frame = Math.floor(now / 200) % 2 === 0 ? WALK_A : WALK_B;
      } else if (state === "sleep") {
        bob = Math.sin((now + bobSeed) / 320) * 1.6; // breathing bob
      } else if (state === "play") {
        frame = Math.floor(now / 170) % 2 === 0 ? WALK_A : WALK_B;
        bob = Math.abs(Math.sin((now + bobSeed) / 150)) * -2.4; // playful bounce
      }

      drawCatFrame(ctx, canvas, frame, facing, colors);
      canvas.style.left = (pos.x - PAD) + "px";
      canvas.style.top = (pos.y - PAD + bob) + "px";
      shadow.style.left = (pos.x + CAT_W / 2 - 24) + "px";
      shadow.style.top = (pos.y + CAT_H - 5) + "px";
      shadow.style.opacity = state === "sleep" ? "0.4" : "0.65";
    }

    return { update };
  }

  const autoCats = [];
  for (let i = 0; i < NUM_EXTRA_CATS; i++) autoCats.push(createAutoCat(i));

  function autoCatsTick(now) {
    autoCats.forEach((cat) => cat.update(now));
    requestAnimationFrame(autoCatsTick);
  }
  requestAnimationFrame(autoCatsTick);
})();
</script>
</body>
</html>
