

# **Guide d'utilisation**
_Projet NF19 - Semestre A22_

Projet mené dans le cadre de l'UE NF19 à l'Université de Technologie de Troyes. Il s'agit du déploiement de l'environnement de test de l'entreprise GiftCard, un site web créé avec WordPress.

# Prérequis de l'installation
## 1. Installer Docker 
_Etape à passer si vous avez déjà Docker Desktop sur votre machine_

Liens de téléchargements :

* Général : https://docs.docker.com/desktop/
* MacOS : https://docs.docker.com/desktop/install/mac-install/
* Linux : https://docs.docker.com/desktop/install/linux-install/
* Windows : https://docs.docker.com/desktop/install/windows-install/



## 2. Installer le plugin Docker-compose
_Si vous avez déjà Docker Desktop, passez à la suite._
_Cette section concerne ceux qui n'ont que Docker Engine & Docker CLI_
1. Installez docker-compose (https://docs.docker.com/compose/gettingstarted/) en suivant la documentation suivante : https://docs.docker.com/compose/install/

## 3. Vérifier l'installation 
1. Lancer la commande :
```docker compose version```
2. Le terminal doit afficher quelque chose de ce style : 
```Docker Compose version v2.14.2```

Si le terminal ne reconnait pas le terme Docker, l'installation a échoué

# Installation
## 1. Lancer Docker : 
    [sudo] systemctl start docker
## 2. Obtenir le dossier wordpress-docker-compose :

* Téléchargez le dossier ZIP : cliquer sur le bouton Code > Download ZIP 
    ![Alt text](../wordpress-docker-compose/git_download.png "Optional title")
* Décompressez le fichier ZIP dans le dossier de votre choix
    ![Alt text](../wordpress-docker-compose/zip_decompress.png "Optional title")
* Vérifiez que le dossier NF19_GiftCard décompressé contient le dossier wordpress-docker-compose.

## 3. Installer le système :
* Ouvrez un terminal
* Placez-vous dans le dossier wordpress-docker-compose **qui comporte le fichier docker-compose.yaml** en exécutant  la commande : 

        cd chemin_relatif_d'accès_au_dossier
* Pour installer les conteneurs du système Docker, exécutez la commande : 

        [sudo] docker-compose up 

* Patientez le temps de l'installation complète du système

## 4. Accéder au site customisé : 

### **En tant que visiteur : visiter le site**
Ouvrez le navigateur de votre choix et entrez l'url suivante : http://localhost:8000
### **En tant que développeur : modifier le site** 
* Ouvrez le navigateur de votre choix et entrez l'url suivante :  http://localhost/wp-admin/
* Se connecter avec l'identifiant ``giftcard_user`` et mot de passe ``giftcard_userPASS``
* Vous pourrez alors modifier les articles, en ajouter, ajouter des pages etc ....

**NB : si vous souhaitez faire évoluer le site**, au lieu de télécharger le fichier ZIP, il faut exécuter la commande ``git clone https://github.com/evebrnd/NF19_GiftCard.git``. Pour mettre en ligne les modifications exécutez successivement à la racine du dossier de travail ``git add .`` puis ``git commit -m "message_au_choix"`` et ``git push``

## 5. Quitter le site
* Placez-vous sur le terminal qui fait tourner les conteneurs
* Appuyer sur CTRL + C
* Entrer la commande

        docker-compose down

# Auteures
Ce projet a été réalisé par :
* **Eve BERNHARD** _alias_ [@evebrnd](https://github.com/evebrnd)
* **Jeanne BOYER** _alias_ [@MissJeanneB](https://github.com/MissJeanneB)


# Licence MIT
Copyright (c) 2022 - Eve BERNHARD, Jeanne BOYER

L'autorisation est accordée par la présente, gratuitement, à toute personne obtenant une copie de ce logiciel et des fichiers de documentation associés (le "Logiciel"), de traiter le Logiciel sans restriction, y compris, sans s'y limiter, les droits d'utilisation, de copie, de modification, de fusion, de publication, de distribution, de sous-licence et/ou de vente de copies du Logiciel, et d'autoriser les personnes à qui le Logiciel est fourni à le faire, sous réserve des conditions suivantes :

L'avis de copyright ci-dessus et cet avis d'autorisation doivent être inclus dans toutes les copies ou parties substantielles du logiciel.

LE LOGICIEL EST FOURNI " EN L'ÉTAT ", SANS GARANTIE D'AUCUNE SORTE, EXPRESSE OU IMPLICITE, Y COMPRIS, MAIS SANS S'Y LIMITER, LES GARANTIES DE QUALITÉ MARCHANDE, D'ADAPTATION À UN UN USAGE PARTICULIER ET DE NON-VIOLATION. EN AUCUN CAS, LES AUTEURS OU LES DÉTENTEURS DE EN AUCUN CAS LES AUTEURS OU LES DÉTENTEURS DE DROITS D'AUTEUR NE PEUVENT ÊTRE TENUS RESPONSABLES DE TOUTE RESPONSABILITÉ, QU'IL S'AGISSE D'UNE ACTION CONTRACTUELLE, DÉLICTUELLE OU AUTRE, DÉCOULANT DE OU EN RELATION AVEC LE LOGICIEL OU L'UTILISATION OU AUTRE DE CELUI-CI. OU EN RELATION AVEC LE LOGICIEL OU L'UTILISATION OU TOUTE AUTRE TRANSACTION RELATIVE AU LOGICIEL.
