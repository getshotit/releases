# ShotIt — installeurs

Ce dépôt ne contient **aucune source**. Il ne sert qu'à distribuer les
installeurs de ShotIt et le flux de mise à jour que l'application consulte.

**[Télécharger la dernière version](../../releases/latest)**

## ShotIt

Capture d'écran et annotation pour Windows et macOS. On sélectionne une zone,
on l'annote — flèche, rectangle, texte, surligneur, pixelisation — puis on la
copie ou on l'enregistre. Tout se passe sur la machine : l'application ne parle
à aucun serveur, hormis pour vérifier qu'une mise à jour existe.

## Ce que contient chaque version

| Fichier | Rôle |
| --- | --- |
| `ShotIt_Setup_<version>.exe` | Installeur Windows, par utilisateur, sans droits administrateur |
| `ShotIt_Setup_<version>.exe.blockmap` | Permet aux mises à jour de ne télécharger que ce qui a changé |
| `latest.yml` | Flux que l'application lit pour détecter une nouvelle version |

Les trois fichiers vont ensemble : publier l'installeur sans son `.blockmap`
ferait retélécharger l'application entière à chaque correction.

## Avertissement Windows au premier lancement

L'application n'est pas encore signée par un certificat d'éditeur. Windows
affiche donc « Windows a protégé votre ordinateur » et cache le bouton
d'exécution derrière *Informations complémentaires*. C'est attendu, et cela
n'empêche ni l'installation, ni les mises à jour automatiques.

---

ShotIt est un logiciel propriétaire. Copyright © 2026 Haniko.
Tous droits réservés.
