# Stéphane Vatinel — Site web

Site vitrine de Stéphane Vatinel, directeur artistique de territoire et expert tiers-lieux.

## Structure du projet

```
stephane-vatinel/
├── .github/
│   └── workflows/
│       └── deploy.yml      # Déploiement automatique vers Hostinger
├── index.html              # Page principale (ex. stephane-vatinel-v5.html)
├── medias.html             # Page Liens & Médias
└── README.md
```

## Stack technique

- **HTML/CSS/JS pur** — aucune dépendance, aucun framework
- **Fonts** : Libre Baskerville, Caveat, DM Sans (Google Fonts)
- **Hébergement** : Hostinger (hébergement partagé statique)
- **Déploiement** : GitHub Actions → FTP automatique à chaque push sur `main`

## Déploiement

### Première fois

1. Cloner ce repo en local
2. Ajouter les secrets dans GitHub (Settings → Secrets → Actions) :
   - `FTP_HOST` : adresse du serveur FTP Hostinger
   - `FTP_USERNAME` : identifiant FTP Hostinger
   - `FTP_PASSWORD` : mot de passe FTP Hostinger
3. Pusher sur `main` → le site se déploie automatiquement

### Modifier le site

```bash
# Faire les modifications sur index.html ou medias.html
git add .
git commit -m "description du changement"
git push
# → le site se met à jour en 1-2 minutes
```

## Pages

| Page | URL | Description |
|------|-----|-------------|
| Accueil | `/` | Landing page principale avec hero, services, impact, lieux, méthode, contact |
| Médias | `/medias.html` | Presse, podcasts et portfolio des lieux |

## Design system

- **Palette** : Pantone 549C (bleu-gris), 5625C (kaki vert), 500C (rose poudré), 7577C (orange rouille), 559C (menthe), 7734C (forêt profond), 580C (sauge), 460C (ocre)
- **Typo** : Libre Baskerville (titres), Caveat (accents manuscrits), DM Sans (corps)
- **Identité** : Herbier corporate sur papier froissé — illustrations botaniques SVG inline

## Contact

Pour toute modification de contenu, s'adresser à l'agence.
