# Copilot Chantier / Terrops — fiche publique (code privé)

> Dépôt source : **privé** (`copilot-chantier`).  
> Cette page décrit le projet pour un recruteur **sans exposer le code**.

## Contexte

SaaS **assurance construction** (DO / décennale) et app mobile chantier : preuves scellées terrain, contrôles, dossiers sinistre, portails assureur / courtier / backoffice.

## Surfaces

| Surface | URL |
|---------|-----|
| Landing | https://terrops.fr |
| Backoffice | https://app.terrops.fr |
| Mobile web | https://mobile.terrops.fr |
| App Store | https://apps.apple.com/fr/app/terrops/id6770127316 |

## Stack

| Couche | Technologies |
|--------|----------------|
| Mobile | Expo, React Native, Expo Router, WatermelonDB (offline), Sentry |
| Backoffice | TypeScript, React |
| Cloud | **AWS** (eu-west-3) — Cognito, RDS PostgreSQL, Lambda, S3, IAM, Secrets Manager, EventBridge |
| IaC | **Terraform** (`infra/aws-proof-gateway` : network, database, cognito, compute, storage, bootstrap, budget-guard) |
| Preuves | Proof Gateway AWS (upload S3, scellé / TSA) |
| Qualité / CI | GitHub Actions, EAS Build, tests e2e / lint |
| Paiements | Stripe (billing AWS) |

## Périmètre technique

- Auth **Amazon Cognito** (User Pool, JWT, Lambda pre-token)
- Données **RDS PostgreSQL** provisionné Terraform
- API / workers **Lambda** (Function URLs)
- Stockage preuves **S3** + pipeline probatoire
- Infra versionnée **Terraform** (VPC/network, SG, IAM, budgets)

## Résultats

- Produit en production (web + App Store)
- Infra cloud industrialisée (IaC Terraform, pas de console-only)
- Parcours terrain + backoffice sur socle AWS

## Code

**Non public.** Review sous NDA possible.
