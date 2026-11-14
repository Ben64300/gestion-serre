GESTION SERRE — V24 : MODIFICATION DES VENTES ET DES ACHATS / COÛTS
===================================================================

NOUVEAUTÉS
- Dans « Ventes », bouton « ✏️ Modifier » à côté de chaque vente et de chaque achat / coût.
- Réouverture de toutes les données : date, produit/libellé, quantité, unité, prix, client, variété, bloc.
- Champ « Notes / précisions » pour les ventes et les achats : texte affiché dans l’historique et modifiable.
- Les modifications mettent à jour l’enregistrement original (même identifiant), sans doublon.
- Le total d’une vente et les indicateurs du mois sont recalculés après correction.
- Les anciennes ventes et dépenses restent compatibles ; elles s'ouvrent avec des notes vides.
- Sauvegarde locale avec annulation possible, comme pour les autres modifications.
- La synchronisation Supabase utilise les collections existantes (ventes, coûts) et conserve le mode hors connexion.
- Les améliorations V23 (transfert vocal express) et V22 (inventaire vivant) restent incluses.

INSTALLATION
1. Vérifiez la synchronisation sur chaque téléphone et créez une sauvegarde depuis « Outils ».
2. Dans le dépôt GitHub Pages, remplacez les 5 fichiers : index.html, manifest.json, sw.js,
   README.txt et qr-chambres.pdf (fichier QR inchangé).
3. Actualisez/réouvrez l’application avec la connexion activée jusqu'à l'affichage de « V24 ».
4. Dans « Ventes », ouvrez « ✏️ Modifier » sur une vente passée, corrigez une note et enregistrez.
5. Vérifiez l'absence de doublon et le maintien de la correction après redémarrage puis synchronisation.
6. Répétez le test sur un coût / achat, puis sur l'autre téléphone.

IMPORTANT
Un achat enregistré comme mouvement de stock est distinct d'un coût dans l'onglet « Ventes ».
Les fiches de stock ont déjà leur propre bouton « Modifier ».
Évitez de corriger simultanément le même enregistrement depuis deux téléphones hors ligne.

GESTION SERRE — V23 : TRANSFERT VOCAL EXPRESS (1 PLANT)
===================================================

NOUVEAUTÉ PRINCIPALE
- Dites simplement : « L14 déplace vers S31 ».
- Fonctionne aussi avec « déplace L14 vers S31 » et « L quatorze déplace vers S trente-et-un ».
- Par défaut, UN SEUL plant est sélectionné pour ce raccourci, même si la chambre en contient plusieurs d'une seule culture.
- Le nom de la variété n'a pas besoin d'être dicté si une seule culture occupe la chambre source.
- L'application ouvre la fenêtre de transfert, avec le départ, la destination et la quantité (1) préremplis.
- VÉRIFIEZ LA PROPOSITION ET APPUYEZ SUR « Confirmer le déplacement ».
- La voix ne déclenche aucun déplacement définitif sans cette confirmation.
- La commande complète reste disponible : « déplace 5 plants de S24 vers L14 ».
- Le raccourci fonctionne avec l'assistant vocal de l'Accueil, du Terrain, et pendant la tournée.

CONTRÔLES DE SÉCURITÉ
- Si la chambre source comporte plusieurs cultures ou lots, l'application n'en choisit aucun automatiquement.
- Si la chambre de destination est pleine, la préparation est refusée.
- Impossible de déplacer vers sa propre chambre ni de retirer plus de plants qu'il n'en existe.
- Les transferts entre GrowStream L et S conservent le suivi des lots et les historiques.
- Les quantités dans l'inventaire V22 se mettent à jour après confirmation du transfert.
- La reconnaissance vocale dépend du navigateur ; elle peut nécessiter la 4G.

INSTALLATION
1. Sur les deux téléphones, vérifier la synchronisation puis effectuer une sauvegarde dans Outils.
2. Dans le dépôt GitHub Pages, remplacer les 5 fichiers de l'application : index.html, manifest.json,
   sw.js, README.txt et qr-chambres.pdf.
3. Relancer l'application sur les deux téléphones, et vérifier que la version V23 est affichée.
4. Essayer « L14 déplace vers S31 » sur une chambre avec une seule culture, vérifier le formulaire et
   confirmer ou annuler. Tester ensuite avec une chambre contenant plusieurs cultures.
