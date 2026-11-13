# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les distributions APK et les packs de ressources versionnés.

## Télécharger

[Release 1.4.2 — Trocadéro et terrasses](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.2-trocadero)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.2-trocadero/No_Heritage_Life_V1.apk)
- [Packs et manifeste pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/No_Heritage_Life_Ressources_1.4.1.zip)
- [Manifeste](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.1-paysages/manifest.json)
- [Empreintes SHA256](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.2-trocadero/SHA256SUMS.txt)

## Installer

1. Installer l’APK en mise à jour de l’application existante, sans la désinstaller.
2. Au premier lancement, choisir « Télécharger les ressources » puis attendre la vérification et l’installation des deux packs (13,90 Mo décimaux).
3. Les sessions suivantes utilisent les ressources installées hors ligne.

L’import local reste disponible : sélectionner le ZIP dans le lanceur, sans le décompresser. Pour les APK codes 7 et 8, utiliser le ZIP de cette release. Une installation complète des packs 1.4.1 réalisée avec l’APK code 6 reste compatible.

## Version

APK **1.4.2-trocadero**, code **8** ; contenu **1.4.1** ; Godot **4.6.3 Compatibility** ; Android **10+**, **ARMv7 et ARM64**. Le pack commun 1.4.0 est inchangé ; le monde est dans le pack 1.4.1. Le manifeste précise tailles, empreintes et dépendances.

## État de validation

Préversion de développement. Les trois nouveaux fichiers publiés (APK, manifeste et empreintes) ont été téléchargés sans authentification et comparés aux originaux : tailles et SHA256 identiques. Les packs restent ceux de la release 1.4.1-paysages. Signature et alignement de l’APK vérifiés. Son contenu exporté démarre hors réseau sous Godot/Linux. La mise à jour code 7 → 8 conserve les packs, les paramètres et une sauvegarde témoin sans réécriture. 98 contrôles du parcours continu jour/nuit et 82 raccordements réussissent dans cet environnement.

Les tests sur téléphone, les performances Android et la reproduction du blocage historique près du parc restent à réaliser. Les ailes, les terrasses et la vue inverse de Chaillot ont été retravaillées ; la finition artistique reste en cours.

Les archives « Source code » automatiques de GitHub contiennent les fichiers de ce dépôt de distribution. Elles ne constituent pas les sources complètes du jeu, livrées séparément à son auteur.
