<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Para ti, Tete ❤</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>

<canvas id="hearts-canvas"></canvas>

<!-- HERO -->
<div class="hero">
  <p class="label fade-up">Para siempre contigo</p>
  <h1 class="fade-up delay-1">Tete ❤</h1>
  <p class="date fade-up delay-2">Juntos desde el 28 de agosto de 2024</p>
  <p class="counter fade-up delay-3" id="counter">Calculando...</p>
  <p class="scroll-hint">&#8595; sigue leyendo</p>
</div>

<!-- POEMA -->
<section>
  <h2>Un poema para ti</h2>
  <div class="poem">
    <p>
      Desde aquel veintiocho de agosto<br>
      que cambió todo para mí,<br>
      cada día a tu lado es un agosto<br>
      que no quiero que acabe aquí.
    </p>
    <p>
      Tu risa es mi canción favorita,<br>
      tu mirada mi lugar seguro,<br>
      contigo el tiempo se limita<br>
      a un presente que quiero futuro.
    </p>
    <p>
      Tete, eres mi calma en la tormenta,<br>
      mi sol cuando todo es gris,<br>
      la historia más bonita que se cuenta,<br>
      la razón de mi sonreír.
    </p>
    <p>
      No busco palabras perfectas,<br>
      solo quiero que sepas bien<br>
      que entre todas las vidas inciertas,<br>
      elegiría la tuya otra vez.
    </p>
    <p class="firma">— Tuya, siempre ❤</p>
  </div>
</section>

<!-- CARRUSEL -->
<section>
  <h2>Nosotros</h2>
  <div class="carousel-wrap">
    <button class="c-btn prev" onclick="move(-1)">&#8592;</button>
    <div class="carousel" id="carousel">
      <!-- Pon tus fotos en la carpeta images/ con los nombres foto1.jpg, foto2.jpg... -->
      <div class="slide active"><img src="images/foto1.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto1.jpg<br>en la carpeta images/</div>'" alt="Foto 1"></div>
      <div class="slide"><img src="images/foto2.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto2.jpg<br>en la carpeta images/</div>'" alt="Foto 2"></div>
      <div class="slide"><img src="images/foto3.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto3.jpg<br>en la carpeta images/</div>'" alt="Foto 3"></div>
      <div class="slide"><img src="images/foto4.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto4.jpg<br>en la carpeta images/</div>'" alt="Foto 4"></div>
      <div class="slide"><img src="images/foto5.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto5.jpg<br>en la carpeta images/</div>'" alt="Foto 5"></div>
      <div class="slide"><img src="images/foto6.jpg" onerror="this.parentElement.innerHTML='<div class=\'placeholder\'><span>📷</span>Añade foto6.jpg<br>en la carpeta images/</div>'" alt="Foto 6"></div>
    </div>
    <button class="c-btn next" onclick="move(1)">&#8594;</button>
  </div>
  <div class="dots" id="dots"></div>
</section>

<footer>Hecho con todo mi amor &nbsp;❤&nbsp; para Jose Luis</footer>

<script>
  // ── CONTADOR ──
  (function () {
    const start = new Date('2024-08-28T00:00:00');
    function update() {
      const now = new Date();
      const diff = now - start;
      const days  = Math.floor(diff / 864e5);
      const hours = Math.floor((diff % 864e5) / 36e5);
      const mins  = Math.floor((diff % 36e5)  / 6e4);
      const secs  = Math.floor((diff % 6e4)   / 1e3);
      document.getElementById('counter').textContent =
        `${days} días, ${hours}h ${mins}m ${secs}s juntos`;
    }
    update();
    setInterval(update, 1000);
  })();

  // ── CARRUSEL ──
  const slides = document.querySelectorAll('.slide');
  const dotsEl = document.getElementById('dots');
  let cur = 0, timer;

  slides.forEach((_, i) => {
    const d = document.createElement('span');
    d.className = 'dot' + (i === 0 ? ' active' : '');
    d.onclick = () => go(i);
    dotsEl.appendChild(d);
  });

  function go(n) {
    slides[cur].classList.remove('active');
    dotsEl.children[cur].classList.remove('active');
    cur = (n + slides.length) % slides.length;
    slides[cur].classList.add('active');
    dotsEl.children[cur].classList.add('active');
    resetTimer();
  }

  function move(dir) { go(cur + dir); }

  function resetTimer() {
    clearInterval(timer);
    timer = setInterval(() => move(1), 4000);
  }

  resetTimer();

  // ── SWIPE TÁCTIL ──
  let touchStartX = 0;
  document.getElementById('carousel').addEventListener('touchstart', e => {
    touchStartX = e.touches[0].clientX;
  }, { passive: true });
  document.getElementById('carousel').addEventListener('touchend', e => {
    const diff = touchStartX - e.changedTouches[0].clientX;
    if (Math.abs(diff) > 40) move(diff > 0 ? 1 : -1);
  }, { passive: true });

  // ── CORAZONES ──
  const canvas = document.getElementById('hearts-canvas');
  const ctx = canvas.getContext('2d');
  let hearts = [];

  function resize() {
    canvas.width  = window.innerWidth;
    canvas.height = window.innerHeight;
  }
  resize();
  window.addEventListener('resize', resize);

  function Heart() {
    this.reset();
  }
  Heart.prototype.reset = function () {
    this.x    = Math.random() * canvas.width;
    this.y    = canvas.height + 20;
    this.size = 8 + Math.random() * 14;
    this.speed= .4 + Math.random() * .8;
    this.alpha= .15 + Math.random() * .35;
    this.drift= (Math.random() - .5) * .4;
    this.sway = 0;
    this.swaySpeed = .01 + Math.random() * .02;
  };
  Heart.prototype.update = function () {
    this.sway += this.swaySpeed;
    this.x += Math.sin(this.sway) * this.drift * 2;
    this.y -= this.speed;
    if (this.y < -20) this.reset();
  };
  Heart.prototype.draw = function () {
    ctx.save();
    ctx.globalAlpha = this.alpha;
    ctx.fillStyle   = '#d966a0';
    ctx.translate(this.x, this.y);
    ctx.scale(this.size / 10, this.size / 10);
    ctx.beginPath();
    ctx.moveTo(0, -3);
    ctx.bezierCurveTo(-5, -8, -10, -3, 0,  4);
    ctx.bezierCurveTo( 10, -3,  5, -8, 0, -3);
    ctx.fill();
    ctx.restore();
  };

  for (let i = 0; i < 40; i++) {
    const h = new Heart();
    h.y = Math.random() * canvas.height; // esparcidos al inicio
    hearts.push(h);
  }

  function loop() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    hearts.forEach(h => { h.update(); h.draw(); });
    requestAnimationFrame(loop);
  }
  loop();
</script>
</body>
</html>
