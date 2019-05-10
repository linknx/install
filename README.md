# Disclaimer
This script is for informational purpose only. It can be used as an example to guide a new user through the installation steps but its logic is not ideal and can easily lead to a corrupt setup. Therefore, a manual installation after understanding the overall architecture is highly recommended.

# Install
Script install LinKnx &amp; KnxWeb

Installation de KnxD / LinKnx / KnxWeb

 Credits : Ivan Morgade, Anthony PENHARD
 Script libre: GPLv3

Install de :
 - pthsem  : 2.0.8
 - KnxD    : "git stable version"
 - LinKnx  : 0.0.1.32  ( + mysql pour les logs )
 - KnxWeb  : 2.1.0 ( + serveur web apache2 )
 - créer un "user" : "knx"  mot de passe "knx"
 - possibilité d'installer :
  - Webmin : Dernière version stable


Liste des commandes :

wget https://github.com/linknx/install/archive/master.tar.gz && tar -xzf master.tar.gz

cd install-master

sudo chmod u+x install-trio.sh

sudo sh ./install-trio.sh --with-mysql --login=knx --password=knx --with-webmin

