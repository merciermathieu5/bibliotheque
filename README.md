# Bibliothèque

Catalogue public de la bibliothèque de classe de M. Univers social : mangas, bandes dessinées, romans graphiques et ouvrages de référence.

On peut y chercher une œuvre par titre, auteur, sujet ou ISBN, puis filtrer par type, période historique, lien au programme, sujet ou disponibilité.

## Contenu du dépôt

- `index.html` : l'application, qui sert à la fois de page pour les élèves et de gestion.
- `catalogue.json` : le catalogue publié pour les élèves, sans noms d'emprunteurs ni notes.
- `couvertures/` : les images des couvertures.
- `admin/` : raccourci vers la gestion.

## Gestion

La gestion se fait en ligne, à l'adresse https://merciermathieu5.github.io/bibliotheque/admin/, avec un jeton d'accès personnel GitHub à accès précis (fine-grained). Le jeton doit avoir le droit « Contents : Read and write » sur ce dépôt et sur le dépôt privé `bibliotheque-donnees`.

- Les fiches complètes, les notes et les prêts sont enregistrés dans le dépôt privé `bibliotheque-donnees`.
- Le fichier `catalogue.json` est republié automatiquement après les changements, au plus une fois toutes les 5 minutes, ou tout de suite avec « Publier maintenant ».
- Les couvertures ajoutées depuis la gestion sont déposées dans `couvertures/`.

Le jeton reste dans le navigateur qui l'utilise. Il n'est jamais publié.

Les couvertures proviennent du site Les libraires, d'Open Library, d'Amazon et de la Fondation Azrieli. Elles servent uniquement à reconnaître les livres de la classe.
