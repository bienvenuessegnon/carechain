# CareChain

Prototype d'application d'épargne santé, de campagnes de financement d'urgence, de cercles familiaux et de paiement en Bitcoin (Lightning ou on-chain). Interface React, état local (données de démonstration).

*A React prototype for health savings, emergency campaigns, family circles and Bitcoin payments.*

**Démo :** [https://carechain-ten.vercel.app](https://carechain-ten.vercel.app)

Le titre affiché sur la démo est encore le titre technique d'origine de l'application. Le dépôt n'est pas une version de [Santé+ Bénin](https://github.com/bienvenuessegnon/santeplusbj) : le concept se rapproche (santé et paiements Bitcoin), les écrans sont différents.

## Fonctionnalités (prototype)

- authentification et profil
- vérification d'identité (KYC), avec un espace d'administration pour valider ou refuser un dossier
- objectifs d'épargne santé
- campagnes d'urgence et dons
- cercle familial (membres, alertes, soutien)
- historique de transactions (dépôt, retrait, don, paiement)
- assistant conversationnel (clé `GEMINI_API_KEY` optionnelle)
- indications de dépenses prévues, à titre illustratif

Les parcours tournent avec des données simulées côté client (Zustand). Ce n'est pas un service de paiement réel.

## Stack

React, TypeScript, Vite, Tailwind CSS, React Router, Zustand, Recharts, Zod.

## Lancer le projet

Prérequis : Node.js.

```bash
cp .env.example .env
npm install
npm run dev
```

L'application est servie sur [http://localhost:3000](http://localhost:3000).

## Structure

```text
src/pages/     accueil, authentification, tableau de bord, épargne, campagnes,
               cercle familial, paiement, KYC, administration, assistant
src/store/     état de l'application
src/components/
```

## Auteur

[Bienvenu ESSEGNON](https://github.com/bienvenuessegnon)
