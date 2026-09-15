# ImmoIA / Immolib — fiche publique (code privé)

> Dépôt source : **privé** (`immolib-ia`).  
> Cette page décrit le projet pour un recruteur **sans exposer le code**.

## Contexte

Application web **immobilier** : upload de documents (CNI, titre, DPE…) + mini-CRM parcours vendeur, enrichissement via workflows IA / n8n.

## Rôle & périmètre

- Uploader documents → Supabase Storage (buckets confidentiels)
- Déclenchement workflows **n8n** → enrichissement table `crm_records`
- Mini-CRM (parcours vendeur multi-étapes, fiche dossier, panneau agent)
- Sécurité : clés anon côté client + **RLS** Postgres / policies Storage

## Stack

| Couche | Technologies |
|--------|----------------|
| UI | React 19, Vite, TypeScript / JS, Tailwind, Motion |
| Data | Supabase (Postgres, REST, Storage, Auth) |
| Orchestration | n8n (webhooks HTTP) |
| Docs | pdf-lib |

## Résultats (niveau produit)

- Pipeline document → extraction / enrichissement CRM
- Deux expériences (uploader + CRM) dans un même produit
- Modèle de sécurité orienté RLS (pas de secrets serveur dans le front)

## Code

**Non public**. Spécifications et architecture restent dans le dépôt privé.
