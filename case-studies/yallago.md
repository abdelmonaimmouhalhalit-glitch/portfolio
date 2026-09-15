# YallaGo — fiche publique (code privé)

> Dépôts source : **privés** (`YallaGo-api`, `YallaGo-front`).  
> Cette page décrit le projet pour un recruteur **sans exposer le code**.

## Contexte

Plateforme de **location de véhicules / agences** (multi-tenant) : réservations, contrats, paiements, parc véhicules.

## Architecture

- **API** : Java 21, Spring Boot (Web, Data JPA, Security, Validation)
- **Front** : Angular 18, Angular Material, OAuth2 / OIDC, Google Maps
- **Données** : PostgreSQL (+ H2 en local)
- **Intégrations** : Stripe, JWT, OpenAPI / springdoc, Docker, GitHub Actions
- Domaine : Tenant, Agence, Véhicule, Réservation, Contrat, Client, Paiement, Rôles…

## Stack

```
YallaGo-api    Spring Boot · JPA · Security · JWT · Stripe · PostgreSQL · Docker · OpenAPI
YallaGo-front  Angular 18 · Material · OAuth2-OIDC · Google Maps · SCSS · Docker
```

## Résultats (niveau produit)

- API REST sécurisée multi-entité métier
- Front responsive généré / aligné OpenAPI
- Pipeline CI GitHub Actions

## Code

**Non public** (les deux dépôts restent privés).
