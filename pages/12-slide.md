<!--
╔══════════════════════════════════════════════╗
║  SLIDE 12 — Gitify demain                    ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase" style="color: rgba(255,255,255,0.25);" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    Gitify demain
  </p>

  <!-- On retire l'animation de groupe pour animer les 4 cartes une par une -->
  <div class="grid grid-cols-2 gap-4" style="width: 640px;">

  <!-- Notifications -->
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <span class="text-xl">🔔</span>
    <div>
        <p class="font-semibold text-sm text-white">Notifications</p>
        <p class="text-xs mt-1" style="color: rgba(255,255,255,0.4);">Alertes sur les nouvelles issues des projets favoris</p>
    </div>
  </div>

  <!-- Application mobile -->
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 450 } } }">
    <span class="text-xl">📱</span>
    <div>
        <p class="font-semibold text-sm text-white">Application mobile</p>
        <p class="text-xs mt-1" style="color: rgba(255,255,255,0.4);">Swipe natif sur iOS & Android</p>
    </div>
  </div>

  <!-- Suivi de contribution -->
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">
    <span class="text-xl">📊</span>
    <div>
        <p class="font-semibold text-sm text-white">Suivi de contribution</p>
        <p class="text-xs mt-1" style="color: rgba(255,255,255,0.4);">Historique des PRs et issues soumises</p>
    </div>
  </div>

  <!-- Mode équipe -->
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 750 } } }">
    <span class="text-xl">👥</span>
    <div>
        <p class="font-semibold text-sm text-white">Mode équipe</p>
        <p class="text-xs mt-1" style="color: rgba(255,255,255,0.4);">Matching de projets pour plusieurs devs</p>
    </div>
  </div>

</div>

  <!-- Apparition du texte de fin en dernier -->
  <p class="mono text-xs" style="color: rgba(255,255,255,0.2);" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 900 } } }">
    La base est là. Le potentiel aussi.
  </p>

</div>

<!--
NOTES ORATEUR — Slide 12
Gitify c'est une v1 — et on sait exactement où elle peut aller.
Côté utilisateur, les notifications permettraient d'être alerté quand une nouvelle issue s'ouvre sur un projet qu'on a mis en favoris. L'application mobile rendrait l'expérience encore plus naturelle — le swipe est fait pour le tactile.
Côté produit, un suivi de contribution permettrait de voir l'historique de ses PRs et issues soumises directement depuis Gitify. Et un mode équipe ouvrirait la plateforme à des groupes de développeurs qui cherchent un projet commun.
La fondation technique qu'on a posée — monorepo, API documentée, architecture modulaire — est conçue pour accueillir ces évolutions.
-->