# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.5 — mode de vol rapide](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.5-vol)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.5-vol/No_Heritage_Life_V1.apk)
- [Packs pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/No_Heritage_Life_Ressources_1.4.1.zip)
- [Manifeste réellement configuré](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/manifest.json)
- [Empreintes SHA256](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.5-vol/SHA256SUMS.txt)

## Installer et voler

Installer l’APK **sans désinstaller** l’application. Les packs common 1.4.0 et world 1.4.1 déjà installés et valides sont réutilisés. Pour une première installation, télécharger les ressources dans le lanceur (13,90 Mo décimaux) ou y sélectionner le ZIP ci-dessus sans le décompresser. Après installation complète, le jeu utilise les ressources locales hors ligne.

1. Ouvrir **Pause → VOL DE TEST · ACTIVER**.
2. Utiliser le joystick et le regard habituels, avec **MONTER / DESCENDRE** à maintenir.
3. Toucher le bouton de vitesse pour alterner **90 → 180 → 30 m/s**.
4. Pour marcher, choisir **Pause → SE POSER ICI · À PIED**, attendre la préparation du sol puis reprendre la promenade.

Le vol traverse les structures pour faciliter les essais. En vol rapide ou élevé, le jeu utilise les panoramas permanents et libère les secteurs détaillés. Le retour au sol prépare les collisions et vérifie une place libre. Le mode reste temporaire : un nouveau lancement démarre à pied. Clavier : Espace/Ctrl pour monter/descendre, F pour la vitesse.

## Version et validation

APK **1.4.5-vol**, code **11** ; contenu **1.4.1** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**.

Le correctif de clignotement de 1.4.4, les reflets, l’éclairage et les budgets mémoire/thermiques de 1.4.3 sont conservés. Le joueur a confirmé la disparition du clignotement avec la version précédente.

Sous Godot/Linux : **39 contrôles de vol** et **319 contrôles de régression** réussis. Le vol est également contrôlé à partir des ressources exactes de l’APK, avec les packs installés. La mise à jour code 10 → 11 conserve les packs, préférences et sauvegarde témoin. Signature et alignement 16 Kio vérifiés.

Le nouveau mode reste à essayer sur téléphone. Ces vérifications ne mesurent pas la chauffe ou les performances du S23 Ultra ; les longues sessions et la stabilité sur l’appareil restent à confirmer. Le menu **COPIER LE DIAGNOSTIC** indique aussi le mode de déplacement et sa vitesse.

Les archives « Source code » automatiques de GitHub contiennent ce dépôt de distribution. Les sources complètes, la procédure de construction et les preuves sont livrées séparément à l’auteur.
