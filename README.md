# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.8 — Revêtements](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.8-revetements)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.8-revetements/No_Heritage_Life_V1.apk)
- [Packs 1.4.7 pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/No_Heritage_Life_Ressources_1.4.7.zip)
- [Manifeste réellement configuré dans l’APK](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/manifest.json)
- [Empreintes de l’APK et du manifeste](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.8-revetements/SHA256SUMS.txt)

## Installer et voler

Installer **sans désinstaller** l’application. Cette mise à jour réutilise les packs **common 1.4.0** et **world 1.4.7** : aucun téléchargement supplémentaire si 1.4.7 et ses packs valides sont déjà installés. Une première installation télécharge **16,41 Mo** de packs. Le ZIP permet aussi une importation locale : le sélectionner dans le lanceur sans le décompresser. Après installation complète, le jeu utilise ses fichiers locaux hors ligne.

1. Ouvrir **Pause → VOL DE TEST · ACTIVER**.
2. Utiliser le joystick et le regard habituels, avec **MONTER / DESCENDRE** à maintenir.
3. Toucher le bouton de vitesse pour alterner **90 → 180 → 30 m/s**.
4. Pour marcher, choisir **Pause → SE POSER ICI · À PIED**, attendre la préparation du sol puis reprendre la promenade.

Le vol traverse les structures pour faciliter les essais. En vol rapide ou élevé, le jeu utilise les panoramas permanents et libère les secteurs détaillés. Le retour au sol prépare les collisions et vérifie une place libre. Un nouveau lancement démarre à pied. Clavier : Espace/Ctrl pour monter/descendre, F pour la vitesse.

## Revêtements 1.4.8

APK **1.4.8-revetements**, code **14** ; contenu **1.4.7** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**.

- Trocadéro : dallage de pierre grise avec joints et inserts géométriques adoucis.
- Tour Eiffel : parvis en asphalte gris, approches minérales et jardins latéraux.
- Champ-de-Mars et Joffre : stabilisé compacté gris-beige sur les allées documentées ; pelouses, trottoirs et seuils distincts.
- Pont : chaussée en asphalte et trottoirs en pierre ; terre limitée au pied des haies.
- École militaire, végétation statique, caméra, commandes, vol, lumière et reflets conservés.

Références : [Ville de Paris, étude d’impact 2022](https://cdn.paris.fr/paris/2022/02/24/ec6ef4e66b62c531c07bf578e5d40235.pdf), [OPPIC, esplanade du Trocadéro](https://www.oppic.fr/article1423.html), [SETE, jardins](https://sete.toureiffel.paris/fr/presse/communiques/point-detape-chantier-du-14-juin-2018). Adaptation originale, pas un relevé exact de chaque dalle. Le stabilisé reste présent là où il est documenté ; les projets futurs ne sont pas présentés comme des travaux déjà réalisés.

## Vérifications

Sous Godot/Linux : **413 contrôles de régression** (monuments, raccords, parcours continu jour/nuit, mémoire, vol et budgets thermiques). Les ressources exactes de l’APK ont été exécutées avec les packs externes, hors réseau ; contrôles du parc, du vol et du budget thermique réussis. Mise à jour **code 13 → 14** : packs, préférences et sauvegarde témoin conservés sans réécriture. Signature et alignement 16 Kio vérifiés.

Neuf vues comparables : mêmes primitives et même mémoire vidéo déclarée, aucune nouvelle texture, lumière ou sonde. Le changement de matériau du pont ajoute **0 à 3 appels de dessin** selon la vue. Deux séquences de petites translations de caméra comparent la variation des pixels avec 1.4.7 ; elles ne constituent pas une garantie contre tout scintillement.

Ces mesures utilisent Linux/llvmpipe, **pas le GPU du téléphone**. L’installation native, les gestes tactiles, la chauffe et la stabilité prolongée sur S23 Ultra restent à valider pour cette version.

Le menu **COPIER LE DIAGNOSTIC** fournit les fenêtres récentes, l’état thermique, les reflets et les coûts d’écriture. La pause coupe le rendu 3D ; les captures de reflets sont suspendues en vol élevé/rapide ou sous bridage sévère, puis reprises au sol selon le budget thermique.

Les mécanismes de transfert, interruption, reprise et intégrité sont conservés ; les 44 contrôles de la livraison 1.4.7 restent des preuves historiques, distinctes des tests ci-dessus. [Historique et packs 1.4.7](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.7-champdemars).

Les archives « Source code » automatiques de GitHub contiennent ce dépôt de distribution. Les sources complètes, la procédure de construction et les preuves sont livrées séparément à l’auteur.
