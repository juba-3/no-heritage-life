# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.3 — mémoire et charge graphique](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.3-performance)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.3-performance/No_Heritage_Life_V1.apk)
- [Packs et manifeste pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/No_Heritage_Life_Ressources_1.4.1.zip)
- [Manifeste réellement configuré](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/manifest.json)
- [Empreintes SHA256 de la nouvelle livraison](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.3-performance/SHA256SUMS.txt)

## Installer

1. Installer l’APK en mise à jour de l’application existante, sans la désinstaller.
2. Au premier lancement, choisir « Télécharger les ressources » puis attendre la vérification et l’installation des deux packs (13,90 Mo décimaux). Les packs 1.4.1 déjà installés et valides sont réutilisés.
3. Garder le profil ÉQUILIBRÉE pour le premier essai. Les sessions suivantes utilisent les ressources installées hors ligne.

L’import local reste disponible : sélectionner le ZIP lié ci-dessus dans le lanceur, sans le décompresser. Il reste compatible avec les APK codes 7, 8 et 9 ; les packs valides installés avec le code 6 sont également réutilisables.

## Version

APK **1.4.3-performance**, code **9** ; contenu **1.4.1** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**. Le pack commun 1.4.0 et le monde 1.4.1 sont inchangés. Le manifeste précise tailles, empreintes et dépendances.

## Changements

- Limite de 30 images/s et plafond de pixels 3D indépendant de la définition de l’écran.
- Atlas des reflets ramené de 64 à 12 emplacements ; captures proches et éclairages bornés.
- Panoramas découpés spatialement ; secteurs déchargés plus tôt, travaux devenus inutiles annulés et données CPU temporaires libérées après transfert.
- Réduction du budget en cas de chauffe signalée par Android, avec délai de récupération.
- Bouton Pause → COPIER LE DIAGNOSTIC et conservation de la session précédente.

Caméra, commandes, géométrie des monuments, carte, textures, shaders, lanceur et végétation statique conservés.

## État de validation

Préversion de développement. Les trois nouveaux fichiers publiés (APK, manifeste et empreintes) ont été téléchargés sans authentification et comparés aux originaux : tailles et SHA256 identiques. Une reprise HTTP après interruption du pack commun a été vérifiée. Signature et alignement de l’APK vérifiés.

Le contenu exact de l’APK exporté démarre hors réseau sous Godot/Linux. La mise à jour code 8 → 9 conserve les packs, les paramètres et une sauvegarde témoin sans réécriture. 98 contrôles du parcours continu jour/nuit, 35 du monument et 82 raccordements réussissent dans cet environnement. Six boucles de chargement avec rendu montrent un nombre d’objets stable aux retours et un plateau de mémoire graphique et de RSS après échauffement.

Sur le banc Linux à rendu logiciel, la mémoire graphique déclarée près de la tour passe de 379,9 à 120,5 Mio. Ces mesures ne sont pas des performances Android.

**La disparition des fermetures et de la chauffe sur S23 Ultra n’est pas encore validée.** L’API thermique native, le presse-papiers et les longues sessions restent à tester sur téléphone. En cas de fermeture, rouvrir le jeu, choisir Pause → COPIER LE DIAGNOSTIC et transmettre le texte à l’auteur. La finition artistique reste en cours.

Les archives « Source code » automatiques de GitHub contiennent les fichiers de ce dépôt de distribution. Elles ne constituent pas les sources complètes du jeu, livrées séparément à son auteur.
