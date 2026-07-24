<!--
╔══════════════════════════════════════════════╗
║  SLIDE 5 — Les fonctionnalités               ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase dim-25"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">Les fonctionnalités</p>

  <div class="grid grid-cols-3 gap-4" style="width: 720px;">

  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <span class="text-xl mt-0.5">🔑</span>
    <div>
      <p class="font-semibold text-sm text-white">GitHub OAuth</p>
      <p class="text-xs mt-1 dim-40">Connexion en un clic via GitHub</p>
    </div>
  </div>
  
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 500 } } }">
    <span class="text-xl mt-0.5">⚙️</span>
    <div>
      <p class="font-semibold text-sm text-white">Préférences</p>
      <p class="text-xs mt-1 dim-40">Langages, niveau, type de projets</p>
    </div>
  </div>
  
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">
    <span class="text-xl mt-0.5">✨</span>
    <div>
      <p class="font-semibold text-sm text-white">Feed personnalisé</p>
      <p class="text-xs mt-1 dim-40">Projets matchés à ton profil</p>
    </div>
  </div>
  
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 800 } } }">
    <span class="text-xl mt-0.5">🤍</span>
    <div>
      <p class="font-semibold text-sm text-white">Favoris</p>
      <p class="text-xs mt-1 dim-40">Sauvegarde les projets qui t'intéressent</p>
    </div>
  </div>
  
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1000 } } }">
    <span class="text-xl mt-0.5">🌐</span>
    <div>
      <p class="font-semibold text-sm text-white">Landing publique</p>
      <p class="text-xs mt-1 dim-40">Showcase sans compte requis</p>
    </div>
  </div>
  
  <div class="card flex items-start gap-3 p-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1200 } } }">
    <span class="text-xl mt-0.5">📄</span>
    <div>
      <p class="font-semibold text-sm text-white">API documentée</p>
      <p class="text-xs mt-1 dim-40">OpenAPI + Scalar UI intégré</p>
    </div>
  </div>
  
  </div>

</div>

<!--
NOTES ORATEUR — Slide 5
Gitify c'est 6 fonctionnalités principales.
On commence par la connexion GitHub OAuth — pas de formulaire, pas de mot de passe, un clic et t'es connecté.
Ensuite l'onboarding préférences : on te demande ton niveau, tes langages, ce que tu cherches.
Le feed personnalisé c'est le cœur de l'app — on y reviendra dans la slide suivante.
Les favoris : tu mets de côté les projets qui t'intéressent pour y revenir plus tard.
La landing publique permet de découvrir Gitify sans compte, avec une sélection de projets en vitrine.
Et enfin une API entièrement documentée avec Scalar — pratique pour tester et pour la maintenance.
-->
