<!--
╔══════════════════════════════════════════════╗
║  SLIDE 11 — Bilan & leçons                   ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-8 h-full">

  <p class="mono text-xs tracking-widest uppercase" style="color: rgba(255,255,255,0.25);" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 100 } } }">
    Bilan & leçons
  </p>

  <!-- On retire l'animation de la grille pour animer les colonnes séparément -->
  <div class="grid grid-cols-2 gap-4" style="width: 680px;">

  <!-- Ce dont on est fiers (Glisse depuis la gauche) -->
  <div class="flex flex-col gap-3 p-5 rounded-xl" style="background: rgba(166,240,211,0.05); border: 1px solid rgba(166,240,211,0.15);"
    v-motion="{ initial: { opacity: 0, x: -20 }, visible: { opacity: 1, x: 0, transition: { duration: 800, delay: 300 } } }">
    <p class="mono text-xs font-bold tracking-widest uppercase" style="color: #A6F0D3;">Ce dont on est fiers</p>
    <ul class="flex flex-col gap-2">
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #A6F0D3; margin-top: 1px;">✓</span> App déployée en production
        </li>
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #A6F0D3; margin-top: 1px;">✓</span> Type-safety end-to-end (Tuyau)
        </li>
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #A6F0D3; margin-top: 1px;">✓</span> Infrastructure pro (Cloudflare · CI/CD)
        </li>
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #A6F0D3; margin-top: 1px;">✓</span> Budget maîtrisé — 42 € total
        </li>
    </ul>
  </div>

  <!-- Ce qu'on referait autrement (Glisse depuis la droite) -->
  <div class="flex flex-col gap-3 p-5 rounded-xl" style="background: rgba(255,35,2,0.04); border: 1px solid rgba(255,35,2,0.15);"
    v-motion="{ initial: { opacity: 0, x: 20 }, visible: { opacity: 1, x: 0, transition: { duration: 800, delay: 500 } } }">
    <p class="mono text-xs font-bold tracking-widest uppercase" style="color: #FF2302;">Ce qu'on referait</p>
    <ul class="flex flex-col gap-2">
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
            <span style="color: #FF2302; margin-top: 1px;">→</span> Partir sur les abstractions natives du framework
        </li>
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #FF2302; margin-top: 1px;">→</span> Définir les conventions Docker dès le départ
        </li>
        <li class="flex items-start gap-2 text-xs" style="color: rgba(255,255,255,0.65);">
          <span style="color: #FF2302; margin-top: 1px;">→</span> Sprint reviews régulières dès le premier mois
        </li>
    </ul>
  </div>

  </div>

  <!-- Footer qui remonte à la fin -->
  <p class="text-xs" style="color: rgba(255,255,255,0.2);" 
     v-motion="{ initial: { opacity: 0, y: 20 }, visible: { opacity: 1, y: 0, transition: { duration: 800, delay: 700 } } }">
    7 mois · v1.0.2 · en production
  </p>

</div>

<!--
NOTES ORATEUR — Slide 11
Le bilan de ces 7 mois est positif.
Ce dont on est le plus fiers : l'app est en production — ce n'est pas un prototype, c'est un vrai produit accessible. On a construit une architecture type-safe de bout en bout grâce à Tuyau, avec une infrastructure sérieuse côté sécurité et déploiement — Cloudflare, GitHub Actions, Docker. Et tout ça pour 42 euros d'hébergement.
Ce qu'on referait différemment : éviter de réimplémenter ce que le framework sait déjà faire, poser les conventions d'infra dès le jour un, et formaliser les sprint reviews pour rester synchronisés en équipe.
Ces leçons, on ne les a pas apprises dans un cours — on les a apprises en les vivant.
-->
