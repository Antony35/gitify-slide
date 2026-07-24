<!--
╔══════════════════════════════════════════════╗
║  SLIDE 8 — Gestion de projet                 ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase dim-25" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    Gestion de projet
  </p>

  <!-- Timeline horizontale -->
  <!-- On retire l'animation de groupe pour animer étape par étape -->
  <div class="flex items-start gap-0" style="width: 820px;">

  <!-- Étape 1 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-mint" style="background: rgba(166,240,211,0.12); border: 1px solid rgba(166,240,211,0.3)">1</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Initialisation</p>
    <p class="text-xs text-center dim-30">Cadrage · Specs · MoSCoW</p>
  </div>
  
  <!-- Étape 2 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 450 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-mint" style="background: rgba(166,240,211,0.12); border: 1px solid rgba(166,240,211,0.3)">2</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Maquettes</p>
    <p class="text-xs text-center dim-30">UX · UI · Design system</p>
  </div>
  
  <!-- Étape 3 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-mint" style="background: rgba(166,240,211,0.12); border: 1px solid rgba(166,240,211,0.3)">3</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Backend</p>
    <p class="text-xs text-center dim-30">API · Auth · Algo feed</p>
  </div>
  
  <!-- Étape 4 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 750 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-mint" style="background: rgba(166,240,211,0.12); border: 1px solid rgba(166,240,211,0.3)">4</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Frontend</p>
    <p class="text-xs text-center dim-30">Nuxt · Feed · Favoris</p>
  </div>
  
  <!-- Étape 5 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 900 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-mint" style="background: rgba(166,240,211,0.12); border: 1px solid rgba(166,240,211,0.3)">5</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Déploiement</p>
    <p class="text-xs text-center dim-30">Hetzner · Docker · CI/CD</p>
  </div>
  
  <!-- Étape 6 -->
  <div class="flex flex-col items-center gap-2 flex-1"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 1050 } } }">
    <div class="w-8 h-8 rounded-full flex items-center justify-center mono text-xs font-bold text-red" style="background: rgba(255,35,2,0.12); border: 1px solid rgba(255,35,2,0.3)">6</div>
    <div style="height: 2px; width: 100%; background: rgba(255,255,255,0.08);"></div>
    <p class="text-xs text-center font-semibold text-white px-1">Dossier & Slides</p>
    <p class="text-xs text-center dim-30">Rapport · Présentation</p>
  </div>

</div>

  <!-- Outils -->
  <div class="flex gap-4">
    <div class="card px-5 py-2 flex items-center gap-2"
         v-motion="{ initial: { opacity: 0, scale: 0.8 }, visible: { opacity: 1, scale: 1, transition: { duration: 800, delay: 1250, type: 'spring', stiffness: 200 } } }">
      <span class="text-sm">📋</span>
      <p class="mono text-xs dim-50">Notion</p>
    </div>
    <div class="card px-5 py-2 flex items-center gap-2"
         v-motion="{ initial: { opacity: 0, scale: 0.8 }, visible: { opacity: 1, scale: 1, transition: { duration: 800, delay: 1400, type: 'spring', stiffness: 200 } } }">
      <span class="text-sm">🗂️</span>
      <p class="mono text-xs dim-50">GitHub Projects</p>
    </div>
    <div class="card px-5 py-2 flex items-center gap-2"
         v-motion="{ initial: { opacity: 0, scale: 0.8 }, visible: { opacity: 1, scale: 1, transition: { duration: 800, delay: 1550, type: 'spring', stiffness: 200 } } }">
      <span class="text-sm">✅</span>
      <p class="mono text-xs dim-50">MoSCoW</p>
    </div>
  </div>

</div>

<!--
NOTES ORATEUR — Slide 8
Notre projet s'est déroulé sur 7 mois, de janvier à juillet 2026.
On a structuré le travail en 6 grandes phases.
D'abord l'initialisation : cadrage du projet, définition du périmètre fonctionnel avec la méthode MoSCoW pour prioriser ce qui est indispensable vs ce qui est optionnel.
Ensuite les maquettes, portées par Théo, pour valider l'UX avant de toucher une ligne de code.
Le backend a suivi en parallèle : API, authentification, base de données, algorithme de feed.
Le frontend a pris le relais pour intégrer le tout côté interface utilisateur.
Le déploiement a été mis en place progressivement avec des pipelines GitHub Actions.
Et on boucle avec le dossier et cette présentation.
On s'est appuyés sur Notion pour la documentation et les specs, GitHub Projects pour le suivi des tâches, et la méthode MoSCoW pour nos décisions produit.
-->
