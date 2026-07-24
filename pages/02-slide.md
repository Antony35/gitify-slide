<!--
╔══════════════════════════════════════════════╗
║       SLIDE 2 — GitHub ne suffit pas         ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-6 h-full text-center">

  <!-- Label de slide -->
  <p class="mono text-xs tracking-widest uppercase dim-25"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    GitHub ne suffit pas
  </p>

  <!-- Chiffre choc -->
  <div class="leading-none" 
    v-motion="{ initial: { scale: 0, y: 20 }, visible: { scale: 1, y: 0, transition: { duration: 1200, delay: 300 } } }">
    <span class="mono font-black text-white" style="font-size: 8rem; line-height: 1;">100M</span><span class="mono font-black text-red" style="font-size: 8rem; line-height: 1">+</span>
  </div>

  <p class="text-2xl dim-50"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }">repositories sur GitHub.</p>

  <!-- Punch line -->
  <div class="mt-4 px-10 py-5 card"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }">
    <p class="mono text-xl dim-80">
       Comment trouver le repos qui te correspond.
    </p>
  </div>

</div>

<!--
NOTES ORATEUR — Slide 2
GitHub c'est immense — plus de 100 millions de repos publics.
Mais quand tu es développeur junior, ou même confirmé, et que tu cherches un projet open source
auquel contribuer... tu te retrouves seul face à un moteur de recherche.
Personne ne te demande ton niveau, tes langages, tes disponibilités.
Résultat : la plupart abandonnent avant même d'avoir trouvé quelque chose.
-->