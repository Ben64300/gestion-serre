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
