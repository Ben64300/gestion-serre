GESTION SERRE — V11 CONSOLIDÉE

Cette version remplace la V11 précédente et devient la nouvelle base de référence.

Objectifs de la consolidation :
- un seul modèle de données cohérent ;
- suppression des fonctions dupliquées accumulées au fil des V1 à V10 ;
- migration automatique des données existantes ;
- même clé de stockage locale : gestion_serre_v1 ;
- version interne de base : schemaVersion 11 ;
- contrôles de capacité des chambres ;
- code organisé par modules logiques dans un seul fichier, sans dépendance externe.

Fonctions incluses :
- tableau de bord, actions rapides et heure de sauvegarde ;
- navigation Android avec retour vers l'écran précédent ;
- GrowStreamPro L1120 : L01-L28 / L29-L56 ;
- GrowStreamPro S1200 : S01-S30 / S31-S60 ;
- 20 emplacements par chambre ;
- libre / en attente (jaune) / partielle (vert) / complète (rouge) ;
- plusieurs cultures par chambre dans la limite disponible ;
- ajout, retrait, déplacement, réservation, libération et modification ;
- historique de chambre lors d'une libération ou fin de culture ;
- recherche et filtres des cultures ;
- planning ;
- stock avancé : catégorie, variété, fournisseur, lot, taux/date de germination,
  seuil d'alerte et historique des mouvements ;
- ventes, coûts et marge ;
- variétés classées par espèce/catégorie puis par variété ;
- ajout/modification/suppression sécurisée des variétés ;
- export/import JSON ;
- annulation de la dernière modification.

Mise à jour GitHub :
Remplacer index.html, manifest.json, sw.js et README.txt dans le dépôt.
Fermer complètement l'application puis la rouvrir.
