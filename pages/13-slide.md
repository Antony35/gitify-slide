<!--
╔══════════════════════════════════════════════╗
║  SLIDE 13 — Merci.                           ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full text-center">

  <!-- Merci -->
  <p class="text-6xl font-bold text-white" 
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }"
    >Merci<span v-motion="{ initial: { opacity: 1 }, enter: { opacity: [1, 1, 0, 0], transition: { duration: 1000, repeat: Infinity, ease: 'linear', times: [0, 0.49, 0.5, 1] } } }" class="text-red">_</span></p>

  <div class="w-16 h-px" style="background: rgba(255,255,255,0.1);"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }"
    ></div>

  <!-- Questions -->
  <p class="mono text-sm dim-30" 
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 800 } } }"
  >Place aux questions.</p>

  <!-- Équipe -->
  <p class="text-xs tracking-widest uppercase dim-20" style="letter-spacing: 0.3em"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1000 } } }">
    Antony &nbsp;·&nbsp; Josué &nbsp;·&nbsp; Richard &nbsp;·&nbsp; Nicolas &nbsp;·&nbsp; Théo
  </p>

</div>

<!--
NOTES ORATEUR — Slide 13
Merci de nous avoir écoutés.
On est disponibles pour répondre à vos questions.
-->