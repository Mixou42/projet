# Site 1BCT prêt pour Netlify + Decap CMS

Ce dossier contient une version prête à publier de ton site.

## Structure

- `index.html` : le site visible par les visiteurs.
- `admin/index.html` : l'interface Decap CMS disponible à `/admin`.
- `admin/config.yml` : la configuration de Decap CMS.
- `content/page.json` : le titre, les boutons, les images principales et le footer.
- `content/info-sections.json` : les cases d'information modifiables depuis l'admin.
- `content/cards.json` : les cartes du jeu modifiables depuis l'admin.
- `images/uploads/` : dossier où Decap CMS mettra les images envoyées depuis l'admin.

## Étape obligatoire avant publication

Dans `admin/config.yml`, remplace cette ligne :

```yml
repo: TON-PSEUDO-GITHUB/TON-NOM-DE-REPO
```

par ton vrai dépôt GitHub. Exemple :

```yml
repo: mixdubus/mon-site-1bct
```

Le compte GitHub utilisé dans l'admin doit avoir le droit de modifier le dépôt.

## Mise en ligne rapide

1. Crée un dépôt GitHub.
2. Envoie tout le contenu de ce dossier dans le dépôt.
3. Sur Netlify, fais "Add new site" puis "Import existing project".
4. Choisis ton dépôt GitHub.
5. Laisse "Build command" vide.
6. Mets "Publish directory" sur `.`.
7. Publie le site.
8. Va sur `https://ton-site.netlify.app/admin`.

## Important

Le site charge d'abord les fichiers JSON dans `content/`. Si un problème arrive, il garde une version intégrée de secours dans `index.html`.
