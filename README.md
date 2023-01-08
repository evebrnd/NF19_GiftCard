

# Guide d'utilisation 
_Projet NF19 - Semestre A22_
Projet mené dans le cadre de l'UE NF19 à l'Université de Technologie de Troyes. Il s'agit du déploiement de l'environnement de test de l'entreprise GiftCard, un site web créé avec WordPress.

## Prérequis de l'installation
1. Installer docker-compose: https://docs.docker.com/compose/install/ en suivant la documentation suivante : https://docs.docker.com/compose/install/
2. Lancer docker-compose

## Installation
1. Obtenir le dossier wordpress-docker-compose
    * Télécharger ZIP : bouton code > Download ZIP 
        ![Tuto téléchargement](D:\Users\Jeanne\Documents\Cours\UTT\NF19 - Administration et virtualisation des systèmes et des bases de données\Projet\telecharger.png "Tuto téléchargement")

    * Décompresser le fichier ZIP dans le dossier de votre choix.
    * Vérifier que le dossier NF19_GiftCard contient le dossier wordpress-docker-compose.

2. Installer le système :
    * Ouvrir un terminal.
    * Pour se placer dans le dossier comportant le fichier wordpress-docker-compose, exécuter la commande : cd chemin_d'accès_au_dossier .
    * Pour installer les conteneurs du système Docker, exécuter la commande : sudo docker-compose up . Patienter le temps de l'installation complète du système.

3. Avoir accès au site customisé : 
    * En tant que vistiteur : ouvrir votre navigateur et rechercher http://localhost:8000
    * En tant que visiteur : ouvrir un navigateur et rechercher  http://localhost/wp-admin/ . Se connecter avec les l'identifiant admin et mot de passe admin.

## Versions
* ??
* 


## Auteurs
Ce projet a été réalisé par :
* **Eve BERNHARD** _alias_ [@evebrnd](https://github.com/evebrnd)
* **Jeanne BOYER** _alias_ [@MissJeanneB](https://github.com/MissJeanneB)


## Licence MIT
Copyright (c) 2022 - Eve BERNHARD, Jeanne BOYER

L'autorisation est accordée par la présente, gratuitement, à toute personne obtenant une copie de ce logiciel et des fichiers de documentation associés (le "Logiciel"), de traiter le Logiciel sans restriction, y compris, sans s'y limiter, les droits d'utilisation, de copie, de modification, de fusion, de publication, de distribution, de sous-licence et/ou de vente de copies du Logiciel, et d'autoriser les personnes à qui le Logiciel est fourni à le faire, sous réserve des conditions suivantes :

L'avis de copyright ci-dessus et cet avis d'autorisation doivent être inclus dans toutes les copies ou parties substantielles du logiciel.

LE LOGICIEL EST FOURNI " EN L'ÉTAT ", SANS GARANTIE D'AUCUNE SORTE, EXPRESSE OU IMPLICITE, Y COMPRIS, MAIS SANS S'Y LIMITER, LES GARANTIES DE QUALITÉ MARCHANDE, D'ADAPTATION À UN UN USAGE PARTICULIER ET DE NON-VIOLATION. EN AUCUN CAS, LES AUTEURS OU LES DÉTENTEURS DE EN AUCUN CAS LES AUTEURS OU LES DÉTENTEURS DE DROITS D'AUTEUR NE PEUVENT ÊTRE TENUS RESPONSABLES DE TOUTE RESPONSABILITÉ, QU'IL S'AGISSE D'UNE ACTION CONTRACTUELLE, DÉLICTUELLE OU AUTRE, DÉCOULANT DE OU EN RELATION AVEC LE LOGICIEL OU L'UTILISATION OU AUTRE DE CELUI-CI. OU EN RELATION AVEC LE LOGICIEL OU L'UTILISATION OU TOUTE AUTRE TRANSACTION RELATIVE AU LOGICIEL.
