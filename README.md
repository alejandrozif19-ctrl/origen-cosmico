<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Origen Cósmico — Comprende el Universo | Edison Avilés</title>
  <meta name="description" content="Guía moderna y clara para entender el universo: Big Bang, agujeros negros, materia oscura y más. Creado por Edison Avilés.">
  <meta name="author" content="Edison Avilés">
  <meta name="theme-color" content="#0a0a1a">
  
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            space: { 950: '#05050f', 900: '#0a0a1a', 800: '#12122a', 700: '#1a1a3a' },
            star: '#e8e8ff',
            nebula: '#7c5cff',
            cosmic: '#00d4ff',
          },
          fontFamily: {
            sans: ['Inter', 'system-ui', 'sans-serif'],
            display: ['Space Grotesk', 'Inter', 'sans-serif'],
          }
        }
      }
    }
  </script>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
  
  <style>
    body {
      background: radial-gradient(ellipse at top, #12122a 0%, #05050f 70%);
      min-height: 100vh;
    }
    .stars {
      background-image: 
        radial-gradient(1px 1px at 20px 30px, #fff, transparent),
        radial-gradient(1px 1px at 40px 70px, rgba(255,255,255,0.8), transparent),
        radial-gradient(1.5px 1.5px at 50px 160px, #fff, transparent),
        radial-gradient(1px 1px at 90px 40px, rgba(255,255,255,0.6), transparent),
        radial-gradient(2px 2px at 130px 80px, #fff, transparent),
        radial-gradient(1px 1px at 160px 120px, rgba(255,255,255,0.7), transparent);
      background-size: 200px 200px;
      animation: twinkle 8s ease-in-out infinite;
    }
    @keyframes twinkle {
      0%, 100% { opacity: 0.7; }
      50% { opacity: 1; }
    }
    .glass {
      background: rgba(18, 18, 42, 0.65);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(124, 92, 255, 0.15);
    }
    .glow-text { text-shadow: 0 0 40px rgba(124, 92, 255, 0.5); }
    .card-hover { transition: all 0.3s ease; }
    .card-hover:hover {
      transform: translateY(-6px);
      border-color: rgba(0, 212, 255, 0.4);
      box-shadow: 0 20px 40px -15px rgba(0, 212, 255, 0.2);
    }
    ::-webkit-scrollbar { width: 8px; }
    ::-webkit-scrollbar-track { background: #0a0a1a; }
    ::-webkit-scrollbar-thumb { background: #3a3a6a; border-radius: 4px; }
  </style>
</head>
<body class="text-star font-sans antialiased">

  <div class="fixed inset-0 stars pointer-events-none opacity-40"></div>

  <!-- NAV -->
  <nav class="relative z-50 border-b border-white/5 sticky top-0 bg-space-950/80 backdrop-blur-md">
    <div class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
      <a href="index.html" class="flex items-center gap-3 group">
        <div class="w-9 h-9 rounded-full bg-gradient-to-br from-nebula to-cosmic flex items-center justify-center text-lg font-bold">∞</div>
        <span class="font-display font-semibold text-lg tracking-tight group-hover:text-cosmic transition-colors">Origen Cósmico</span>
      </a>
      <div class="hidden md:flex items-center gap-7 text-sm font-medium text-white/70">
        <a href="#escala" class="hover:text-white transition-colors">Escala</a>
        <a href="#temas" class="hover:text-white transition-colors">Temas</a>
        <a href="#aprender" class="hover:text-white transition-colors">Aprender</a>
        <a href="blog.html" class="hover:text-white transition-colors">Blog</a>
        <a href="#recursos" class="hover:text-white transition-colors">Recursos</a>
      </div>
      <a href="#empezar" class="px-5 py-2 rounded-full bg-nebula/20 border border-nebula/40 text-sm font-medium hover:bg-nebula/30 transition-all">
        Empezar
      </a>
    </div>
  </nav>

  <!-- HERO -->
  <header class="relative z-10 pt-20 pb-24 px-6">
    <div class="max-w-4xl mx-auto text-center">
      <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full glass text-xs font-medium text-cosmic mb-8">
        <span class="w-2 h-2 rounded-full bg-cosmic animate-pulse"></span>
        El universo es comprensible
      </div>
      
      <h1 class="font-display text-5xl md:text-7xl font-bold leading-[1.1] tracking-tight mb-6 glow-text">
        Comprende el<br>
        <span class="bg-gradient-to-r from-nebula via-cosmic to-nebula bg-clip-text text-transparent">Universo</span>
      </h1>
      
      <p class="text-lg md:text-xl text-white/60 max-w-2xl mx-auto mb-10 leading-relaxed">
        Una guía clara y visual sobre el Big Bang, agujeros negros, materia oscura y todo lo que sabemos (y lo que aún no) del cosmos.
      </p>
      
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="#temas" class="px-8 py-4 rounded-full bg-gradient-to-r from-nebula to-cosmic text-space-950 font-semibold hover:opacity-90 transition-opacity shadow-lg shadow-nebula/25">
          Explorar temas
        </a>
        <a href="blog.html" class="px-8 py-4 rounded-full glass text-white/80 font-medium hover:text-white transition-colors">
          Ir al Blog →
        </a>
      </div>
      
      <p class="mt-10 text-sm text-white/30">Creado por <span class="text-white/50">Edison Avilés</span></p>
    </div>
  </header>

  <!-- ESCALA -->
  <section id="escala" class="relative z-10 py-20 px-6">
    <div class="max-w-6xl mx-auto">
      <div class="text-center mb-14">
        <h2 class="font-display text-3xl md:text-4xl font-bold mb-4">La escala que cambia todo</h2>
        <p class="text-white/50 max-w-xl mx-auto">Entender el universo empieza por sentir lo pequeño que somos.</p>
      </div>
      
      <div class="grid md:grid-cols-3 gap-6 mb-10">
        <div class="glass rounded-2xl p-8 card-hover">
          <div class="text-4xl mb-4">🌍</div>
          <h3 class="font-display text-xl font-semibold mb-3">Tierra</h3>
          <p class="text-white/50 text-sm leading-relaxed">12.742 km de diámetro. Un punto azul pálido en la inmensidad.</p>
        </div>
        <div class="glass rounded-2xl p-8 card-hover">
          <div class="text-4xl mb-4">☀️</div>
          <h3 class="font-display text-xl font-semibold mb-3">Sistema Solar</h3>
          <p class="text-white/50 text-sm leading-relaxed">El Sol es 109 veces más grande que la Tierra. Neptuno está a 4.500 millones de km.</p>
        </div>
        <div class="glass rounded-2xl p-8 card-hover">
          <div class="text-4xl mb-4">🌌</div>
          <h3 class="font-display text-xl font-semibold mb-3">Vía Láctea</h3>
          <p class="text-white/50 text-sm leading-relaxed">100.000 años luz de diámetro. Cientos de miles de millones de estrellas.</p>
        </div>
      </div>
      
      <div class="glass rounded-2xl p-10 text-center">
        <p class="text-white/40 text-sm uppercase tracking-widest mb-3">Universo observable</p>
        <p class="font-display text-4xl md:text-6xl font-bold bg-gradient-to-r from-cosmic to-nebula bg-clip-text text-transparent mb-4">
          93.000 millones de años luz
        </p>
        <p class="text-white/50 max-w-lg mx-auto text-sm">Eso es solo lo que podemos ver. El universo real podría ser mucho más grande… o infinito.</p>
      </div>
    </div>
  </section>

  <!-- TEMAS PRINCIPALES -->
  <section id="temas" class="relative z-10 py-20 px-6 bg-space-900/40">
    <div class="max-w-6xl mx-auto">
      <div class="text-center mb-14">
        <h2 class="font-display text-3xl md:text-4xl font-bold mb-4">Temas fundamentales</h2>
        <p class="text-white/50 max-w-xl mx-auto">Los pilares para comprender cómo funciona el cosmos.</p>
      </div>

      <!-- Big Bang -->
      <div id="bigbang" class="glass rounded-2xl p-8 md:p-10 mb-8">
        <div class="flex flex-col md:flex-row gap-8 items-start">
          <div class="flex-shrink-0 w-16 h-16 rounded-2xl bg-gradient-to-br from-orange-500/30 to-red-500/20 flex items-center justify-center text-3xl">💥</div>
          <div class="flex-1">
            <h3 class="font-display text-2xl font-bold mb-3">El Big Bang</h3>
            <p class="text-white/60 leading-relaxed mb-4">
              Hace aproximadamente <strong class="text-white">13.800 millones de años</strong> el universo comenzó a expandirse a partir de un estado extremadamente caliente y denso. No fue una explosión en el espacio, sino la expansión del propio espacio.
            </p>
            <div class="grid sm:grid-cols-2 gap-4 text-sm">
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">¿Qué sabemos?</p>
                <p class="text-white/50">La expansión del universo, la radiación de fondo de microondas (CMB) y la abundancia de elementos ligeros confirman el modelo.</p>
              </div>
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">¿Qué no sabemos?</p>
                <p class="text-white/50">Qué provocó el Big Bang, qué había “antes” (si es que la pregunta tiene sentido) y la naturaleza exacta de la inflación cósmica.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Agujeros Negros -->
      <div id="agujeros" class="glass rounded-2xl p-8 md:p-10 mb-8">
        <div class="flex flex-col md:flex-row gap-8 items-start">
          <div class="flex-shrink-0 w-16 h-16 rounded-2xl bg-gradient-to-br from-purple-500/30 to-indigo-500/20 flex items-center justify-center text-3xl">🕳️</div>
          <div class="flex-1">
            <h3 class="font-display text-2xl font-bold mb-3">Agujeros Negros</h3>
            <p class="text-white/60 leading-relaxed mb-4">
              Regiones del espacio donde la gravedad es tan intensa que nada, ni siquiera la luz, puede escapar. Se forman cuando estrellas muy masivas colapsan al final de su vida, o en el centro de las galaxias (agujeros negros supermasivos).
            </p>
            <div class="grid sm:grid-cols-3 gap-4 text-sm">
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">Horizonte de sucesos</p>
                <p class="text-white/50">El “punto de no retorno”. Una vez cruzado, no hay vuelta atrás.</p>
              </div>
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">Sagitario A*</p>
                <p class="text-white/50">El agujero negro supermasivo en el centro de nuestra galaxia. Ya tenemos su imagen.</p>
              </div>
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">Ondas gravitacionales</p>
                <p class="text-white/50">Detectamos la fusión de agujeros negros gracias a LIGO y Virgo.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Materia y Energía Oscura -->
      <div id="oscura" class="glass rounded-2xl p-8 md:p-10 mb-8">
        <div class="flex flex-col md:flex-row gap-8 items-start">
          <div class="flex-shrink-0 w-16 h-16 rounded-2xl bg-gradient-to-br from-cyan-500/30 to-blue-500/20 flex items-center justify-center text-3xl">🌑</div>
          <div class="flex-1">
            <h3 class="font-display text-2xl font-bold mb-3">Materia Oscura y Energía Oscura</h3>
            <p class="text-white/60 leading-relaxed mb-4">
              Solo el <strong class="text-white">~5%</strong> del universo es materia ordinaria (la que conocemos). El resto es un misterio:
            </p>
            <div class="grid sm:grid-cols-2 gap-4 text-sm">
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">Materia Oscura (~27%)</p>
                <p class="text-white/50">No emite ni absorbe luz, pero su gravedad mantiene unidas a las galaxias. Aún no sabemos de qué está hecha.</p>
              </div>
              <div class="bg-white/5 rounded-xl p-4">
                <p class="text-cosmic font-medium mb-1">Energía Oscura (~68%)</p>
                <p class="text-white/50">Es lo que acelera la expansión del universo. Es el mayor misterio de la cosmología actual.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Expansión y Multiverso / Más temas -->
      <div class="grid md:grid-cols-2 gap-6">
        <div class="glass rounded-2xl p-7 card-hover">
          <div class="text-3xl mb-3">📈</div>
          <h3 class="font-display text-xl font-semibold mb-2">Expansión del Universo</h3>
          <p class="text-white/50 text-sm leading-relaxed">
            Descubierta por Edwin Hubble. Las galaxias se alejan unas de otras. Cuanto más lejos están, más rápido se alejan. La expansión se está acelerando.
          </p>
        </div>
        <div class="glass rounded-2xl p-7 card-hover">
          <div class="text-3xl mb-3">🧬</div>
          <h3 class="font-display text-xl font-semibold mb-2">Origen de los elementos</h3>
          <p class="text-white/50 text-sm leading-relaxed">
            El hidrógeno y el helio se formaron en los primeros minutos. El resto de elementos se crearon en el interior de las estrellas y en supernovas.
          </p>
        </div>
        <div class="glass rounded-2xl p-7 card-hover">
          <div class="text-3xl mb-3">🌀</div>
          <h3 class="font-display text-xl font-semibold mb-2">Galaxias y estructura a gran escala</h3>
          <p class="text-white/50 text-sm leading-relaxed">
            El universo no es uniforme: forma una “red cósmica” de filamentos de galaxias, cúmulos y grandes vacíos.
          </p>
        </div>
        <div class="glass rounded-2xl p-7 card-hover">
          <div class="text-3xl mb-3">⏳</div>
          <h3 class="font-display text-xl font-semibold mb-2">Destino del Universo</h3>
          <p class="text-white/50 text-sm leading-relaxed">
            Según los datos actuales, lo más probable es la “muerte térmica”: expansión eterna hasta que todo se enfríe y se apague.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- CÓMO APRENDER -->
  <section id="aprender" class="relative z-10 py-20 px-6">
    <div class="max-w-6xl mx-auto">
      <div class="text-center mb-14">
        <h2 class="font-display text-3xl md:text-4xl font-bold mb-4">Cómo empezar a comprenderlo</h2>
        <p class="text-white/50 max-w-xl mx-auto">Un camino sencillo y realista.</p>
      </div>
      
      <div class="grid md:grid-cols-2 gap-8">
        <div class="space-y-5">
          <div class="flex gap-4">
            <div class="flex-shrink-0 w-10 h-10 rounded-full bg-nebula/20 border border-nebula/40 flex items-center justify-center font-display font-bold text-nebula">1</div>
            <div>
              <h3 class="font-semibold mb-1">Observa el cielo</h3>
              <p class="text-white/50 text-sm">Apps como Stellarium o SkySafari. Binoculares o un telescopio pequeño ayudan mucho.</p>
            </div>
          </div>
          <div class="flex gap-4">
            <div class="flex-shrink-0 w-10 h-10 rounded-full bg-nebula/20 border border-nebula/40 flex items-center justify-center font-display font-bold text-nebula">2</div>
            <div>
              <h3 class="font-semibold mb-1">Viaja visualmente</h3>
              <p class="text-white/50 text-sm">Mira el documental 4K de viaje por el universo y Cosmos de Carl Sagan.</p>
            </div>
          </div>
          <div class="flex gap-4">
            <div class="flex-shrink-0 w-10 h-10 rounded-full bg-nebula/20 border border-nebula/40 flex items-center justify-center font-display font-bold text-nebula">3</div>
            <div>
              <h3 class="font-semibold mb-1">Conceptos clave</h3>
              <p class="text-white/50 text-sm">ScienceClic y canales serios te explican relatividad, cuántica y cosmología con claridad.</p>
            </div>
          </div>
          <div class="flex gap-4">
            <div class="flex-shrink-0 w-10 h-10 rounded-full bg-nebula/20 border border-nebula/40 flex items-center justify-center font-display font-bold text-nebula">4</div>
            <div>
              <h3 class="font-semibold mb-1">Profundiza</h3>
              <p class="text-white/50 text-sm">Libros (Hawking, Sagan, Carroll…) y, si quieres, matemáticas y física básica.</p>
            </div>
          </div>
        </div>
        
        <div class="glass rounded-2xl p-8">
          <h3 class="font-display text-xl font-semibold mb-5">Actitud recomendada</h3>
          <ul class="space-y-3 text-white/60 text-sm">
            <li class="flex gap-3"><span class="text-cosmic">→</span> Acepta que no lo sabemos todo</li>
            <li class="flex gap-3"><span class="text-cosmic">→</span> Prefiere la claridad a la complejidad innecesaria</li>
            <li class="flex gap-3"><span class="text-cosmic">→</span> Combina asombro con rigor</li>
            <li class="flex gap-3"><span class="text-cosmic">→</span> Sé paciente: el universo no se entiende en un día</li>
            <li class="flex gap-3"><span class="text-cosmic">→</span> Pregunta siempre y verifica las fuentes</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- RECURSOS -->
  <section id="recursos" class="relative z-10 py-20 px-6 bg-space-900/40">
    <div class="max-w-6xl mx-auto">
      <div class="text-center mb-14">
        <h2 class="font-display text-3xl md:text-4xl font-bold mb-4">Recursos recomendados</h2>
        <p class="text-white/50">Seleccionados por claridad y calidad.</p>
      </div>
      
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
        <a href="https://www.youtube.com/watch?v=FjTbRjwqXxA" target="_blank" rel="noopener" class="glass rounded-2xl p-6 card-hover block group">
          <div class="text-xs text-white/40 uppercase tracking-wider mb-3">Documental 4K</div>
          <h3 class="font-semibold text-lg mb-2 group-hover:text-cosmic transition-colors">Viaje por el Universo</h3>
          <p class="text-white/50 text-sm">Imágenes reales NASA/ESA. El mejor recorrido visual disponible.</p>
        </a>
        <a href="https://www.youtube.com/@ScienceClicES" target="_blank" rel="noopener" class="glass rounded-2xl p-6 card-hover block group">
          <div class="text-xs text-white/40 uppercase tracking-wider mb-3">Canal</div>
          <h3 class="font-semibold text-lg mb-2 group-hover:text-cosmic transition-colors">ScienceClic Español</h3>
          <p class="text-white/50 text-sm">Explicaciones visuales precisas de física moderna.</p>
        </a>
        <a href="https://www.youtube.com/results?search_query=carl+sagan+cosmos" target="_blank" rel="noopener" class="glass rounded-2xl p-6 card-hover block group">
          <div class="text-xs text-white/40 uppercase tracking-wider mb-3">Clásico</div>
          <h3 class="font-semibold text-lg mb-2 group-hover:text-cosmic transition-colors">Cosmos — Carl Sagan</h3>
          <p class="text-white/50 text-sm">El documental que cambió cómo vemos el cosmos.</p>
        </a>
        <div class="glass rounded-2xl p-6">
          <div class="text-xs text-white/40 uppercase tracking-wider mb-3">Libro</div>
          <h3 class="font-semibold text-lg mb-2">Una breve historia del tiempo</h3>
          <p class="text-white/50 text-sm">Stephen Hawking. Claro y profundo.</p>
        </div>
        <div class="glass rounded-2xl p-6">
          <div class="text-xs text-white/40 uppercase tracking-wider mb-3">Libro</div>
          <h3 class="font-semibold text-lg mb-2">Cosmos</h3>
          <p class="text-white/50 text-sm">Carl Sagan. Ciencia y poesía juntas.</p>
        </div>
 
