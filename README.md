# Reinforced Concrete Studio

Application web de pré-dimensionnement du béton armé, avec huit modules pour les semelles isolées et filantes, les poutres de redressement, poteaux, poutres, dalles pleines et sections en T ou en I. Les rapports détaillent les paramètres saisis, les hypothèses, les vérifications calculées et les schémas.

Les calculs citent le BAEL 91 révisé 99, le DTU 13.12 et le Fascicule 62, titre V. Ces références et formules n'ont pas fait l'objet d'une certification indépendante : les résultats sont indicatifs, ne constituent pas une attestation de conformité et doivent être validés par un ingénieur structure qualifié, avec les textes applicables et les données du projet.

## Développement

```sh
npm install
npm run dev
```

## Vérification

```sh
npm run build
npm run lint
```

## Rapport PDF

Les boutons « Télécharger PDF » génèrent un rapport A4 portrait. Si la génération directe échoue ou si sa bibliothèque n'est pas disponible, l'application ouvre la boîte d'impression du navigateur pour permettre l'enregistrement en PDF.

Le style, le rendu des formules et l'export PDF chargent Tailwind CSS, KaTeX et html2pdf.js depuis des CDN; ces fonctions nécessitent une connexion réseau. L'impression native peut servir de solution de repli.

## Icône

Le pictogramme de bâtiment du logo est adapté de l'icône [building-complex de Lucide](https://lucide.dev/icons/building-complex), publiée sous licence ISC. L'avis de licence est inclus dans `public/favicon.svg`.
