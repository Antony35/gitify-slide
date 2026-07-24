<!--
╔══════════════════════════════════════════════╗
║  SLIDE 9 — Réalité du projet                 ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase dim-25" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    Ce qu'on a appris
  </p>

  <!-- On retire l'animation de groupe pour animer carte par carte -->
  <div class="flex flex-col gap-4" style="width: 640px;">

  <!-- Auth -->
  <div class="card flex items-start gap-4 px-6 py-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 300 } } }">
    <span class="text-2xl mt-0.5">🔐</span>
    <div>
      <p class="font-semibold text-sm text-white">Authentification</p>
      <p class="text-xs mt-1 leading-relaxed dim-45">
        Implémenter manuellement les tokens HTTP-only, c'est complexe.
        Les sessions natives d'Adonis le font automatiquement — et mieux.
      </p>
    </div>
  </div>
  
  <!-- Docker permissions -->
  <div class="card flex items-start gap-4 px-6 py-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 450 } } }">
    <span class="text-2xl mt-0.5">🐳</span>
    <div>
      <p class="font-semibold text-sm text-white">Permissions Docker</p>
      <p class="text-xs mt-1 leading-relaxed dim-45">
        Problèmes de permissions de fichiers entre le host et les containers.
        Résolu en définissant <span class="mono text-mint">user: "node"</span> dans chaque service du Compose.
      </p>
    </div>
  </div>
  
  <!-- Organisation -->
  <div class="card flex items-start gap-4 px-6 py-4"
    v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 600 } } }">
    <span class="text-2xl mt-0.5">🗣️</span>
    <div>
      <p class="font-semibold text-sm text-white">Organisation d'équipe</p>
      <p class="text-xs mt-1 leading-relaxed dim-45">
        Plus de communication et des sprint reviews régulières auraient évité
        des désynchronisations sur l'avancement de chacun.
      </p>
    </div>
  </div>

</div>

</div>

<!--
NOTES ORATEUR — Slide 9
Tout projet a ses embûches — voilà les nôtres, et ce qu'on en a retenu.
Premier point : l'authentification. Au début j'ai implémenté manuellement les routes, la gestion du token opaque et la sécurisation HTTP-only. C'est faisable, mais complexe et source d'erreurs. Richard a identifié que les sessions natives d'Adonis gèrent tout ça automatiquement — le cookie est HTTP-only par défaut. Ça a simplifié énormément le code, et une fois le Swagger en place avec Scalar, l'équipe frontend n'avait même plus besoin de Postman pour tester l'API.
Deuxième point : Docker et les permissions. Quand on récupère un projet qu'on n'a pas créé soi-même, les fichiers n'appartiennent pas au bon utilisateur dans le container. La solution : définir `user: "node"` dans chaque service du docker-compose — plus aucun problème de permissions ensuite.
Troisième point : l'organisation. Ce qu'on referait différemment, c'est davantage de communication et des sprint reviews formalisées pour que tout le monde sache où en est chacun. Sur 7 mois, c'est facile de se désynchroniser.
-->
