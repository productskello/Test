# Prototypes Skello

## affiner-shifts-penibles/

Prototype interactif « Affiner les shifts pénibles » (paramètres Planification → Règles et critères), repris de l'artefact
https://claude.ai/artifact/KvbyAyzjTnsk1QU333LRMo

- `index.html` : deux vues, avec navigation par la barre Skello
  - **Planning** (`#planning`, vue par défaut) : planning semaine. Le bouton « Assigner automatiquement » (icône Beta de la barre d'outils) ouvre la modale « Assigner les shifts automatiquement » ; son bouton « Affiner » ouvre la modale « Affiner les shifts pénibles ». Au survol d'un shift, la carte d'aperçu affiche « Shift pénible : … » selon les réglages enregistrés dans « Affiner ».
  - **Paramètres** (`#parametres`, roue crantée) : Planification → Règles et critères, avec la même modale « Affiner »
  - Figma : nœuds `39575:416252` (modale AA) et `39576:434258` (survol d'un shift) du fichier ⚙️ Settings shop
- `skello-kit.js` : kit Skello (police Gellix, tokens Orora, composants, élément `sk-icon`)

Pour l'ouvrir : ouvrir `affiner-shifts-penibles/index.html` dans un navigateur (aucune dépendance externe).

## custom-rules-phase-2/

Prototype interactif « Custom Rules phase 2 » : la section Figma `39444:195291` du fichier ⚙️ Settings shop (9 écrans).

- `index.html` : même base que `affiner-shifts-penibles/` (planning `#planning`, paramètres `#parametres`)
  - **Modale AA** : le critère « Favoriser l’équité des postes et horaires pénibles » est décoché par défaut ; une fois coché, le bouton « Affiner » apparaît
  - **« Affiner »** ouvre une modale en 2 étapes avec barre de progression : Étape 1/2 « Affiner les jours et horaires pénibles » (période « Semaine actuelle » / « 4 dernières semaines », exceptions par employé, volontaires), puis Étape 2/2 « Définir les postes pénibles ». Boutons « Précédent », « Valider et continuer », « Valider et terminer »
  - **Survol d’un shift** : « Shift pénible : ouverture » (et le poste, s’il est défini comme pénible)
  - **Paramètres** : Planification automatique → Règles et critères, info-bulle sur « Critères d’optimisations »
- `skello-kit.js` : copie du kit Skello