5. Éviter les modifications simultanées hors ligne du même lot depuis deux téléphones jusqu'à la synchronisation.

GESTION SERRE — V22 : INVENTAIRE VIVANT ET POINTAGE DES PLANTS
===========================================================

CE QUI CHANGE
- Accueil : nombre global de plants présents dans les systèmes, avec accès au pointage.
- Serre & cultures : inventaire de tous les plants actifs, classés par espèce et variété.
- Exemple : total de laitues, détail Suzanne / Merveille d’hiver, chou-rave Azure Star, chou frisé rouge.
- Agrégation sur tous les GrowStream et toutes les chambres, même pour plusieurs lots de la même variété.
- Les plants en attente et les cultures terminées ne sont pas comptés comme « présents ».
- Tout ajout, retrait, déplacement de culture ou changement de statut actualise les totaux automatiquement.
- Pointer / Corriger : compte réel de chaque chambre, ajustable sans saisir un total isolé incohérent.
- Contrôle de la capacité physique des chambres avant toute correction.
- Filtres système, espèce/variété, semaine, année ou plage de dates de mise en système.
  IMPORTANT : un filtre de date sélectionne les lots actifs plantés pendant la période ;
  il ne reconstitue PAS l’inventaire à une date passée.
- Export CSV de l’inventaire affiché.
- Toutes les nouveautés V21 et précédentes sont conservées.

INSTALLATION SUR LES DEUX TÉLÉPHONES
1. Sur chaque téléphone, attendez la mention « Synchronisé », puis créez une sauvegarde complète dans Outils.
2. Remplacez les CINQ fichiers du dépôt GitHub Pages : index.html, sw.js, manifest.json,
   README.txt, qr-chambres.pdf. Ne remplacez pas uniquement le HTML.
3. Faites relancer l’application aux deux personnes avec la connexion disponible.
4. Vérifiez « V22 » dans Outils et comparez le premier total avec le comptage réel.
5. Contrôlez une variété dans plusieurs chambres, corrigez une chambre, puis vérifiez
   le nouveau total sur chaque téléphone après synchronisation.
6. En cas d’écart de données entre téléphones, n’effectuez pas simultanément deux corrections
   hors ligne sur le même lot : la dernière modification synchronisée peut remplacer l’autre.

PRÉCISION
La saisie d’une récolte (poids, bottes ou pièces) n’indique pas nécessairement
que le plant entier est retiré. Pour décrémenter l’inventaire, utilisez « Retirer des plants »,
« Terminer la culture » ou « Pointer / Corriger » selon la situation.

GESTION SERRE — V21 UNIFIÉE (V20 + V21 + V22 regroupées)
=============================================

NOUVEAUTÉS V21

1. DEMANDES CLIENTS — SAISIE EN RENDEZ-VOUS
- Depuis Accueil : « Noter une demande client » ; depuis le bouton + ; ou Ventes.
- Client, date, statut « À confirmer » ou « Confirmée », produits, quantité et unité.
- Ajoutez autant de produits que nécessaire, sans créer une vente.
- Pour chaque produit, le volet « Disponibilité vérifiée » permet (facultativement) de noter la quantité disponible et le manque ; rien n’est inventé si la quantité est inconnue.
- « Nouvelle demande » à partir d’une fiche reprend le restaurant, les produits et les quantités demandées, mais réinitialise les disponibilités périmées.
- Bouton micro à côté de chaque ligne : « 1 kilo de persil », « 500 grammes de mizuna », « quatre bottes de cerfeuil ».
- Exemple « Cabeillou » : préremplit 1 kg persil, 500 g mizuna pourpre et 4 bottes de cerfeuil, MAIS NE L'ENREGISTRE PAS sans validation.
- Les demandes à confirmer restent distinctes des commandes fermes et des ventes comptabilisées.
- Les besoins hebdomadaires sont un indicateur de fréquence, sans création automatique de commande.

2. TERRAIN INTELLIGENT
- Accueil : chambres favorites et cinq dernières chambres ouvertes sur cet appareil.
- Chaque chambre : Favori, Précédente, Suivante, Replanter, Photo.
- Replanter : propose une variété déjà présente ou historiquement cultivée dans la chambre ; crée un nouveau lot sans altérer l'ancien.
- Commande vocale sur Accueil et Terrain : ouverture de chambre, préparation de récolte ou transfert, ouverture de demande client ou relevé bassin.
- AUCUNE récolte ni déplacement n'est validé automatiquement par la voix : confirmation manuelle indispensable.
- La tournée vocale V17 et les transferts inter-systèmes V19 restent disponibles.

