# No Heritage Life

Jeu Android d’exploration à la première personne. Ce dépôt public héberge les APK et les packs versionnés.

## Télécharger

[Release 1.4.9 — Bassin du Trocadéro](https://github.com/juba-3/no-heritage-life/releases/tag/v1.4.9-eau-trocadero)

- [APK Android](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.9-eau-trocadero/No_Heritage_Life_V1.apk)
- [Packs 1.4.7 pour import local](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/No_Heritage_Life_Ressources_1.4.7.zip)
- [Manifeste réellement configuré](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.7-champdemars/manifest.json)
- [Empreintes APK et manifeste](https://github.com/juba-3/no-heritage-life/releases/download/v1.4.9-eau-trocadero/SHA256SUMS.txt)

## Installer et voler

Installer **sans désinstaller** l’application. Les packs **common 1.4.0** et **world 1.4.7** sont réutilisés : aucun téléchargement supplémentaire s’ils sont déjà installés et valides. Première installation : **16,41 Mo** de packs. Le ZIP permet aussi un import local : le sélectionner dans le lanceur sans le décompresser. Après installation complète, le jeu démarre depuis les fichiers locaux hors ligne.

1. Ouvrir **Pause → VOL DE TEST · ACTIVER**.
2. Utiliser le joystick et le regard habituels ; maintenir **MONTER / DESCENDRE**.
3. Alterner **90 → 180 → 30 m/s** avec le bouton de vitesse.
4. Pour marcher : **Pause → SE POSER ICI · À PIED**, attendre la préparation du sol puis reprendre.

Le vol traverse les structures pour faciliter les essais. En vol rapide ou élevé, le jeu utilise les panoramas et libère les secteurs détaillés. Un nouveau lancement démarre à pied. Clavier : Espace/Ctrl pour monter/descendre, F pour la vitesse.

## Bassin du Trocadéro 1.4.9

APK **1.4.9-eau-trocadero**, code **15** ; contenu **1.4.7** ; Godot **4.6.3 Compatibility** ; Android **10+**, ARMv7 et ARM64.

- Bassin principal arrondi côté Seine, eau horizontale vert olive et fond visible.
- Retenues étagées, cascades animées, 20 canons balistiques de portée 50 m et colonnes secondaires.
- Talus inclinés inspirés des profils IGN, quatre escaliers latéraux et topiaires statiques.
- Jets regroupés et détails adaptés à la distance, à la qualité et au budget thermique ; animation suspendue en pause ou hors champ.
- Caméra, commandes, vol, École militaire, ambiance et mécanismes des reflets de flaques conservés. Aucune nouvelle texture lourde ni lumière dynamique.

Références : étude V2 du projet, orthophoto IGN 2016–2020, cinq profils RGE ALTI, [Ville de Paris](https://www.paris.fr/lieux/jardins-du-trocadero-1789). Adaptation pour la carte existante : profondeur, niveaux fins des retenues et inventaire secondaire des jets restent provisoires. Les jets restent stylisés ; le bassin utilise les reflets d’environnement, sans nouvelle capture miroir.

## Vérifications et limites

Sous Godot/Linux : **33 contrôles du bassin**, **393 contrôles de régression**, **44 contrôles de transfert/interruption/reprise/intégrité/retour arrière**. Ressources exactes de l’APK démarrées avec les packs hors réseau ; contrôles du bassin, du parc, du vol et du budget thermique réussis. Mise à jour **code 14 → 15** : packs, préférences et sauvegarde témoin conservés sans réécriture. Signature et alignement 16 Kio vérifiés.

Neuf vues avant/après à caméras identiques. Mémoire vidéo déclarée Linux : environ 107,0 → 95,4 Mio ; retrait des anciennes sondes dédiées au bassin. Les temps d’image de la scène complète sur le rendu logiciel llvmpipe restent élevés : ils ne valident pas la fluidité mobile. Le coût du décor demeure important.

**Installation native, rendu Adreno, chauffe, mémoire et stabilité prolongée sur S23 Ultra restent à valider.** Aucun gain de FPS Android ni disparition définitive du crash n’est revendiqué. Le menu **COPIER LE DIAGNOSTIC** conserve les relevés thermiques et de temps d’image.

Les trois fichiers de la release et les trois fichiers de contenu configurés ont été téléchargés publiquement et comparés par taille et SHA256. [Historique des versions](https://github.com/juba-3/no-heritage-life/releases).

Les archives « Source code » automatiques de GitHub contiennent uniquement ce dépôt de distribution. Les sources complètes, la procédure de construction et les preuves sont livrées séparément à l’auteur.
