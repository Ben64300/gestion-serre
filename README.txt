GESTION SERRE — V19 VOIX & TRANSFERTS

NOUVEAUTÉS V19

1) DÉPLACEMENT ENTRE GROWSTREAM L ET S
- Dans une chambre : sélectionner « ↔ Déplacer » sur la culture concernée.
- Choisir le GrowStream de destination (L ou S), puis la chambre disponible.
- Indiquer un nombre de plants : tout ou partie du lot.
- Vérification des places disponibles avant enregistrement.
- Entre L et S, un nouveau lot lié est créé à destination ; les récoltes déjà saisies restent liées à l'ancien lot et à l'ancienne chambre.
- Le transfert entrant et sortant apparaît dans l'historique de chacune des deux chambres.
- Annuler la dernière modification reste disponible en cas d'erreur.

2) OUVERTURE VOCALE DIRECTE
- Depuis l'accueil, bouton « 🎙️ Ouvrir à la voix » sous la recherche.
- Depuis « Mode terrain », bouton « Ouvrir à la voix » sans lancer de tournée.
- Dire « Ouvre S24 », « L15 », « L quinze », « S vingt-quatre », « S quatre », etc.
- Ouvre la fiche avec les actions Récolte / Ajouter / Déplacer / Modifier.
- La tournée vocale V17 reste fonctionnelle : « RAS », « problème », « observation », « récolte », « suivant » et « précédente ».
- Si le navigateur ne reconnaît pas la voix ou si la 4G est absente, utiliser la recherche et les boutons tactiles ; la reconnaissance en ligne n'est pas garantie hors ligne sur Android.

3) CONSERVATION DES DONNÉES
- Pas de nouvelle table Supabase ni de suppression de données.
- Clé de données locale conservée ; V18 migre automatiquement vers V19.
- V18 Récoltes & Rendements, V17 assistant terrain, NFC/QR, stocks, ventes, sauvegardes, mode offline-first et partage sont conservés.
- Ne pas effacer les données de navigation du navigateur pendant la mise à jour.
- Vérifier que la synchronisation indique 🟢 Synchronisé, puis effectuer une sauvegarde complète avant déploiement.

DÉPLOIEMENT GITHUB PAGES
Remplacer les 5 fichiers à la racine du dépôt : index.html, manifest.json, sw.js, README.txt, qr-chambres.pdf
(Le PDF QR reste inchangé.)
Actualiser l'application avec Internet, la fermer et la rouvrir. Vérifier l'affichage V19 dans Paramètres puis tester une voix et un transfert avec des données de test.

=== HISTORIQUE V18 ===
GESTION SERRE — V18 RÉCOLTES & RENDEMENTS

V18 conserve toutes les fonctions des versions précédentes :
- synchronisation Benoît / Carine via Supabase ;
- offline-first et file de synchronisation ;
- sauvegardes / restauration V16 ;
- assistant vocal, dictée, recherche universelle et journal automatique V17 ;
- QR / NFC, tournée de serre, cultures, chambres, stock, planning, ventes.

NOUVEAUTÉS V18

1. ONGLET « RÉCOLTES » DÉDIÉ
Accès direct depuis la barre principale avec un véritable tableau de bord de production.

2. FILTRES
- Aujourd’hui
- 7 derniers jours
- Ce mois
- Mois précédent
- Cette année
- Toutes les dates
- Période personnalisée
- Variété
- GrowStream
- Chambre
- Classement commercial
- Récolté par Benoît / Carine

3. QUATRE VUES
- Chronologie
- Par variété
- Par chambre
- Par mois

4. CLASSEMENT COMMERCIAL
Chaque récolte peut être classée :
- Commercialisable
- Déclassé
- Perte

La qualité visuelle reste disponible séparément.
Une destination facultative peut être indiquée : vente, transformation, autoconsommation, don, déchet/compost.

5. RENDEMENT
Le formulaire mémorise un nombre de plants de référence.
Le système calcule le rendement en g/plant pour les récoltes au poids.
La fiche culture affiche automatiquement le cumul récolté, le nombre de passages, la première / dernière récolte et le rendement par plant lorsque calculable.

6. GRAPHIQUES
- production en kg par variété ;
- évolution des récoltes dans le temps.
Les grammes sont convertis en kilogrammes.
Les kg ne sont jamais additionnés aux pièces, bottes ou barquettes.

7. MODIFICATION ET EXPORT
Chaque saisie peut désormais être modifiée ou supprimée depuis la chronologie.
Le bouton CSV exporte uniquement les récoltes correspondant aux filtres affichés, pratique pour Excel, la comptabilité ou le suivi DJA.

8. MIGRATION AUTOMATIQUE
Les anciennes récoltes V15/V16/V17 sont conservées.
Si aucun classement commercial n’existait, elles sont classées commercialisables par défaut, sauf ancienne qualité « Déclassée » qui devient « Déclassé ».

MISE À JOUR GITHUB PAGES
Remplacer les 5 fichiers :
- index.html
- manifest.json
- sw.js
- README.txt
- qr-chambres.pdf

Aucune nouvelle table ni nouveau script Supabase n’est nécessaire.
Fermer complètement l’application puis la rouvrir avec Internet après publication.
