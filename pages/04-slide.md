<!--
╔══════════════════════════════════════════════╗
║  SLIDE 4 — L'équipe                          ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase" style="color: rgba(255,255,255,0.25);"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">L'équipe</p>

  <!-- Cartes membres -->
  <div class="flex gap-4 justify-center flex-wrap" 
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">

  <!-- Richard -->
  <div class="card flex flex-col items-center gap-3 px-6 py-5 w-36">
    <div class="w-12 h-12 rounded-full flex items-center justify-center mono font-bold text-sm" style="background: rgba(166,240,211,0.1); color: #A6F0D3; border: 1px solid rgba(166,240,211,0.25);"
        v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 800, delay: 400 } } }">RK</div>
    <div class="text-center">
        <p class="font-semibold text-sm text-white"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }">Richard</p>
        <p class="mono text-xs mt-1" style="color: #A6F0D3;"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">Lead Dev</p>
    </div>
  </div>
  
  <!-- Antony -->
  <div class="card flex flex-col items-center gap-3 px-6 py-5 w-36">
    <div class="w-12 h-12 rounded-full flex items-center justify-center mono font-bold text-sm" style="background: rgba(166,240,211,0.1); color: #A6F0D3; border: 1px solid rgba(166,240,211,0.25);"
        v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 800, delay: 500 } } }">AH</div>
    <div class="text-center">
        <p class="font-semibold text-sm text-white"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">Antony</p>
        <p class="mono text-xs mt-1" style="color: #A6F0D3;"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }">Backend</p>
    </div>
  </div>
  
  <!-- Théo -->
  <div class="card flex flex-col items-center gap-3 px-6 py-5 w-36">
    <div class="w-12 h-12 rounded-full flex items-center justify-center mono font-bold text-sm" style="background: rgba(255,35,2,0.1); color: #FF2302; border: 1px solid rgba(255,35,2,0.25);"
        v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 800, delay: 600 } } }">TH</div>
    <div class="text-center">
        <p class="font-semibold text-sm text-white"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }">Théo</p>
        <p class="mono text-xs mt-1" style="color: #FF2302;"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 800 } } }">PO · Design</p>
    </div>
  </div>
  
  <!-- Josué -->
  <div class="card flex flex-col items-center gap-3 px-6 py-5 w-36">
    <div class="w-12 h-12 rounded-full flex items-center justify-center mono font-bold text-sm" style="background: rgba(166,240,211,0.1); color: #A6F0D3; border: 1px solid rgba(166,240,211,0.25);"
        v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 800, delay: 700 } } }">JO</div>
    <div class="text-center">
        <p class="font-semibold text-sm text-white"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 800 } } }">Josué</p>
        <p class="mono text-xs mt-1" style="color: #A6F0D3;"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 900 } } }">Frontend</p>
    </div>
  </div>
  
  <!-- Nicolas -->
  <div class="card flex flex-col items-center gap-3 px-6 py-5 w-36">
    <div class="w-12 h-12 rounded-full flex items-center justify-center mono font-bold text-sm" style="background: rgba(166,240,211,0.1); color: #A6F0D3; border: 1px solid rgba(166,240,211,0.25);"
        v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 800, delay: 800 } } }">NI</div>
    <div class="text-center">
        <p class="font-semibold text-sm text-white"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 900 } } }">Nicolas</p>
        <p class="mono text-xs mt-1" style="color: #A6F0D3;"
          v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1000 } } }">Frontend</p>
    </div>
  </div>
  
</div>
  
  <p class="text-xs" style="color: rgba(255,255,255,0.2);" 
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1100 } } }">ESGI 5e année &nbsp;·&nbsp; Janvier → Juillet 2026</p>
</div>

<!--
NOTES ORATEUR — Slide 4
Notre équipe c'est 5 profils complémentaires.
Richard a assuré le rôle de lead dev — architecture, revues de code, décisions techniques.
Antony sur le backend : les API, la base de données, l'authentification.
Théo a porté le produit côté vision et design : UX, maquettes, priorités fonctionnelles.
Josué et Nicolas ont construit l'interface utilisateur, de l'onboarding au feed en passant par les favoris.
7 mois, une vraie organisation projet, et un livrable déployé en production.
-->
