<!--
╔══════════════════════════════════════════════╗
║  SLIDE 10 — Démonstration                    ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-10 h-full text-center">

  <!-- Icône play -->
  <div class="w-20 h-20 rounded-full flex items-center justify-center" style="background: rgba(255,35,2,0.1); border: 1px solid rgba(255,35,2,0.3);" 
       v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    <span style="font-size: 2rem; margin-left: 4px;">▶</span>
  </div>

  <div class="flex flex-col gap-2" 
       v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <h2 class="text-4xl font-bold text-white tracking-tight">Démonstration</h2>
    <p class="mono text-sm" style="color: rgba(255,255,255,0.3);">en direct</p>
  </div>

  <!-- Ce qu'on va montrer -->
  <div class="flex flex-col gap-3" style="width: 440px;">
    <div class="flex items-center gap-3 px-5 py-3 card rounded-xl"
         v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }">
      <span class="mono text-xs font-bold" style="color: #A6F0D3;">01</span>
      <p class="text-sm text-white">Onboarding & préférences</p> 
    </div>

  <div class="flex items-center gap-3 px-5 py-3 card rounded-xl"
      v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 650 } } }">
      <span class="mono text-xs font-bold" style="color: #A6F0D3;">02</span>
      <p class="text-sm text-white">Feed personnalisé</p>
    </div>
    
  <div class="flex items-center gap-3 px-5 py-3 card rounded-xl"
      v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 800 } } }">
      <span class="mono text-xs font-bold" style="color: #A6F0D3;">03</span>
      <p class="text-sm text-white">Gestion des favoris</p>
    </div>

  </div>

</div>

<!--
NOTES ORATEUR — Slide 10
On va maintenant vous faire une démonstration en direct de Gitify.
[Un membre de l'équipe est déjà connecté avec son compte GitHub]
On va vous montrer trois choses : d'abord l'onboarding avec la configuration des préférences, ensuite le feed personnalisé qui en résulte, et enfin la liste des favoris.
[Passer à la démo live]
-->