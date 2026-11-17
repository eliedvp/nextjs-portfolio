# Portfolio Next.js (première version, abandonnée)

> **Dépôt archivé.** Ce prototype n'a pas été terminé : seules la page d'accueil et la navigation sont réalisées. Il a été remplacé par mon portfolio actuel, en ligne sur https://eliedvp.vercel.app. Les dépendances ne sont plus maintenues (Next.js 15.5.6 fait l'objet d'avis de sécurité) : ne pas déployer ce code en l'état.

Première version d'un portfolio personnel de développeur, construite avec Next.js (App Router), Tailwind CSS et Framer Motion.

Mon portfolio actuel est en ligne sur https://eliedvp.vercel.app.

## État du projet

- **Page d'accueil réalisée** : présentation, titre animé (« web Developer » / « DEVELOPPEUR FULL STACK »), coordonnées, icônes de réseaux sociaux, motif et forme décoratifs (blob).
- **Navigation** : menu latéral sur grand écran et menu mobile (composant `Sheet` de shadcn/ui, basé sur Radix UI), lien actif selon la route.
- **Transitions** : animations d'apparition et de changement de page avec Framer Motion.
- **Pages À propos, Services, Travaux et Contact** : routes créées, contenu pas encore rédigé.

## Stack

- Next.js 15 (App Router) et React 19
- Tailwind CSS 4
- Framer Motion, react-type-animation
- shadcn/ui (Radix UI Dialog), react-icons, lucide-react
- Police Sometype Mono via `next/font`

## Structure

```
app/          routes : /, /about, /services, /work, /contact
components/   en-tête, navigation, transitions, éléments décoratifs
components/ui composant Sheet (shadcn/ui)
public/assets images (blobs, services, vignettes de projets)
```

## Lancer le projet

```bash
npm install
npm run dev
```

Puis ouvrir http://localhost:3000.

Build de production :

```bash
npm run build
npm start
```
