GESTION SERRE — V17 ASSISTANT TERRAIN

V17 conserve intégralement V16 :
- Supabase partagé Benoît / Carine
- fonctionnement offline-first
- file de synchronisation
- sauvegardes et restauration
- snapshots locaux
- reprise des brouillons après passage dans Chrome
- cultures, chambres GrowStream, planning, stock, ventes, récoltes, QR codes et tournée.

NOUVEAUTÉS V17

1. ASSISTANT VOCAL TERRAIN
Pendant une tournée, toucher « Écouter » puis dire par exemple :
- « RAS »
- « problème pucerons sur trois plants »
- « problème feuilles jaunes créer une tâche demain »
- « observation début de floraison »
- « récolte 2 kilos 400 »
- « suivant »
- « précédente »

Le système reste push-to-talk : il n'écoute jamais en permanence.
Les boutons tactiles restent toujours disponibles.
La compatibilité de reconnaissance vocale dépend du navigateur Android et peut nécessiter une connexion réseau.

2. DICTÉE DANS LES FORMULAIRES
Les zones de notes / observations affichent automatiquement un bouton « Dicter » lorsque le navigateur prend la reconnaissance vocale en charge.

3. CONFIRMATION
Une vibration confirme les commandes.
Une confirmation vocale peut être activée ou désactivée dans Mode terrain.

4. RECHERCHE UNIVERSELLE
Depuis l'accueil, une seule recherche retrouve :
- chambres (L17, S04...)
- variétés
- cultures
- tâches
- stock
- récoltes.

5. JOURNAL AUTOMATIQUE
Le tableau de bord construit le journal du jour à partir des opérations enregistrées :
- contrôles RAS
- observations et problèmes
- récoltes
- tâches terminées
- ventes.
Le journal peut être copié en texte pour archivage ou transmission.

6. FIABILITÉ
Aucune nouvelle table Supabase n'est requise.
Les nouvelles fonctions utilisent les données déjà synchronisées.
Les commandes vocales ne remplacent jamais les contrôles manuels.

MISE À JOUR GITHUB PAGES
Remplacer les 5 fichiers :
- index.html
- manifest.json
- sw.js
- README.txt
- qr-chambres.pdf

Après publication :
- fermer complètement Gestion Serre ;
- la rouvrir avec Internet ;
- autoriser le microphone au premier essai vocal.
Carine reçoit la même V17 en fermant / rouvrant son application.
