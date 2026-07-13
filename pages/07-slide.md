
<!--
╔══════════════════════════════════════════════╗
║  SLIDE 7 — Architecture & Stack              ║
╚══════════════════════════════════════════════╝
-->

<div class="flex flex-col items-center justify-center gap-6 h-full">

  <p class="mono text-xs tracking-widest uppercase" style="color: rgba(255,255,255,0.25);">Architecture & Stack</p>

  <!-- Diagramme en couches -->
  <div class="flex flex-col items-center gap-0" style="width: 580px;">

  <!-- Cloudflare -->
  <div class="w-full px-6 py-0 text-center rounded-xl" style="background: rgba(249,130,0,0.08); border: 1px solid rgba(249,130,0,0.3);">
    <p class="mono text-xs font-bold tracking-widest uppercase mb-1" style="color: rgba(249,130,0,0.7);">Cloudflare</p>
    <p class="text-xs" style="color: rgba(255,255,255,0.4);">WAF · CDN · Protection DDoS</p>
  </div>
  
  <div class="flex flex-col items-center py-1" style="color: rgba(255,255,255,0.15);">
    <div style="width:1px; height:14px; background: rgba(255,255,255,0.12);"></div>
    <span style="font-size:9px;">▼</span>
  </div>
  
  <!-- Frontend -->
  <div class="w-full px-6 py-0 text-center rounded-xl" style="background: rgba(166,240,211,0.06); border: 1px solid rgba(166,240,211,0.2);">
    <p class="mono text-xs font-bold tracking-widest uppercase mb-1" style="color: rgba(166,240,211,0.6);">Frontend</p>
    <p class="text-xs" style="color: rgba(255,255,255,0.5);">Nuxt 4 · Vue 3 · Pinia · @nuxt/ui · Tailwind CSS v4</p>
  </div>
  
  <div class="flex flex-col items-center py-1">
    <div style="width:1px; height:14px; background: rgba(255,255,255,0.12);"></div>
    <span style="font-size:9px; color: rgba(255,255,255,0.15);">▼</span>
  </div>
  
  <!-- Backend -->
  <div class="w-full px-6 py-0 text-center rounded-xl" style="background: rgba(166,240,211,0.06); border: 1px solid rgba(166,240,211,0.2);">
    <p class="mono text-xs font-bold tracking-widest uppercase mb-1" style="color: rgba(166,240,211,0.6);">Backend</p>
    <p class="text-xs" style="color: rgba(255,255,255,0.5);">AdonisJS 7 · TypeScript · Node.js 24 · Tuyau · VineJS</p>
  </div>
  
  <div class="flex flex-col items-center py-1">
   <div style="width:1px; height:14px; background: rgba(255,255,255,0.12);"></div>
   <span style="font-size:9px; color: rgba(255,255,255,0.15);">▼</span>
  </div>
  
  <!-- Base de données -->
  <div class="w-full px-6 py-0 text-center rounded-xl" style="background: rgba(166,240,211,0.06); border: 1px solid rgba(166,240,211,0.2);">
    <p class="mono text-xs font-bold tracking-widest uppercase mb-1" style="color: rgba(166,240,211,0.6);">Base de données</p>
    <p class="text-xs" style="color: rgba(255,255,255,0.5);">PostgreSQL 15 · Lucid ORM · ULID</p>
  </div>

</div>

  <!-- Pastilles infra + outillage -->
  <div class="flex gap-4 mt-2">
    <div class="card px-4 py-2 text-center">
      <p class="mono text-xs" style="color: rgba(255,255,255,0.35);">Hetzner VPS · Docker Compose · Certbot SSL</p>
    </div>
    <div class="card px-4 py-2 text-center">
      <p class="mono text-xs" style="color: rgba(255,255,255,0.35);">Turborepo · GitHub Actions · oxlint</p>
    </div>
  </div>

</div>

<!--
NOTES ORATEUR — Slide 7
On a construit Gitify sur un monorepo pnpm avec Turborepo pour gérer le build de manière efficace.
En frontal, Cloudflare fait office de bouclier : WAF, CDN, et protection contre les attaques DDoS.
Le frontend c'est Nuxt 4 avec Vue 3 — on a choisi @nuxt/ui pour les composants et Tailwind v4 pour le style, cohérent avec le design system de l'app.
Le backend est en AdonisJS 7, un framework Node.js TypeScript-first. On a utilisé Tuyau pour générer automatiquement un client HTTP type-safe partagé entre le front et le back — plus de désynchronisation entre les types.
En base de données, PostgreSQL 15 avec l'ORM Lucid natif d'Adonis, et des identifiants ULID plutôt qu'auto-incrémentés pour plus de robustesse en environnement distribué.
Côté infra : un VPS Hetzner, Docker Compose pour orchestrer les containers, et Certbot pour le SSL.
-->
