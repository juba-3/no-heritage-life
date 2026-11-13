# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.6 — thermique et pause](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.6-thermique)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.6-thermique/No_Heritage_Life_V1.apk)
- [Packs pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/No_Heritage_Life_Ressources_1.4.1.zip)
- [Manifeste réellement configuré](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/manifest.json)
- [Empreintes SHA256](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.6-thermique/SHA256SUMS.txt)

## Installer et voler

Installer l’APK **sans désinstaller** l’application. Les packs common 1.4.0 et world 1.4.1 déjà installés et valides sont réutilisés. Pour une première installation, télécharger les ressources dans le lanceur (13,90 Mo décimaux) ou y sélectionner le ZIP ci-dessus sans le décompresser. Après installation complète, le jeu utilise les ressources locales hors ligne.

1. Ouvrir **Pause → VOL DE TEST · ACTIVER**.
2. Utiliser le joystick et le regard habituels, avec **MONTER / DESCENDRE** à maintenir.
3. Toucher le bouton de vitesse pour alterner **90 → 180 → 30 m/s**.
4. Pour marcher, choisir **Pause → SE POSER ICI · À PIED**, attendre la préparation du sol puis reprendre la promenade.

Le vol traverse les structures pour faciliter les essais. En vol rapide ou élevé, le jeu utilise les panoramas permanents et libère les secteurs détaillés. Le retour au sol prépare les collisions et vérifie une place libre. Le mode reste temporaire : un nouveau lancement démarre à pied. Clavier : Espace/Ctrl pour monter/descendre, F pour la vitesse.

## Version et validation

APK **1.4.6-thermique**, code **12** ; contenu **1.4.1** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**.

Cette version coupe le rendu 3D pendant la pause, suspend les nouvelles captures de reflets en vol élevé/rapide ou sous bridage sévère, et déclenche plus tôt la prévention thermique. Les journaux sont encodés et écrits par un travailleur unique. Le diagnostic distingue les 10/60 dernières secondes de jeu et propose un compteur natif Android optionnel, distinct de la mémoire totale.

Mode de vol, caméra, décors et correctif de clignotement conservés. Les reflets proches sont repris au sol ; leurs rafraîchissements sont espacés et peuvent attendre pendant le refroidissement.

Sous Godot/Linux : **28 contrôles ciblés** et **358 contrôles de régression** réussis. Vol et contrôles thermiques également exercés avec les ressources exactes de l’APK. Démarrage hors réseau avec packs installés ; mise à jour code 11 → 12 conservant packs, préférences et sauvegarde témoin. Signature et alignement 16 Kio vérifiés.

Dans la scène de comparaison Linux, le menu passe de 541 à 22 appels de dessin. Les appels de dessin de la vue principale en vol restent inchangés : le coût du décor doit encore être réduit. Ces mesures ne prouvent pas une baisse de température ni la disparition des crashes sur S23 Ultra. Les essais prolongés de cette version et le nouveau compteur natif restent à valider sur téléphone.

Le menu **COPIER LE DIAGNOSTIC** fournit les fenêtres récentes, l’état thermique, les reflets et les coûts d’écriture. Installer en mise à jour sans désinstaller.

Les archives « Source code » automatiques de GitHub contiennent ce dépôt de distribution. Les sources complètes, la procédure de construction et les preuves sont livrées séparément à l’auteur.