3. SUIVI BASSIN
- Saisir date, heure, pH, EC (mS/cm), température de l'eau, eau ajoutée et notes d'engrais.
- Dernier relevé sur l'Accueil et le Terrain ; historique dans Outils.
- Alertes visuelles selon des seuils modifiables (valeurs initiales : pH 5,5–6,5 ; EC 1,0–2,0).
- Alerte aussi si variation de pH d'au moins 0,4 entre deux relevés.
- Les seuils sont des repères de suivi à adapter aux cultures, pas des recommandations universelles.

4. PHOTOS DE CULTURES
- Depuis une chambre : « Photo » ouvre l'appareil photo ou la galerie Android.
- L'image est réduite à 480 px et environ 65 000 caractères pour ménager le stockage et la 4G.
- Photos, dates et observations sont incluses dans les sauvegardes et les enregistrements partagés.
- Limite de 25 photos au total pour éviter l'épuisement de la mémoire locale.
- Galerie consultable dans « Outils » ; supprimer les anciennes photos selon vos besoins.

5. PRÉVISIONS DE RÉCOLTE
- L'Accueil présente les cultures ayant une date de récolte prévue OU un nombre de jours avant récolte renseigné dans la fiche variété.
- Un coefficient saisonnier tient compte grossièrement de l'absence de chauffage sous serre.
- La fenêtre est INDICATIVE et ne remplace pas l'observation et le suivi réel de croissance.
- Aucune quantité vendable n'est inventée.

6. CONFORT & SÉCURITÉ
- Date locale utilisée au lieu de la date UTC (évite la veille juste après minuit en France).
- Aucun nouvel onglet de navigation principale.
- Les historiques et fonctions V18/V19 restent présents (cultures, récoltes, NFC, QR, stocks, planning, ventes, sauvegardes et synchronisation).
- Nouvelles catégories de données synchronisées dans la table générique « records » de Supabase : client_request, water_reading, crop_photo. Aucune migration SQL.

IMPORTANT AVANT D'INSTALLER
==========================
1. À partir de la V19, sur les deux téléphones, attendez l'indication 🟢 Synchronisé.
2. Effectuez une sauvegarde complète (Outils > Sauvegardes).
3. Mettez à jour LES DEUX téléphones (Benoît et Carine) vers la V21 avant de saisir les nouvelles fiches.
   Ne continuez pas à utiliser V19 sur l'autre téléphone avec les nouvelles données V21 : une ancienne version ne connaît pas les nouvelles catégories et pourrait les effacer lors d'une synchronisation.
4. Sur GitHub Pages, remplacez ces cinq fichiers : index.html, manifest.json, sw.js, README.txt et qr-chambres.pdf.
5. Fermez complètement les deux applications, relancez avec Internet et vérifiez la présence de « V21 unifiée » dans Outils.
6. Testez sur une DEMANDE FICTIVE, puis vérifiez sa synchronisation entre les deux téléphones, et supprimez-la.
7. Vérifiez également le microphone avec Chrome sur Android. La reconnaissance vocale peut nécessiter une connexion Internet.

LIMITES CONNUES
- Les favoris, derniers codes ouverts et seuils d'alerte personnalisés sont propres à chaque téléphone (préférences locales).
- Les images sont partagées sous forme de miniatures compressées, pas en résolution originale ; qualité insuffisante pour une expertise phytosanitaire détaillée.
- Le mécanisme de synchronisation existant repose sur une file hors ligne. Des modifications simultanées du MÊME enregistrement sur deux téléphones hors ligne peuvent conduire à une écriture ultérieure qui remplace l'autre. Éviter de modifier la même demande sur deux appareils simultanément.
- Un suivi des commandes ne remplace pas les obligations de devis, bon de livraison ou de facturation.
- Test des fonctions réalisé sur le code ; la publication GitHub et les essais en condition réelle avec micro, appareil photo et synchronisation doivent être effectués sur les appareils.

HISTORIQUE
==========
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
