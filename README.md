# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.4 — correction du clignotement](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.4-clignotement)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.4-clignotement/No_Heritage_Life_V1.apk)
- [Packs et manifeste pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/No_Heritage_Life_Ressources_1.4.1.zip)
- [Manifeste réellement configuré](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/manifest.json)
- [Empreintes SHA256](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.4-clignotement/SHA256SUMS.txt)

## Installer

1. Installer l’APK en mise à jour de l’application existante, **sans la désinstaller**.
2. Au premier lancement, télécharger les deux packs (13,90 Mo décimaux) et attendre leur vérification. Les packs 1.4.1 déjà installés et valides sont réutilisés.
3. Garder le profil ÉQUILIBRÉE pour le premier essai. Après installation complète, les sessions suivantes utilisent les ressources locales hors ligne.

L’import local reste disponible : sélectionner le ZIP lié ci-dessus dans le lanceur, sans le décompresser. Il reste compatible avec les APK codes 7 à 10 ; les packs valides installés avec le code 6 sont également réutilisables.

## Version et correction

APK **1.4.4-clignotement**, code **10** ; contenu **1.4.1** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**.

Le clignotement du parvis a été reproduit sous Linux. Le dallage et le dessus de volumes de support occupaient exactement le même plan. Les faces cachées ont été retirées ; les collisions et hauteurs sont conservées. Le dessus des fondations des ailes est conservé du côté où le jardin descend. La mer régionale est découpée sous la Seine monumentale pour éviter une seconde surface d’eau superposée.

Caméra, commandes, textures, shaders, éclairage, reflets, lanceur et budgets mémoire de 1.4.3 sont inchangés : plafond de 30 images/s, pixels 3D bornés, atlas de reflets réduit et secteurs locaux limités.

## Validation et limites

Préversion de développement. Sous Godot/Linux : 22 points géométriques contrôlés ont une seule surface rendue après correction, contre deux ou trois auparavant. Les séquences de 36 images avant/après montrent une forte réduction des alternances sur le sol. Elles ne mesurent pas les FPS Android.

98 contrôles de marche jour/nuit, 35 du monument, 82 raccordements, 19 de budgets et 85 de mémoire réussissent. Le contenu exact de l’APK exporté démarre hors réseau sous Godot/Linux ; la mise à jour code 9 → 10 conserve les packs, paramètres et sauvegarde témoin. Signature et alignement de l’APK vérifiés.

**La correction reste à confirmer sur le S23 Ultra.** La chauffe, les fermetures, l’API thermique native et les longues sessions restent à vérifier sur appareil. En cas de fermeture, rouvrir le jeu puis choisir Pause → COPIER LE DIAGNOSTIC. La finition artistique reste en cours.

Les packs common 1.4.0 et world 1.4.1 sont inchangés. Le manifeste précise tailles, empreintes et dépendances. Les archives « Source code » automatiques de GitHub contiennent ce dépôt de distribution ; les sources complètes du jeu sont livrées séparément à son auteur.
