GESTION SERRE — V15 TERRAIN & RÉCOLTES

Base : V14 Partage & Synchronisation, conservée intégralement.

NOUVEAUTÉS V15
- Accueil « Aujourd’hui dans la serre » avec priorités.
- Bouton flottant + pour les actions les plus fréquentes.
- Mode Terrain dédié.
- Mode Tournée : parcours des chambres, RAS, observation, problème, création facultative de tâche.
- Récoltes : date, culture, chambre, quantité, unité, qualité, notes.
- Bouton Récolte directement depuis une chambre.
- Accès chambre par QR code ou saisie L01 / S01.
- PDF prêt à imprimer : qr-chambres.pdf (116 chambres).
- Vérification intégrée des mises à jour dans Outils.
- Synchronisation de harvests et inspections entre Benoît et Carine.

QR
Les QR contiennent l’URL GitHub Pages avec ?chamber=L01 (ou S01, etc.).
Ils peuvent donc être scannés avec l’appareil photo du téléphone. Gestion Serre accepte également le scan QR depuis le Mode Terrain lorsque BarcodeDetector est disponible.

MISE À JOUR
Pour GitHub Pages, remplacer / ajouter :
- index.html
- manifest.json
- sw.js
- README.txt
- qr-chambres.pdf

Aucune nouvelle configuration Supabase n’est nécessaire : les nouvelles données utilisent la table public.records déjà en place.

IMPORTANT
Faire un export JSON avant toute mise à jour majeure reste une bonne sauvegarde de sécurité.
