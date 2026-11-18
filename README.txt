GESTION SERRE V25 — CORRECTION DE LA SYNCHRONISATION
=================================================

V25 reprend l'interface et toutes les fonctions V24, V23 et V22 :
- Transferts vocaux express « L14 déplace vers S31 » avec confirmation ;
- Correction des ventes, des achats, des notes et recalcul des montants ;
- Inventaire des plantes, récoltes, commandes, voix, NFC, QR et mode hors connexion.

CE QUI A ÉTÉ CORRIGÉ
- Comparaison stable des données indépendamment de l'ordre des clés JSON.
- Arrêt des milliers de réécritures des fiches inchangées.
- Écriture conditionnée par la version Supabase (anti-écrasement à deux appareils).
- Les anciennes opérations en file V24 sont ARCHIVÉES et non renvoyées en masse.
- Les modifications hors ligne passent par la file de synchronisation versionnée.
- Copies de sauvegarde locales avant la première connexion V25.
- Export d'un fichier de diagnostic contenant les opérations héritées et conflits.

IMPORTANT : la correction du logiciel n'est PAS une restauration des mauvais
emplacements actuellement enregistrés. Les déplacements historiques doivent
être réconciliés sans inventer les quantités ni effacer les récoltes.

INSTALLATION MANUELLE SUR GITHUB PAGES
1. Avant de publier, fermer l'application sur PC ET les deux téléphones.
2. Si possible, depuis chaque appareil, sauvegarder en local (sans forcer une
   synchronisation de l'ancienne V24). Ne jamais effacer les données du navigateur.
3. Remplacer index.html, manifest.json, sw.js, README.txt, qr-chambres.pdf
   ensemble à la racine du dépôt Ben64300/gestion-serre.
4. Recharger la nouvelle version sur un appareil connecté à la fois.
5. Vérifier V25 dans Outils et exporter le diagnostic de récupération V24.
6. Confirmer les entrées et les mouvements avant toute restauration.

Un conflit d'écriture ne peut pas être fusionné automatiquement sans savoir
quelle valeur est correcte : il reste conservé localement pour contrôle.
Conserver les sauvegardes pendant toute la période de récupération.
