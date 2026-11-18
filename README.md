# Yellow Jacket · Cédric Doumbé × Jake Paul

Site statique bilingue (français / anglais) : « La négociation annuelle » et le « Vestiaire ».
Aucune dépendance, aucun build : des fichiers HTML, un script d'images et une photo.

**Démo :** https://VOTRE-UTILISATEUR.github.io/Yellow_Jacket_FR_EN/

## Structure

```
index.html          Choix de la langue (mémorisé dans localStorage, redirection auto)
fr/index.html       Version française — La négociation annuelle
fr/atelier.html     Version française — Vestiaire
en/index.html       English version — The Annual Pay Talks
en/atelier.html     English version — Locker Room
assets/art.js       Images encodées (webp, base64)
assets/faceoff.jpg  Visuel de la page d'accueil
```

## Liens directs

| URL | Effet |
|-----|-------|
| `index.html?lang=fr` | Ouvre directement la version française |
| `index.html?lang=en&view=atelier` | Ouvre directement le vestiaire en anglais |

## Lancer en local

Ouvrir `index.html` dans un navigateur, ou servir le dossier :

```
python -m http.server 8000
```

puis aller sur http://localhost:8000/

## Déploiement GitHub Pages

Le site est servi tel quel depuis la branche `main` (racine).
Le fichier `.nojekyll` désactive le traitement Jekyll.
