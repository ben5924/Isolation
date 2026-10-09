# Guide des isolants SOBREN

Outil web qui montre aux exploitants quels isolants, et à partir de quelle épaisseur, donnent droit à la prime CEE de l'opération **« Isolation thermique des parois planes ou cylindriques sur des installations industrielles »**, appliquée aux digesteurs de méthanisation.

- Règle appliquée : **R = épaisseur ÷ λ à 50 °C ≥ 2,80 m²·K/W** (cuves et parois de grand diamètre, fluide entre 40 et 100 °C).
- Épaisseurs en vert : éligibles. En rouge : non éligibles.
- Comparaison des isolants à épaisseur égale, fiche par isolant avec contact fabricant.
- Export du catalogue en PDF (bouton « Télécharger le catalogue »).

Tout tient dans un seul fichier : `index.html` (données, logos, photos et code compris).

## Mettre le site en ligne (GitHub Pages)

1. Déposez `index.html` à la racine du dépôt (bouton **Add file → Upload files**).
2. Dans le dépôt : **Settings → Pages**.
3. Sous « Build and deployment », choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une à deux minutes, l'adresse du site s'affiche en haut de la page Pages (du type `https://<compte>.github.io/<dépôt>/`). C'est ce lien que vous envoyez aux clients.

## Mettre à jour le catalogue

Pas besoin de toucher au code.

1. Ouvrez le site en ajoutant `#gestion` à la fin de l'adresse, par exemple `https://<compte>.github.io/<dépôt>/#gestion`.
2. Cliquez sur **Mode gestion**. Vous pouvez :
   - modifier un isolant (bouton **Modifier** dans sa fiche) ou en ajouter un ;
   - changer l'image d'un isolant (bouton **Changer l'image** sur la carte) ;
   - ajouter les logos des fournisseurs (**Logos des fournisseurs**) : ils remplacent le nom de la marque sur le site et dans le PDF ;
   - changer la règle CEE si l'opération évolue (**Réglages CEE** : intitulé de l'opération, seuil R, température du λ) ;
   - exporter les données en CSV pour Excel.
3. Cliquez sur **Télécharger le site à jour (index.html)** en bas de l'écran.
4. Sur GitHub, déposez ce nouveau `index.html` à la place de l'ancien (**Add file → Upload files**, puis **Commit changes**). Le site est à jour une minute plus tard.

Les modifications faites en mode gestion restent dans votre navigateur tant que vous n'avez pas déposé le nouveau fichier : les visiteurs ne les voient pas.

## Bon à savoir

- Le mode gestion n'est pas protégé par un mot de passe, mais il ne modifie rien en ligne : seul le dépôt du fichier sur GitHub change le site.
- Ouvert directement depuis l'ordinateur (double-clic sur `index.html`), le site fonctionne aussi, connexion internet nécessaire pour les polices et l'export PDF.
- Valeurs issues des fiches techniques et déclarations de performance des fabricants. Faites valider chaque dossier par SOBREN et vérifiez la fiche technique en vigueur avant commande.
