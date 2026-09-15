# Copilot Chantier — fiche publique (code privé)

> Dépôt source : **privé** (`copilot-chantier`).  
> Cette page décrit le projet pour un recruteur **sans exposer le code**.

## Contexte

SaaS / application mobile **BTP urbain** : coordination terrain, preuves d’intervention, conformité (ZFE, accès livreurs), backoffice exécutif.

## Rôle & périmètre

- App mobile terrain (Expo / React Native)
- Backoffice org-admin (TypeScript / React)
- Backend données : Supabase (Postgres, RLS, Edge Functions, Storage)
- CI/CD : GitHub Actions, EAS Build (iOS production)
- Modules : interventions, QR d’accès livreur + SMS, contrôles ZFE, incidents, apporteurs d’affaires, valeur probatoire (GPS + horodatage)

## Stack

| Couche | Technologies |
|--------|----------------|
| Mobile | Expo, React Native, Expo Router, Sentry |
| Offline | WatermelonDB |
| Backend | Supabase, PostgreSQL, Edge Functions, RLS |
| Qualité | ESLint, tests, workflows e2e / regression / lint |
| Ops | EAS, GitHub Actions |

## Résultats (niveau produit)

- Parcours terrain + backoffice sur un même socle données
- Preuves d’intervention (GPS, timestamps) orientées usage professionnel
- Automatisations métier (ZFE, QR accès, commissions apporteurs)

## Code

**Non public** (propriétaire / mission). Demande de review sous NDA possible.
