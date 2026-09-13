# Politique de confidentialité — The Steward

Dernière mise à jour : 12 septembre 2026.

The Steward est conçu pour fonctionner sans compte et pour conserver les données
personnelles sur l’appareil. L’application n’intègre ni publicité, ni outil
d’analyse d’audience, ni profilage.

## Données conservées localement

Selon les fonctions utilisées, l’application peut enregistrer :

- les séances, exercices, séries, performances et notes d’entraînement ;
- les aliments, repas, objectifs et journaux nutritionnels ;
- les habitudes suivies, événements, raisons, stratégies et moments de doute ;
- les préférences d’affichage, paramètres et objectifs quotidiens ;
- le total quotidien agrégé des pas lorsque l’accès Health Connect est autorisé.

Ces informations sont conservées dans une base SQLite chiffrée. Sa clé est
stockée dans le stockage sécurisé fourni par le système d’exploitation.

## Communications externes

The Steward n’envoie aucune donnée à un serveur exploité par Arthas Solutions.
Deux fonctions facultatives peuvent communiquer avec un service tiers :

- **Open Food Facts** : lors d’une recherche explicite par code-barres absent du
  cache local, le code-barres est transmis au service afin d’obtenir la fiche du
  produit ;
- **Health Connect** : Android fournit à l’application un total de pas agrégé
  pour la date demandée, uniquement après accord de l’utilisateur.

Les exports « Copier pour IA » placent un texte factuel dans le presse-papiers.
Ils ne contactent et n’ouvrent automatiquement aucun service d’intelligence
artificielle.

## Permissions

- la caméra est demandée uniquement pour scanner un code-barres ;
- les notifications servent notamment aux minuteurs de repos et aux repères
  activés par l’utilisateur ;
- Health Connect reste entièrement facultatif ;
- l’authentification biométrique ou le verrouillage de l’appareil peuvent protéger
  l’accès à Control.

Refuser une permission ne bloque pas le reste de l’application. Les captures
d’écran sont empêchées uniquement dans Control afin de protéger les informations
sensibles ; elles restent possibles dans les autres espaces.

## Sauvegarde, export et suppression

L’utilisateur peut, depuis **Réglages → Confidentialité et données** :

- créer une sauvegarde chiffrée au format `.steward` ;
- restaurer une sauvegarde après vérification complète ;
- produire un export JSON lisible et sélectif ;
- supprimer les données de l’application.

Une désinstallation Android supprime normalement le stockage privé local. Il est
donc recommandé de créer une sauvegarde avant de désinstaller ou de changer
d’appareil.

## Contact

Pour toute question relative à la confidentialité : `contact@arthas.fr`.

Cette politique décrit la version présentée dans ce dépôt. Les règles propres à
Open Food Facts, Health Connect, Android et aux boutiques d’applications restent
applicables à leurs services respectifs.
