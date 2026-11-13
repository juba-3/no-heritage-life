# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.7 — Champ-de-Mars](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.7-champdemars)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/No_Heritage_Life_V1.apk)
- [Packs pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/No_Heritage_Life_Ressources_1.4.7.zip)
- [Manifeste configuré dans l’APK](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/manifest.json)
- [Empreintes SHA256](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/SHA256SUMS.txt)

## Installer et voler

Installer l’APK **sans désinstaller** l’application. Le lanceur télécharge le nouveau pack **world 1.4.7 (3,36 Mo)** et réutilise **common 1.4.0** si déjà installé et valide. Une première installation télécharge **16,41 Mo** de packs. Le ZIP permet aussi une importation locale : le sélectionner dans le lanceur sans le décompresser. Après installation complète, le jeu utilise ses fichiers locaux hors ligne.

1. Ouvrir **Pause → VOL DE TEST · ACTIVER**.
2. Utiliser le joystick et le regard habituels, avec **MONTER / DESCENDRE** à maintenir.
3. Toucher le bouton de vitesse pour alterner **90 → 180 → 30 m/s**.
4. Pour marcher, choisir **Pause → SE POSER ICI · À PIED**, attendre la préparation du sol puis reprendre la promenade.

Le vol traverse les structures pour faciliter les essais. En vol rapide ou élevé, le jeu utilise les panoramas permanents et libère les secteurs détaillés. Le retour au sol prépare les collisions et vérifie une place libre. Le mode reste temporaire : un nouveau lancement démarre à pied. Clavier : Espace/Ctrl pour monter/descendre, F pour la vitesse.

## Champ-de-Mars et validation

APK **1.4.7-champdemars**, code **13** ; contenu **1.4.7** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**.

Le parc est reconstruit d’après les plans de l’[APUR](https://www.apur.org/sites/default/files/documents/jardins_champ_mars.pdf) et de la [Ville de Paris](https://www.paris.fr/lieux/parc-du-champ-de-mars-1807) : pelouse centrale, grandes allées, doubles alignements de platanes, jardins latéraux, bassin Jacques-Rueff, place Joffre et façade de l’École militaire. Cette adaptation originale conserve l’axe vers la tour Eiffel et la vue inverse. Elle comporte 324 arbres statiques, trois bassins, des bancs, lanternes, bordures et fenêtres en retrait. Ce n’est pas un relevé architectural à l’identique.

Les groupes de sol et le quartier d’origine lointain sont simplifiés pour réduire les appels de dessin. Les arbres utilisent des détails adaptés à la distance. Aucune nouvelle lumière dynamique ni sonde de reflet. Caméra, commandes, vol, correctifs de clignotement et protections thermiques précédentes conservés.

Sur ordinateur : **23 contrôles spécifiques du parc**, **120 contrôles du parcours continu de jour et de nuit**, raccords/collisions/vol/mémoire/thermique réussis. **44 contrôles** de téléchargement, interruption, reprise, intégrité, retour arrière et démarrage hors ligne. Les ressources exactes de l’APK ont été montées et exécutées avec les nouveaux packs ; mise à jour code 12 → 13, sauvegarde et préférences conservées, pack commun réutilisé sans réécriture. Signature et alignement 16 Kio vérifiés.

| Vue témoin, mêmes caméra et réglages | Appels de dessin 1.4.6 | 1.4.7 |
|---|---:|---:|
| À pied, pelouse vers la tour | 1 996 | 636 |
| Depuis la tour vers le parc | 174 | 206 |

Mesures Linux/llvmpipe, pas des FPS Android. La vue aérienne montre davantage de végétation et de géométrie. Les essais prolongés, la chauffe, les crashes, les pilotes et l’installation native sur S23 Ultra restent à valider pour cette version.

Le menu **COPIER LE DIAGNOSTIC** fournit les fenêtres récentes, l’état thermique, les reflets et les coûts d’écriture. La pause coupe le rendu 3D ; les captures de reflets sont suspendues en vol élevé/rapide ou sous bridage sévère, puis reprises au sol selon le budget thermique.

Les archives « Source code » automatiques de GitHub contiennent ce dépôt de distribution. Les sources complètes, la procédure de construction et les preuves sont livrées séparément à l’auteur.
