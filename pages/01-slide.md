<!--
╔══════════════════════════════════════════════╗
║             SLIDE 1 — Couverture             ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-7 h-full">

  <!-- Logo + titre -->
  <div class="flex items-center gap-4" 
       v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    <div class="w-14 h-14 rounded-xl flex items-center justify-center mono font-bold text-xl text-mint"
         style="border: 2px solid #A6F0D3;">
      &gt;_
    </div>
    <span class="mono font-black text-6xl tracking-tight text-white">
      Gitify<span class="animate-blinkCursor text-red">_</span>
    </span>
  </div>

  <!-- Tagline -->
  <p class="mono text-2xl dim-45" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    Code, Collab, <span class="text-mint">Conquer.</span>
  </p>

  <!-- Séparateur -->
  <div class="w-16 h-px" style="background: rgba(255,255,255,0.1);" 
       v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }"></div>

  <!-- Équipe -->
  <p class="tracking-widest text-xs uppercase dim-25" style="letter-spacing: 0.3em;" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }">
    Josué &nbsp;·&nbsp; Richard &nbsp;·&nbsp; Théo &nbsp;·&nbsp; Antony &nbsp;·&nbsp; Nicolas
  </p>

  <!-- Contexte -->
  <p class="text-xs dim-15" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 900 } } }">
    Projet annuel 2025 / 2026 &nbsp;·&nbsp; ESGI
  </p>

</div>

<!--
NOTES ORATEUR — Slide 1
Bonjour à tous. Nous sommes l'équipe Gitify, 5 étudiants de l'ESGI en 5e année.
On vous présente aujourd'hui le fruit de 7 mois de travail : une application web qu'on a conçue,
développée, et déployée de A à Z.
-->