<!--
╔══════════════════════════════════════════════╗
║  SLIDE 6 — Le moteur de matching             ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-2 h-full">

  <p class="mono text-xs tracking-widest uppercase mb-4" style="color: rgba(255,255,255,0.25);" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    Le moteur de matching
  </p>

<!-- FLUX VERTICAL -->
<div class="flex flex-col items-center gap-0">

  <!-- Bloc 1 -->
  <div class="card px-8 py-3 text-center" style="min-width: 260px;"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <p class="mono text-sm font-semibold" style="color: #A6F0D3;">Tes préférences</p>
    <p class="text-xs mt-1" style="color: rgba(255,255,255,0.35);">langages · niveau · type de projets</p>
  </div>
  
  <!-- Flèche 1 -->
  <div class="flex flex-col items-center" style="color: rgba(255,255,255,0.2); gap: 0;"
    v-motion="{ initial: { opacity: 0 }, visible: { opacity: 1, transition: { duration: 500, delay: 450 } } }">
    <div style="width:1px; height:16px; background: rgba(255,255,255,0.15);"></div>
    <span style="font-size: 10px;">▼</span>
  </div>
  
  <!-- Bloc 2 — GitHub API + lazy-fetch -->
  <div class="flex items-center gap-3"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">
    <div class="card px-8 py-3 text-center" style="min-width: 260px;">
      <p class="mono text-sm font-semibold text-white">GitHub API</p>
      <p class="text-xs mt-1" style="color: rgba(255,255,255,0.35);">lazy-fetch si stock &lt; 25 projets</p>
    </div>
  </div>
  
  <!-- Flèche 2 -->
  <div class="flex flex-col items-center"
    v-motion="{ initial: { opacity: 0 }, visible: { opacity: 1, transition: { duration: 500, delay: 750 } } }">
    <div style="width:1px; height:16px; background: rgba(255,255,255,0.15);"></div>
    <span style="font-size: 10px; color: rgba(255,255,255,0.2);">▼</span>
  </div>
  
  <!-- Bloc 3 — Cache 2 niveaux -->
  <div class="px-8 py-4 text-center rounded-xl" style="min-width: 260px; background: rgba(166,240,211,0.05); border: 1px solid rgba(166,240,211,0.2);"
    v-motion="{ initial: { opacity: 0, scale: 0.95 }, visible: { opacity: 1, scale: 1, transition: { duration: 800, delay: 900 } } }">
    <p class="mono text-xs font-bold mb-2" style="color: #A6F0D3; letter-spacing: 0.1em;">CACHE</p>
    <div class="flex justify-center gap-6">
      <div>
        <p class="mono text-sm font-semibold text-white">24h</p>
        <p class="text-xs" style="color: rgba(255,255,255,0.35);">liste de repos</p>
      </div>
      <div style="width:1px; background: rgba(255,255,255,0.1);"></div>
      <div>
        <p class="mono text-sm font-semibold text-white">7j</p>
        <p class="text-xs" style="color: rgba(255,255,255,0.35);">détails d'un repo</p>
      </div>
    </div>
  </div>
  
  <!-- Flèche 3 -->
  <div class="flex flex-col items-center"
    v-motion="{ initial: { opacity: 0 }, visible: { opacity: 1, transition: { duration: 500, delay: 1050 } } }">
    <div style="width:1px; height:16px; background: rgba(255,255,255,0.15);"></div>
    <span style="font-size: 10px; color: rgba(255,255,255,0.2);">▼</span>
  </div>
  
  <!-- Bloc 4 — Round-robin -->
  <div class="card px-8 py-3 text-center" style="min-width: 260px;"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1200 } } }">
    <p class="mono text-sm font-semibold text-white">Round-robin par langage</p>
    <p class="text-xs mt-1" style="color: rgba(255,255,255,0.35);">équité entre TypeScript, Python, Rust…</p>
  </div>
  
  <!-- Flèche 4 -->
  <div class="flex flex-col items-center"
    v-motion="{ initial: { opacity: 0 }, visible: { opacity: 1, transition: { duration: 500, delay: 1350 } } }">
    <div style="width:1px; height:16px; background: rgba(255,255,255,0.15);"></div>
    <span style="font-size: 10px; color: rgba(255,255,255,0.2);">▼</span>
  </div>
  
  <!-- Bloc 5 — Feed -->
  <div class="px-8 py-3 text-center rounded-xl" style="min-width: 260px; background: rgba(255,35,2,0.08); border: 1px solid rgba(255,35,2,0.3);"
    v-motion="{ initial: { opacity: 0, scale: 0.8 }, visible: { opacity: 1, scale: 1, transition: { duration: 800, delay: 1500, type: 'spring', stiffness: 200 } } }">
    <p class="mono text-sm font-bold" style="color: #FF2302;">Ton feed ✓</p>
  </div>

</div>

</div>

<!--
NOTES ORATEUR — Slide 6
Le cœur de Gitify c'est cet algorithme.
Quand tu arrives sur le feed, on regarde tes préférences : langages, niveau, type de projets.
On compte les projets disponibles que tu n'as pas encore vus. Si on en a moins de 25 en stock, on déclenche un lazy-fetch vers l'API GitHub pour en récupérer de nouveaux — sans que tu aies à attendre.
Ce qu'on récupère est mis en cache à deux niveaux : la liste des repos pendant 24h, et les détails d'un repo spécifique pendant 7 jours. Ça évite de surcharger l'API GitHub à chaque visite.
Enfin, le round-robin par langage garantit que si tu aimes TypeScript, Python et Rust, tu ne te retrouves pas noyé sous du TypeScript — on alterne équitablement.
Résultat : un feed qui tourne, qui se renouvelle, et qui reste pertinent.
-->
