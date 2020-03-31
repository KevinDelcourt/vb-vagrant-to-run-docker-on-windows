## Objectif

Faire marcher docker sur windows (sans utiliser [docker windows](https://docs.docker.com/docker-for-windows/) qui nécessite Windows Pro)

## Pré requis

1. Installer [Virtualbox](https://www.virtualbox.org/)

2. Installer [Vagrant](https://www.vagrantup.com/)

## Installation

1. Créer un dossier (appelé par exemple `VAGRANT`) sur l'ordinateur

2. Coller dans ce dossier le [Vagrantfile](/Vagrantfile)

3. Ouvrir l'invité de commande Windows (`cmd` dans la barre de recherche)

## Démarrer

1. Se placer dans le dossier `VAGRANT` (`cd <chemin vers le dossier>`)

2. Lancer la vm linux: `vagrant up`

3. Se connecter à la vm: `vagrant ssh`

4. Vérifier que Docker est bien installé et marche: `docker version` / `docker run hello-world`

#### Les sous-dossiers du dossier `VAGRANT` sont disponibles dans le répertoire `/vagrant` de la machine virtuelle

## Quitter

1. `exit` pour quiter la session ssh

2. `vagrant halt` pour arrêter la machine virtuelle

## Infos

1. Il est possible d'éditer le Vagrantfile pour modifier des options comme la liste des ports transférés entre la vm et l'hôte

2. Faire très attention aux différences de fin de ligne entre windows et linux
