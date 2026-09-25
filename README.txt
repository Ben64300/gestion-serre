GESTION SERRE — V16 SÉCURITÉ & CONFORT

Base : V15 Terrain & Récoltes. Toutes les fonctions V15 sont conservées.

NOUVEAUTÉS V16
- Sauvegarde complète au format JSON enrichi.
- Sauvegarde téléchargeable sur téléphone OU ordinateur.
- Historique local des 10 derniers snapshots dans IndexedDB.
- Snapshot automatique au maximum une fois par 24 h lorsque l'application est ouverte.
- Aperçu avant restauration : date, version et comptages.
- Copie de sécurité automatique juste avant une restauration.
- Restauration complète réservée au propriétaire lorsque la serre partagée est active.
- Reprise du travail après passage dans Chrome :
  * écran courant mémorisé ;
  * position de défilement mémorisée ;
  * fenêtre / formulaire en cours mémorisé ;
  * champs saisis sauvegardés automatiquement.
- Bouton « Rechercher » sur chaque variété :
  * germination ;
  * conseils de culture.
- Correctif de fiabilité de la file de synchronisation pour les suppressions hors ligne.

SAUVEGARDE SUR ORDINATEUR
1. Ouvrir l'adresse habituelle de Gestion Serre sur le PC.
2. Se connecter avec le compte Benoît.
3. Attendre l'indicateur vert « Synchronisé ».
4. Ouvrir Plus → Sauvegardes & restauration.
5. Cliquer « Créer une sauvegarde complète ».
6. Conserver le fichier Gestion_Serre_sauvegarde_....json dans un dossier de sauvegarde du PC.

En cas de téléphone perdu ou cassé, les données synchronisées restent dans Supabase.
La sauvegarde sur ordinateur constitue une protection supplémentaire indépendante de l'appareil mobile.

CONTINUITÉ ANDROID
Android peut suspendre ou fermer une PWA en arrière-plan. V16 ne peut pas empêcher Android de le faire,
mais elle mémorise le travail en cours au fil de la saisie. Au retour dans Gestion Serre, le formulaire et ses champs
sont restaurés automatiquement (hors lecteur QR/caméra).

MISE À JOUR GITHUB PAGES
Remplacer / ajouter les 5 fichiers :
- index.html
- manifest.json
- sw.js
- README.txt
- qr-chambres.pdf

Aucune nouvelle configuration Supabase n'est nécessaire.
