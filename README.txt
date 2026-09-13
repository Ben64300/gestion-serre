GESTION SERRE — V14 PARTAGE & SYNCHRONISATION

Cette version est construite sur la V13 Consolidée.

SUPABASE
- Projet : Gestion-serre
- URL configurée dans l'application : https://zoewrjylrvkejdtkmkla.supabase.co
- La clé intégrée est la clé PUBLIABLE uniquement.
- Les données sont protégées côté base par Supabase Auth + RLS.

UTILISATION PARTAGÉE
- Benoît et Carine ont chacun leur propre compte.
- Les deux comptes utilisent la même « Serre principale ».
- Benoît est propriétaire ; Carine est membre.
- Les données communes sont stockées dans public.records.

MODE HORS CONNEXION
- L'application reste utilisable lorsque la 4G disparaît.
- Les données restent immédiatement enregistrées sur le téléphone.
- IndexedDB conserve la file des modifications à synchroniser.
- Lorsque le réseau revient, l'application synchronise automatiquement.
- Une synchronisation automatique est également tentée toutes les 20 secondes lorsque l'application est ouverte et connectée.
- Un bouton de synchronisation manuelle reste disponible dans Outils.

PREMIÈRE MIGRATION
1. Installer / ouvrir la V14 sur le téléphone de Benoît.
2. Se connecter avec le compte Benoît.
3. Ouvrir Outils → Partage & synchronisation.
4. Si la base partagée est vide, appuyer sur « Envoyer les données de ce téléphone ».
5. Attendre l'indicateur vert « Synchronisé ».
6. Ouvrir ensuite la même adresse GitHub Pages sur le téléphone de Carine.
7. Installer Gestion Serre et se connecter avec le compte Carine.
8. Les données de la Serre principale sont alors téléchargées automatiquement.

TÂCHES
- Responsable : Benoît, Carine ou Tous.
- Statut : À faire, En cours ou Terminée.
- Les cartes de tâches indiquent le responsable et, après synchronisation, le dernier utilisateur ayant modifié la tâche.

JOURNAL
- Outils → Activité partagée affiche les dernières opérations synchronisées et leur auteur.

INDICATEURS
- 🟢 Synchronisé
- 🟡 Modifications en attente / initialisation
- 🔵 Synchronisation en cours
- 🔴 Hors connexion
- ⚪ Connexion requise

SAUVEGARDE
L'export/import JSON reste disponible en complément de la synchronisation cloud.
