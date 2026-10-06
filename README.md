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
