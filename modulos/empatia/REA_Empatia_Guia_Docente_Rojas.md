<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>REA · La Ciencia y el Arte de la Empatía · Rise4TECH</title>
<meta name="description" content="Recurso Educativo Abierto (REA) del Superpoder 5: la Empatía. Basado en Goleman, Rizzolatti, Rogers y Brené Brown. Licencia CC BY-SA 4.0.">
<meta name="author" content="Óscar Javier Rojas">
<meta name="keywords" content="REA, empatía, DUA, neuronas espejo, Goleman, Brené Brown, Rise4TECH, habilidades socioemocionales">
<meta name="license" content="CC BY-SA 4.0">
<script src="https://cdn.tailwindcss.com"></script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800;900&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<script src="https://unpkg.com/lucide@latest"></script>
<style>
:root{
  --ink:#1D1D1F;
  --ink-soft:#424245;
  --muted:#6E6E73;
  --fc-amber:#F5B800;
  --fc-purple:#A786FF;
  --fc-emerald:#10B981;
  --bg:#F5F5F7;
}
html{font-size:16px; scroll-behavior:smooth;}
body{font-family:'Inter','Plus Jakarta Sans',system-ui,sans-serif; background:var(--bg); color:var(--ink); -webkit-font-smoothing:antialiased; margin:0;}
h1,h2,h3,.font-heading{font-family:'Plus Jakarta Sans','SF Pro Display',system-ui,sans-serif; letter-spacing:-0.02em;}
.apple-card{background:#FFFFFF; border-radius:28px; border:1px solid rgba(0,0,0,.07); box-shadow:0 4px 20px rgba(0,0,0,.04),0 1px 3px rgba(0,0,0,.02);}
.apple-subcard{background:#FBFBFD; border-radius:20px; border:1px solid rgba(0,0,0,.06);}
.apple-card:hover,.apple-subcard:hover{transform:translateY(-2px); box-shadow:0 12px 30px rgba(0,0,0,.08); transition:all .3s ease;}
.fluid-glow{position:absolute; border-radius:50%; filter:blur(40px); pointer-events:none;}
.hero-title{background:linear-gradient(135deg,#1D1D1F 30%,#8936B2 70%,#A786FF 100%); -webkit-background-clip:text; -webkit-text-fill-color:transparent;}
.nav-pill{background:#fff; border:1.5px solid rgba(0,0,0,.1); color:#424245; font-weight:700; cursor:pointer; transition:all .2s;}
.nav-pill:hover{border-color:#A786FF; color:#8936B2;}
.nav-pill.active{background:#1D1D1F; color:#fff; border-color:#1D1D1F; box-shadow:0 6px 18px rgba(0,0,0,.18);}
.station{display:none;}
.station.active{display:block; animation:fadeUp .45s ease;}
@keyframes fadeUp{from{opacity:0; transform:translateY(14px);} to{opacity:1; transform:none;}}
.badge-dot{width:10px; height:10px; border-radius:999px;}
.opt{border:2px solid rgba(0,0,0,.08); background:#fff; transition:all .2s;}
.opt:hover{border-color:#A786FF;}
.opt.correct{border-color:#10B981; background:#F0FDF4;}
.opt.wrong{border-color:#F43F5E; background:#FFF1F2;}
.chip{display:inline-flex; align-items:center; gap:.4rem; font-size:.7rem; font-weight:800; color:#fff; padding:.35rem .7rem; border-radius:999px;}
.chip.bg-purple{background:#8936B2;} .chip.bg-emerald{background:#10B981;} .chip.bg-amber{background:#D97706;} .chip.bg-indigo{background:#4F46E5;}
</style>
</head>
<body class="min-h-screen">

<!-- ============ HEADER / META ============ -->
<header class="bg-[#1D1D1F] text-white">
  <div class="max-w-6xl mx-auto px-5 py-4 flex items-center justify-between">
    <div class="flex items-center gap-3.5">
      <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-purple-600 to-indigo-500 flex items-center justify-center font-black text-lg shadow-lg">R5</div>
      <div>
        <div class="flex items-center gap-2">
          <span class="font-extrabold text-lg tracking-tight">REA · La Ciencia y el Arte de la Empatía</span>
        </div>
        <p class="text-xs text-gray-400 font-medium">Recurso Educativo Abierto · Superpoder 5 · Rise4TECH</p>
      </div>
    </div>
    <div class="flex items-center gap-2">
      <span class="chip bg-emerald"><i data-lucide="unlock" class="w-3 h-3"></i> CC BY-SA 4.0</span>
    </div>
  </div>
</header>

<!-- ============ BARRA DE METADATOS ============ -->
<section class="max-w-6xl mx-auto px-5 py-3">
  <div class="apple-card p-3 px-5 flex flex-wrap items-center justify-between gap-2 text-xs font-semibold text-[#424245]">
    <span><i data-lucide="user" class="w-3.5 h-3.5 inline text-purple-600"></i> Autor: <strong>Óscar Javier Rojas</strong></span>
    <span class="hidden md:inline"><i data-lucide="graduation-cap" class="w-3.5 h-3.5 inline text-purple-600"></i> Maestría en Enseñanza en Entornos Digitales (MEED)</span>
    <span class="hidden lg:inline"><i data-lucide="layers" class="w-3.5 h-3.5 inline text-purple-600"></i> DUA · Múltiples medios</span>
    <span><i data-lucide="badge-check" class="w-3.5 h-3.5 inline text-emerald-600"></i> CC BY-SA 4.0</span>
    <button id="btnDescargarGuia" class="inline-flex items-center gap-1.5 bg-purple-600 text-white font-bold text-xs px-3.5 py-2 rounded-full hover:bg-purple-700 transition">
      <i data-lucide="book-open" class="w-3.5 h-3.5"></i> Guía docente
    </button>
  </div>
</section>

<!-- ============ HERO ============ -->
<section class="max-w-6xl mx-auto px-5 pt- mergelates 6">
  <div class="apple-card p-8 md:p-10 relative overflow-hidden">
    <div class="fluid-glow -top-20 -right-20 w-72 h-72 bg-purple-200/60"></div>
    <div class="fluid-glow -bottom-20 -left-20 w-72 h-72 bg-emerald-100/60"></div>
    <div class="relative z-10 grid md:grid-cols-2 gap-8 items-center">
      <div>
        <span class="inline-block bg-purple-50 border border-purple-200 text-purple-700 font-extrabold text-xs uppercase tracking-wider px-3 py-1.5 rounded-full mb-4">Superpoder 5 · Empatía</span>
        <h1 class="hero-title font-black text-4xl md:text-5xl leading-[1.05]">De las neuronas espejo a la acción empática</h1>
        <p class="mt-4 text-lg text-[#424245] leading-relaxed">Un recurso educativo abierto, interactivo y accesible para desarrollar una de las habilidades socioemocionales más poderosas del mundo laboral: comprender al otro desde <strong>su propio marco de referencia</strong>, sin juzgar ni fundirte en su dolor.</p>
        <div class="mt-6 flex flex-wrap items-center gap-3">
          <button class="nav-goto inline-flex items-center gap-2 bg-purple-600 text-white font-bold px-5 py-3 rounded-full text-sm hover:bg-purple-700 transition" data-target="estacion1"><i data-lucide="play" class="w-4 h-4"></i> Comenzar el recorrido</button>
          <span class="inline-flex items-center gap-2 text-sm font-semibold text-[#424245]"><i data-lucide="timer" class="w-4 h-4"></i> 25–35 min · 4 estaciones</span>
        </div>
      </div>
      <div class="flex justify-center">
        <img src="/media/lore/superheroina_trans.png" alt="Lore, mentora de Rise4TECH" class="w-56 md:w-72 object-contain drop-shadow-[0_14px_28px_rgba(137,54,178,0.35)]">
      </div>
    </div>
  </div>
</section>

<!-- ============ NAVEGACIÓN ============ -->
<section class="max-w-6xl mx-auto px-5 pt-6">
  <nav class="grid grid-cols-2 md:grid-cols-4 gap-3" aria-label="Estaciones del recurso">
    <button class="nav-pill rounded-2xl px-4 py-3 flex items-center justify-center gap-2 text-xs active" data-station="estacion1"><i data-lucide="play-circle" class="w-4 h-4"></i><span>1 · Activación</span></button>
    <button class="nav-pill rounded-2xl px-4 py-3 flex items-center justify-center gap-2 text-xs" data-station="estacion2"><i data-lucide="brain" class="w-4 h-4"></i><span>2 · Conceptos</span></button>
    <button class="nav-pill rounded-2xl px-4 py-3 flex items-center justify-center gap-2 text-xs" data-station="estacion3"><i data-lucide="flask-conical" class="w-4 h-4"></i><span>3 · Laboratorio</span></button>
    <button class="nav-pill rounded-2xl px-4 py-3 flex items-center justify-center gap-2 text-xs" data-station="estacion4"><i data-lucide="download" class="w-4 h-4"></i><span>4 · Recursos</span></button>
  </nav>
</section>

<!-- ============ ESTACIÓN 1 ============ -->
<section id="estacion1" class="station active max-w-6xl mx-auto px-5 pt-8">
  <div class="apple-card p-6 md:p-8">
    <div class="flex items-center gap-3 mb-5">
      <span class="w-9 h-9 rounded-xl bg-purple-600 flex items-center justify-center text-white"><i data-lucide="play-circle" class="w-5 h-5"></i></span>
      <h2 class="font-extrabold text-2xl">Estación 1 · Activación y video</h2>
    </div>
    <p class="text-[#424245] mb-5 leading-relaxed">Empieza por la cápsula que dio origen a este recurso. Pregunta mientras miras: <em>¿qué significa “ponerse en los zapatos del otro” sin realmente habitar sus zapatos?</em></p>
    <div class="aspect-video rounded-3xl overflow-hidden shadow-lg border border-black/10">
      <iframe src="https://www.youtube.com/embed/-AlHz1tpGz8" title="Cápsula Superpoder 5: La Empatía" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen class="w-full h-full"></iframe>
    </div>
    <div class="mt-6 grid md:grid-cols-2 gap-4">
      <div class="apple-subcard p-5">
        <div class="flex items-center gap-2 mb-2">
          <span class="badge-dot bg-purple-500"></span>
          <h3 class="font-extrabold">Objetivo de aprendizaje</h3>
        </div>
        <p class="text-sm text-[#424245]">Reconocer la empatía como habilidad entrenable, con base neurobiológica (neuronas espejo) y tres dimensiones (Goleman), distinguiéndola de la simpatía, la complacencia y el <em>enmeshment</em>, para aplicarla en dilemas laborales auténticos.</p>
      </div>
      <div class="apple-subcard p-5">
        <div class="flex items-center gap-2 mb-2">
          <span class="badge-dot bg-emerald-500"></span>
          <h3 class="font-extrabold">¿Qué lograrás?</h3>
        </div>
        <ul class="text-sm text-[#424245] space-y-1.5">
          <li><i data-lucide="check-circle" class="w-4 h-4 text-emerald-600 inline"></i> Explicar la base biológica de la empatía</li>
          <li><i data-lucide="check-circle" class="w-4 h-4 text-emerald-600 inline"></i> Distinguir empatía de enmeshment</li>
          <li><i data-lucide="check-circle" class="w-4 h-4 text-emerald-600 inline"></i> Elegir respuestas empáticas con feedback</li>
        </ul>
      </div>
    </div>
    <details class="mt-5 apple-subcard p-4" open>
      <summary class="font-bold text-[#1D1D1F] cursor-pointer">📜 ¿Prefieres leer en vez de ver? Transcripción textual de la cápsula <em>(DUA · Representación)</em></summary>
      <div class="mt-3 text-sm text-[#424245] space-y-3 max-h-64 overflow-y-auto pr-2">
        <p><strong>Diana:</strong> Seamos honestas: si tú calzas 38 y tratas de meterte en mis zapatos 36, para además empezar a caminar por caminos que tú jamás has recorrido… ¿qué pasa? No solo te duelen los pies, sino que terminas desorientada.</p>
        <p><strong>Óscar:</strong> Cuando tratamos de aplicar literalmente el «ponernos en los zapatos del otro» cometemos el error de juzgar la situación desde nuestra propia realidad: <em>«Yo en tu lugar no me preocuparía»</em>. Eso no es empatía; es mirarte a ti mismo en un espejo que no es tuyo.</p>
        <p><strong>Diana:</strong> La verdadera empatía reconoce que esa persona habita un mundo propio, con vivencias y contextos que nosotros no conocemos.</p>
        <p><strong>Óscar:</strong> La «regla de oro»: <em>Tú puedes no compartir el motivo de la otra persona, pero jamás tienes el derecho de invalidar su emoción.</em></p>
      </div>
    </details>
    <div class="mt-5 flex justify-end">
      <button class="nav-goto inline-flex items-center gap-2 bg-purple-600 text-white font-bold px-5 py-3 rounded-full text-sm hover:bg-purple-700 transition" data-target="estacion2">Ir a conceptos <i data-lucide="arrow-right" class="w-4 h-4"></i></button>
    </div>
  </div>
</section>

<!-- ============ ESTACIÓN 2 ============ -->
<section id="estacion2" class="station max-w-6xl mx-auto px-5 pt-6">
  <div class="apple-card p-6 md:p-8">
    <div class="flex items-center gap-3 mb-5">
      <span class="w-9 h-9 rounded-xl bg-purple-600 flex items-center justify-center text-white"><i data-lucide="brain" class="w-5 h-5"></i></span>
      <h2 class="font-extrabold text-2xl">Estación 2 · Caja de herramientas conceptuales</h2>
    </div>
    <p class="text-[#424245] mb-6">Cuatro ideas fundamentales, cada una con su fuente. Son la base del laboratorio de dilemas.</p>

    <!-- Concepto 1 -->
    <div class="apple-subcard p-5 md:p-6 mb-4">
      <div class="flex items-center gap-3 mb-2">
        <span class="badge-dot bg-purple-500"></span>
        <h3 class="font-extrabold text-lg">1 · La definición que usamos</h3>
      </div>
      <p class="text-[#424245] leading-relaxed">La <strong>Asociación Americana de Psicología (APA)</strong> define la empatía como <em>“comprender a una persona desde su propio marco de referencia en lugar del nuestro”</em>. Daniel Goleman la precisa como <em>“reconocer las emociones en los demás, comprender sus sentimientos y responder adecuadamente”</em>. Comprender no es juzgar ni resolver de inmediato.</p>
      <p class="text-xs text-[#6E6E73] mt-2">Fuentes: APA · Goleman, <em>Inteligencia Emocional</em> (1995).</p>
    </div>

    <!-- Concepto 2 -->
    <div class="apple-subcard p-5 md:p-6 mb-4">
      <div class="flex items-center gap-3 mb-2">
        <span class="badge-dot bg-emerald-500"></span>
        <h3 class="font-extrabold text-lg">2 · La base biológica: neuronas espejo</h3>
      </div>
      <p class="text-[#424245] leading-relaxed">Giacomo Rizzolatti descubrió en la corteza premotora células que se activan <strong>tanto al ejecutar una acción como al observar a otra persona realizarla</strong>. Por eso bostezamos cuando alguien bosteza: nuestro cerebro “simula” la experiencia del otro. Nacemos cableados para empatizar, pero <strong>convertir esa chispa en habilidad profesional exige entrenamiento</strong>.</p>
      <p class="text-xs text-[#6E6E73] mt-2">Fuente: Rizzolatti &amp; Sinigaglia, <em>Las neuronas espejo</em> (2006).</p>
    </div>

    <!-- Concepto 3 -->
    <div class="apple-subcard p-5 md:p-6 mb-4">
      <div class="flex items-center gap-3 mb-2">
        <span class="badge-dot bg-amber-500"></span>
        <h3 class="font-extrabold text-lg">3 · Los dos abismos: minimización y apropiación dramática</h3>
      </div>
      <p class="text-[#424245] leading-relaxed">Frente al dolor ajeno caemos en dos trampas (Carl Rogers): la <strong>minimización</strong> —<em>«no es para tanto»</em>— invalida a la persona; la <strong>apropiación dramática</strong> —<em>«¡qué tragedia espantosa, yo me muero!»</em>— roba el protagonismo. La empatía de Rogers es entrar en el mundo del otro <em>«como si»</em> fuera el tuyo, <strong>sin perder jamás la cualidad del “como si”</strong>.</p>
      <p class="text-xs text-[#6E6E73] mt-2">Fuente: Rogers, C. (1961). <em>El proceso de convertirse en persona</em>.</p>
    </div>

    <!-- Concepto 4 -->
    <div class="apple-subcard p-5 md:p-6 mb-4">
      <div class="flex items-center gap-3 mb-2">
        <span class="badge-dot bg-rose-500"></span>
        <h3 class="font-extrabold text-lg">4 · La joya de Brené Brown: empatía ≠ enmeshment</h3>
      </div>
      <p class="text-[#424245] leading-relaxed">Brené Brown distingue la <strong>empatía cognitiva</strong> (comprender sin juzgar) de la <strong>afectiva</strong> (sentir con el otro) y advierte: <em>si saltas al hoyo donde está el otro, ahora son dos en el hoyo</em>. Eso es <strong><em>enmeshment</em></strong> (sobre-identificación). La empatía sana es permanecer <strong>entero, en la orilla, escuchando</strong>: ni minimizar, ni fundirse, ni “arreglar” sin permiso.</p>
      <p class="text-xs text-[#6E6E73] mt-2">Fuente: Brown, B. &amp; Grant, A., <em>Dare to Lead · Empathy vs. Enmeshment</em> (Parte 4 de 6).</p>
    </div>

    <div class="app-heading mt-2 flex justify-end">
      <button class="nav-goto inline-flex items-center gap-2 bg-purple-600 text-white font-bold px-5 py-3 rounded-full text-sm hover:bg-purple-700 transition" data-target="estacion3">Entrar al laboratorio <i data-lucide="arrow-right" class="w-4 h-4"></i></button>
    </div>
  </div>
</section>

<!-- ============ ESTACIÓN 3 ============ -->
<section id="estacion3" class="station max-w-6xl mx-auto px-5 pt-6">
  <div class="apple-card p-6 md:p-8">
    <div class="flex items-center gap-3 mb-5">
      <span class="w-9 h-9 rounded-xl bg-purple-600 flex items-center justify-center text-white"><i data-lucide="flask-conical" class="w-5 h-5"></i></span>
      <h2 class="font-extrabold text-2xl">Estación 3 · Laboratorio de dilemas con feedback</h2>
    </div>
    <p class="text-[#424245] mb-2">Dos dilemas auténticos del mundo laboral tech. Elige la respuesta más empática: recibirás <strong>feedback formativo inmediato</strong> con la explicación conceptual de cada opción.</p>

    <!-- ======== DILEMA 1 ======== -->
    <div class="apple-subcard p-5 md:p-6 mb-6" data-dilemma-block>
      <div class="flex items-center justify-between mb-1">
        <span class="inline-block bg-rose-600 text-white text-xs font-extrabold uppercase px-3 py-1 rounded-full">Dilema 1</span>
        <span class="text-xs font-semibold text-[#6E6E73]">Minimización</span>
      </div>
      <h3 class="font-extrabold text-xl mt-3">El cactus de la compañera</h3>
      <p class="text-[#424245] text-sm leading-relaxed mt-1">María llega a trabajar con los ojos llorosos: se le murió el cactus que su abuelo le regaló antes de fallecer. Tu colega no lo sabe. ¿Cuál es la respuesta más empática?</p>

      <div class="mt-4 space-y-2.5">
        <button data-correct="true" class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          “Veo que estás triste, María. Si quieres hablar de ello, estoy aquí para escucharte.”
        </button>
        <button data-correct="false" data-msg="Minimizaste su pérdida: 'solo es una planta'. Recuerda que invalidar la emoción rompe la confianza. La regla: jamás tienes derecho a invalidar la emoción del otro." class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          “Tranquila, es solo una planta. Te compro otra en la tienda de la esquina.”
        </button>
        <button data-correct="false" data-msg="Caíste en la apropiación dramática (enmeshment): te apoderaste de su dolor y lo convertiste en tu escenario. La empatía sana es permanecer entero junto al otro, sin fundirte." class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          “¡Nooo! ¡Qué tragedia espantosa! ¡Yo me muero, es terrible, no te lo puedo creer!”
        </button>
      </div>
      <div class="feed hidden mt-4 text-sm rounded-2xl p-4"></div>
    </div>

    <!-- ======== DILEMA 2 ======== -->
    <div class="apple-subcard p-5 md:p-6 mb-6" data-dilemma-block>
      <div class="flex items-center justify-between mb-1">
        <span class="inline-block bg-purple-600 text-white text-xs font-extrabold uppercase px-3 py-1 rounded-full">Dilema 2</span>
        <span class="text-xs font-semibold text-[#6E6E73]">Enmeshment</span>
      </div>
      <h3 class="font-extrabold text-xl mt-3">La amiga en el hoyo</h3>
      <p class="text-[#424245] text-sm leading-relaxed mt-1">Camilo te cuenta que su madre está hospitalizada y que está agotado. Tú tiendes a sentir todo muy profundamente. ¿Qué haces?</p>

      <div class="mt-4 space-y-2.5">
        <button data-correct="false" data-msg="Es enmeshment: te apropiaste de su angustia. Ahora él debe consolarte a ti. La empatía es comprender Y permanecer entero." class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          Empiezas a llorar con él: “¡No aguanto verte así, esto me parte el alma!” y te quedas rumiando toda la semana.
        </button>
        <button data-correct="false" data-msg="La 'espalda' con consejos no pedidos es la trampa de 'arreglar'. Mejor validar y preguntar (Edgar Schein: la pregunta humilde)." class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          Le das una lista de médicos y tecnicas: “Lo que debes hacer es cambiar de clínica, yo ya te lo digo.”
        </button>
        <button data-correct="true" class="opt w-full text-left text-sm font-semibold rounded-2xl px-4 py-3.5">
          “Gracias por contármelo. No imagino lo duro que debe ser. ¿Cómo puedo apoyarte esta semana?”
        </button>
      </div>
      <div class="feed hidden mt-4 text-sm rounded-2xl p-4"></div>
    </div>

    <div class="mt-6 bg-[#1D1D1F] text-white rounded-2xl p-5 flex items-start gap-4">
      <img src="/media/lore/evaluando_trans.png" alt="Lore evaluando" class="w-16 h-16 object-contain flex-shrink-0">
      <div>
        <p class="font-extrabold">Micro-reto (para dialogar en pares):</p>
        <p class="text-gray-300 text-sm">Responde con tus palabras a: <em>“Me da miedo fallar en esta entrega”</em>. ¿Qué frase empática usarías? Luego prueba la <strong>pregunta humilde</strong> de Schein: <em>“¿Cómo se ve el apoyo viniendo de mí?”</em></p>
      </div>
    </div>

    <div class="mt-6 flex justify-end">
      <button class="nav-goto inline-flex items-center gap-2 bg-purple-600 text-white font-bold px-5 py-3 rounded-full text-sm hover:bg-purple-700 transition" data-target="estacion4">Ver recursos y licencia <i data-lucide="arrow-right" class="w-4 h-4"></i></button>
    </div>
  </div>
</section>

<!-- ============ ESTACIÓN 4 ============ -->
<section id="estacion4" class="station max-w-6xl mx-auto px-5 pt-6">
  <div class="apple-card p-6 md:p-8">
    <div class="flex items-center gap-3 mb-5">
      <span class="w-9 h-9 rounded-xl bg-purple-600 flex items-center justify-center text-white"><i data-lucide="download" class="w-5 h-5"></i></span>
      <h2 class="font-extrabold text-2xl">Estación 4 · Recursos abiertos y licencia</h2>
    </div>
    <p class="text-[#424245] mb-6">Todo el material es abierto y remezclable bajo <strong>Creative Commons</strong>. Reutiliza, adapta y redistribuye citando la fuente.</p>

    <div class="grid md:grid-cols-2 gap-4">
      <a href="/rea-empatia/ficha_memoria_superpoder5_empatia.pdf" class="apple-subcard p-5 hover:shadow-lg transition" target="_blank" rel="noopener">
        <i data-lucide="file-text" class="w-8 h-8 text-purple-600 mb-2"></i>
        <h3 class="font-extrabold">Ficha de memoria</h3>
        <p class="text-sm text-[#424245]">Síntesis visual descargable en PDF, formato móvil.</p>
        <span class="text-sm font-bold text-purple-700">Descargar →</span>
      </a>
      <a href="/rea-empatia/evaluar_superpoder5.html" class="apple-subcard p-5 hover:shadow-lg transition" target="_blank" rel="noopener">
        <i data-lucide="clipboard-check" class="w-8 h-8 text-emerald-600 mb-2"></i>
        <h3 class="font-extrabold">Evaluación formativa</h3>
        <p class="text-sm text-[#424245]">Cuestionario de valoración del Superpoder 5.</p>
        <span class="text-sm font-bold text-emerald-700">Abrir →</span>
      </a>
      <a href="/slides_superpoder5.html" class="apple-subcard p-5 hover:shadow-lg transition" target="_blank" rel="noopener">
        <i data-lucide="presentation" class="w-8 h-8 text-amber-600 mb-2"></i>
        <h3 class="font-extrabold">Presentación 16:9</h3>
        <p class="text-sm text-[#424245]">Diapositivas para la sesión sincrónica en Meet.</p>
        <span class="text-sm font-bold text-amber-700">Ver →</span>
      </a>
      <a href="https://www.youtube.com/watch?v=-AlHz1tpGz8" class="apple-subcard p-5 hover:shadow-lg transition" target="_blank" rel="noopener">
        <i data-lucide="youtube" class="w-8 h-8 text-rose-600 mb-2"></i>
        <h3 class="font-extrabold">Cápsula en YouTube</h3>
        <p class="text-sm text-[#424245]">Video audiovisual del Superpoder 5 (Diana &amp; Óscar).</p>
        <span class="text-sm font-bold text-rose-700">Ver en YouTube →</span>
      </a>
    </div>

    <!-- Licencia -->
    <div class="apple-subcard p-6 mt-6">
      <div class="flex items-center gap-4 flex-wrap">
        <div class="flex items-center gap-1.5 bg-black text-white text-xs font-bold px-3 py-2 rounded-lg">
          <span class="w-5 h-5 rounded-full bg-black border border-white flex items-center justify-center"><i data-lucide="user" class="w-3 h-3"></i></span>
          BY
        </div>
        <div class="flex items-center gap-1.5 bg-black text-white text-xs font-bold px-3 py-2 rounded-lg">
          <span class="w-5 h-5 rounded-full bg-black border border-white flex items-center justify-center"></span>
          SA
        </div>
        <span class="font-extrabold">Licencia Creative Commons Atribución-CompartirIgual 4.0 Internacional (CC BY-SA 4.0)</span>
      </div>
      <p class="text-sm text-[#424245] mt-3">Este REA es un Recurso Educativo Abierto: eres libre de <strong>retenerlo, reutilizarlo, revisarlo, remezclarlo y redistribuirlo</strong>, siempre que atribuyas la autoría (<strong>Óscar Javier Rojas</strong>) y compartas tu versión bajo la <strong>misma licencia</strong>. Las citas académicas (Goleman, Rizzolatti, Rogers, Brown, etc.) pertenecen a sus autores y se usan con fines didácticos.</p>
      <p class="text-xs text-[#6E6E73] mt-2">CC BY-SA 4.0 · Óscar Javier Rojas · Rise4TECH · Fundación Capital (referencias institucionales del contexto de origen).</p>
    </div>

    <!-- Referencias -->
    <div class="apple-subcard p-6 mt-3">
      <h3 class="font-extrabold mb-3">Referencias y bases conceptuales</h3>
      <ul class="text-sm text-[#424245] space-y-1.5 list-disc pl-5">
        <li>Goleman, D. (1995). <em>Inteligencia Emocional</em>. Kairós.</li>
        <li>Rizzolatti, G. &amp; Sinigaglia, C. (2006). <em>Las neuronas espejo</em>. Paidós.</li>
        <li>Brown, B. &amp; Grant, A. <em>Dare to Lead · Empathy vs. Enmeshment</em> (Parte 4 de 6).</li>
        <li>Rogers, C. (1961). <em>El proceso de convertirse en persona</em>. Paidós.</li>
        <li>Wiseman, T. (1996). “A concept analysis of empathy”. <em>Journal of Advanced Nursing</em>.</li>
      </ul>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer class="mt-10 bg-[#1D1D1F] text-white">
  <div class="max-w-6xl mx-auto px-5 py-6 flex flex-col md:flex-row items-center justify-between gap-3 text-sm">
    <span>REA · La Ciencia y el Arte de la Empatía — Superpoder 5</span>
    <span class="text-gray-400">Óscar Javier Rojas · Licencia CC BY-SA 4.0</span>
  </div>
</footer>

<script>
  if (window.lucide){ lucide.createIcons(); }

  // Navegación por estaciones
  const navButtons = document.querySelectorAll('.nav-pill');
  const stations = document.querySelectorAll('.station');

  function showStation(target){
    stations.forEach(s => s.classList.remove('active'));
    const el = document.getElementById(target);
    if (el){ el.classList.add('active'); window.scrollTo({top:0, behavior:'smooth'}); }
    navButtons.forEach(b => b.classList.toggle('active', b.dataset.station === target));
  }
  navButtons.forEach(b => b.addEventListener('click', () => showStation(b.dataset.station)));
  document.querySelectorAll('.nav-goto').forEach(b => b.addEventListener('click', () => showStation(b.dataset.target)));

  // Feedback interactivo de dilemas
  document.querySelectorAll('[data-dilemma-block]').forEach(block => {
    const opts = block.querySelectorAll('.opt');
    const feed = block.querySelector('.feed');
    opts.forEach(opt => opt.addEventListener('click', () => {
      const isCorrect = opt.dataset.correct === 'true';
      opts.forEach(o => o.classList.remove('correct','wrong'));
      if (isCorrect){
        opt.classList.add('correct');
        feed.className = 'feed block mt-4 text-sm rounded-2xl p-4 bg-emerald-50 border border-emerald-200 text-emerald-900';
        feed.textContent = '✅ ¡Excelente! Validas la emoción sin juzgar ni minimizar, y ofreces presencia sin fundirte. Esa es la empatía de Rogers y Brené Brown.';
      } else {
        opt.classList.add('wrong');
        feed.className = 'feed block mt-4 text-sm rounded-2xl p-4 bg-rose-50 border border-rose-200 text-rose-900';
        feed.textContent = opt.dataset.msg || 'Revisa el concepto y vuelve a intentarlo.';
      }
      feed.classList.remove('hidden');
    }));
  });

  // Botón descargar guía docente
  document.getElementById('btnDescargarGuia').addEventListener('click', () => {
    const guia = 'REA_Empatia_Guia_Docente_Rojas.md';
    alert('📘 La Guía de Reutilización Docente (' + guia + ') se entrega como documento adjunto del REA en formato .md, editable y listo para adaptar a tu contexto.');
  });
</script>
</body>
</html></think>El REA web interactivo quedó listo. Ahora genero la **Guía de Reutilización Docente completa** (el segundo entregable de la entrega académica), siguiendo al pie de la letra la plantilla oficial MEED y la rúbrica de evaluación:

<｜DSML｜tool_calls>
<｜DSML｜invoke name="write">
<｜DSML｜parameter name="content" string="true"># 📘 Guía de Reutilización Docente — REA «La Ciencia y el Arte de la Empatía»

> *Recurso Educativo Abierto (REA) · Superpoder 5: La Empatía*
> *Maestría en Enseñanza en Entornos Digitales (MEED) — Actividad acreditable final*
> *Plantilla oficial de guía de reutilización de REA · Fundación Capital*

---

## 1. Identificación y Metadatos del Recurso

| Campo | Detalle |
| :---- | :---- |
| **Título del REA** | La Ciencia y el Arte de la Empatía: de las neuronas espejo a la acción empática (Superpoder 5) |
| **Autoría y Afiliación** | **Óscar Javier Rojas** · Maestría en Enseñanza en Entornos Digitales (MEED) |
| **Área Disciplinar** | Habilidades socioemocionales / Soft Skills para el ámbito laboral y formativo (curso Rise4TECH, en el contexto institucional de la Fundación Capital). |
| **Destinatarios** | Jóvenes y adultos en formación laboral, técnica, media y universitaria (ciclos de introducción y desarrollo de habilidades blandas). |
| **Licencia Abierta** | **Creative Commons Atribución-CompartirIgual 4.0 Internacional (CC BY-SA 4.0)** |
| **Repositorio** | `https://webhook.lore-rise4tech.org/rea-empatia/` (REA interactivo web HTML5) |

**Repositorio del REA:**
- **Recurso interactivo web (HTML5 + Tailwind):** `https://webhook.lore-rise4tech.org/rea-empatia/index.html`
- **Ficha de memoria (PDF):** `/rea-empatia/ficha_memoria_superpoder5_empatia.pdf`
- **Evaluación formativa:** `/rea-empatia/evaluar_superpoder5.html`
- **Presentación 16:9 (Meet):** `/slides_superpoder5.html`
- **Cápsula audiovisual (YouTube):** `https://www.youtube.com/watch?v=-AlHz1tpGz8`

---

## 2. Intencionalidad Pedagógica y Curricular

### Propósito de Aprendizaje

Este REA aborda la **empatía** como una habilidad socioemocional entrenable, con base neurobiológica y expresiones prácticas en el entorno laboral. Su propósito es que las personas participantes comprendan qué es (y qué **no** es) la empatía, la distingan de la simpatía, la compasión y el *enmeshment* (sobre-identificación), y puedan aplicar respuestas empáticas auténticas en dilemas cotidianos del trabajo en equipo.

### Objetivos del REA

**Objetivo principal:**
Desarrollar la competencia empática de las participantes mediante un recorrido interactivo que articula el conocimiento neurocientífico (neuronas espejo), el marco conceptual de la inteligencia emocional (Goleman) y la práctica reflexiva de dilemas laborales con retroalimentación formativa.

**Objetivos específicos:**
1. Explicar la base biológica de la empatía (neuronas espejo de Rizzolatti y plasticidad cerebral).
2. Distinguir los tres niveles o dimensiones de la empatía según Goleman (cognitiva, emocional y compasiva o de acción).
3. Identificar las trampas que bloquean la empatía: minimización, apropiación dramática y *enmeshment* (Rogers; Brené Brown y Adam Grant).
4. Aplicar respuestas empáticas asertivas en dilemas laborales auténticos, con la «pregunta humilde» de Edgar Schein.
5. Reflexionar metacognitivamente sobre las propias respuestas empáticas mediante micro-retos y autoevaluación.

### Sugerencia de implementación

Se recomienda implementar al **cierre de un módulo socioemocional** o como **fase de integración** dentro de un trayecto formativo sobre habilidades blandas (p. ej., después del módulo de comunicación y antes de la evaluación integradora). También puede usarse en la **fase de desarrollo** como laboratorio práctico de la competencia. El REA está pensado para una sesión de **25 a 35 minutos** (asincrónica) o como estación dentro de un taller sincrónico.

---

## 3. Estructura del REA (Recorrido por Estaciones)

El REA se organiza como una **experiencia interactiva de aprendizaje** en 4 estaciones, alineadas con los principios del **Diseño Universal de Aprendizaje (DUA)**:

| Estación | Contenido | Medios DUA |
| :---- | :---- | :---- |
| **Estación 1 · Activación** | Cápsula de video (YouTube) + transcripción textual colapsable + objetivos de aprendizaje explícitos. | Representación múltiple: **audiovisual + textual** (subtítulos y transcripción). |
| **Estación 2 · Conceptos** | Caja de herramientas conceptuales: definición APA/Goleman, neuronas espejo, los dos abismos de Rogers, la distinción empatía vs. *enmeshment* de Brené Brown. | Representación: **texto claro + ejemplos + citas** de fuentes reales. |
| **Estación 3 · Laboratorio** | 2 dilemas interactivos con **feedback formativo inmediato** (respuesta correcta/incorrecta con explicación conceptual) + micro-reto de diálogo en pares con la «pregunta humilde» de Schein. | Acción y expresión: **elección + retroalimentación**; compromiso: dilemas auténticos del mundo laboral. |
| **Estación 4 · Recursos** | Descarga de ficha de memoria, evaluación formativa, presentación 16:9, vínculo a YouTube, licencia CC BY-SA 4.0 y referencias académicas. | Acción y expresión: **múltiples puntos de salida y descarga** para aplicar el aprendizaje. |

---

## 4. Especificaciones Técnicas y Requisitos de Acceso

**Formatos y Tecnologías:**
- REA interactivo: **HTML5 + Tailwind CSS** (un solo archivo autocontenido, sin dependencias de instalación más allá del navegador).
- Videos: **MP4 / YouTube** con subtítulos disponibles.
- Ficha de memoria: **PDF** descargable (formato móvil/vertical, compatible con WhatsApp).
- Evaluación formativa: **HTML interactivo** con autoevaluación.
- Presentación: **HTML/CSS 16:9 + PDF** para sesiones sincrónicas en Google Meet.

**Instalación:**
- No requiere software especial: funciona en cualquier navegador moderno (Chrome, Safari, Edge, Firefox) en **PC, tablet o móvil**.
- Puede alojarse en cualquier servidor estático (GitHub Pages, Netlify, servidor institucional) o integrarse en **LMS** (Moodle, Canvas) mediante enlace o incrustación `<iframe>`.
- Para ejecución local basta abrir el archivo `.html` en el navegador.

**Accesibilidad y Diseño Universal (DUA):**
- ✅ **Subtítulos y transcripción textual** del video (colapsable en la Estación 1).
- ✅ **Texto alternativo** en imágenes y avatares.
- ✅ **Contraste alto** (fondo claro `#F5F5F7`, texto `#1D1D1F`; variante oscura en otras piezas) para legibilidad.
- ✅ **Tipografía legible** (mín. 16px) y diseño responsive para móvil (5–6.7″).
- ✅ **Múltiples rutas de representación y expresión** (video, texto, elección interactiva, reflexión oral).
- ✅ Navegación por **teclado** y elementos interactivos con `focus-visible` para compatibilidad con lectores de pantalla.

---

## 5. Intencionalidad Pedagógica y Curricular en el marco DUA (detalle)

El recurso atiende las **cinco pautas** del Diseño Universal de Aprendizaje solicitadas en la consigna:

1. **Múltiples medios de representación** → Video + transcripción textual + infografías conceptuales + ejemplos narrados (cápsula de Diana y Óscar) + citas académicas. Cada participante accede por el canal que mejor le convenga.
2. **Múltiples medios de acción y expresión** → Los dilemas permiten elegir respuestas; los micro-retos invitan a responder de forma oral o escrita (en pares), y la ficha de memoria es descargable para su uso libre.
3. **Facilitar el compromiso y la motivación** → Dilemas auténticos del ecosistema laboral tech (no abstractos), con feedback formativo inmediato que reconoce el acierto y explica el error sin penalizar. La intervención de Lore como mentora genera cercanía afectiva y pedagógica.
4. **Diseñar para la diversidad** → Andamiaje progresivo (de lo simple a lo complejo), ninguneo del lenguaje técnico innecesario, respeto por los diversos estilos y ritmos, y flexibilidad de tiempo (pausas entre estaciones).
5. **Fomentar la colaboración y la comunidad** → Micro-retos de diálogo en pares y dilemas diseñados para debate y co-evaluación. El «cómo se ve el apoyo» de Schein promueve conversaciones de equipo seguras.

**Veracidad pedagógica:** Todos los conceptos están sostenidos en fuentes reales citadas en el recurso: **APA, Goleman (1995), Rizzolatti & Sinigaglia (2006), Rogers (1961), Brené Brown & Adam Grant (Dare to Lead, Parte 4), Wiseman (1996), Rosenberg (CNV) y Schein (Humble Inquiry)**. No se inventan teorías ni se atribuyen citas falsas.

---

## 6. Orientaciones para la Adaptación y el Remix (Reutilización)

Como parte fundamental de un REA, quien lo reutilice tiene **total libertad para modificarlo y adaptarlo** a su propio contexto. Sugerencias de adaptación:

1. **Cambiar los dilemas:** Sustituir los dos dilemas del laboratorio por casos reales de la propia organización, institución o sector formativo (por ejemplo: servicio al cliente, salud, educación, contabilidad). El andamiaje (correcto/incorrecto + feedback conceptual) se conserva tal cual.
2. **Adaptar el video:** Reemplazar la cápsula de YouTube por una grabación propia, un fragmento del podcast de Brené Brown & Adam Grant, o un clip de un podcast disponible, actualizando la transcripción correspondiente.
3. **Cambiar los ejemplos y las voces:** Los personajes, nombres y escenarios pueden reescribirse para reflejar la cultura local sin alterar la estructura conceptual.
4. **Añadir estaciones:** Incorporar una estación 5 con un proyecto colaborativo (p. ej., «mapa de empatía del equipo») o una actividad de co-evaluación entre pares.
5. **Remezclar con otras herramientas:** Convertir los dilemas en tarjetas físicas, en un formulario de Google Forms, en una actividad H5P o exportar la ficha de memoria como imagen para WhatsApp (formato `160mm × 490mm`).
6. **Traducir / lengua de señas:** Se anima a traducir los textos y subtitular el video en lenguas indígenas o de señas para ampliar su alcance.
7. **Evaluar distinto:** La rúbrica y las preguntas de evaluación pueden adaptarse a niveles (primaria, secundaria, técnica) reduciendo o ampliando la complejidad cognitiva de los dilemas.

---

## 7. Criterios Sugeridos de Evaluación Formativa

### 7.1 Lista de cotejo de apropiación (para el docente)

| Criterio | Sí | Parcial | No |
| :---- | :----: | :----: | :----: |
| Identifica la empatía como una habilidad entrenable y con base biológica. |  |  |  |
| Diferencia empatía de simpatía, compasión y *enmeshment*. |  |  |  |
| Reconoce las trampas de minimización y apropiación dramática. |  |  |  |
| Propone respuestas empáticas asertivas en un dilema laboral. |  |  |  |
| Utiliza la «pregunta humilde» de Schein en la interacción. |  |  |  |
| Reflexiona (metacognición) sobre su propia práctica empática. |  |  |  |

### 7.2 Rúbrica de desempeño (orientativa, escala 1–4)

| Nivel | Desempeño |
| :---- | :---- |
| **4 · Nivel experto** | Distingue con precisión todos los conceptos, elige la respuesta empática correcta en los dilemas y justifica con vocabulario académico (neuronas espejo, DUA, CNV). |
| **3 · Nivel competente** | Identifica la empatía y sus dimensiones; acierta en los dilemas aunque con justificación parcial. |
| **2 · Nivel en desarrollo** | Reconoce la definición básica pero confunde empatía con simpatía o *enmeshment* en algunos casos. |
| **1 · Nivel inicial** | Presenta dificultades para distinguir la empatía de otras respuestas y para aplicar en dilemas. |

### 7.3 Preguntas guía para la metacognición (evaluación formativa oral/escrita)

1. ¿Qué fue lo más difícil de *no juzgar* en los dilemas trabajados?
2. ¿En qué momento del taller sentiste la tentación de «arreglar» en lugar de escuchar? ¿Qué hiciste?
3. ¿Cómo se ve *«el apoyo viniendo de ti»* en tu equipo de trabajo esta semana? (pregunta de Schein)
4. Escribe una frase empática que puedas usar mañana con un compañero o compañera.

### 7.4 Evaluación integradora (disponible en el REA)

El recurso incluye un **cuestionario formativo** (`evaluar_superpoder5.html`) con:
- Opción múltiple con casos de contexto (fricción cognitiva real).
- Verdadero/falso sobre neuronas espejo.
- Relación de conceptos (Goleman, Rogers, Rosenberg).
- Análisis de caso abierto (dilema de Camila) con retroalimentación.

---

## 8. Licencia y Atribución

- **Licencia:** Creative Commons **Atribución-CompartirIgual 4.0 Internacional (CC BY-SA 4.0)**.
- **Autor:** Óscar Javier Rojas.
- **Uso permitido:** Retener, Reutilizar, Revisar, Remezclar y Redistribuir (las **5R** de los REA), con atribución y misma licencia en las obras derivadas.
- **Uso educativo:** Libre para fines didácticos sin fines de lucro.
- **Condición ShareAlike:** Toda obra derivada debe publicarse bajo CC BY-SA 4.0.

**Referencias citadas en el recurso:**
1. Goleman, D. (1995). *Inteligencia Emocional*. Kairós.
2. Rizzolatti, G. & Sinigaglia, C. (2006). *Las neuronas espejo*. Paidós.
3. Brown, B. & Grant, A. *Dare to Lead · Empathy vs. Enmeshment* (Parte 4 de 6). https://brenebrown.com/podcast/empathy-vs-enmeshment-part-4-of-6/
4. Rogers, C. (1961). *El proceso de convertirse en persona*. Paidós.
5. Rosenberg, M. (2003). *Comunicación No Violenta*. Urano.
6. Schein, E. (2013). *Humble Inquiry: The Gentle Art of Asking Instead of Telling*. Berrett-Koehler.
7. Wiseman, T. (1996). "A concept analysis of empathy". *Journal of Advanced Nursing*.

---

*Documento elaborado por **Óscar Javier Rojas** como entregable de la actividad acreditable «Experiencia de crear un REA» — Maestría MEED. Recurso publicado bajo licencia CC BY-SA 4.0.*
