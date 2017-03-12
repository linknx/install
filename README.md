# install
Script install LinKnx &amp; KnxWeb

Installation de KnxD / LinKnx / KnxWeb

 Credits : Ivan Morgade, Anthony PENHARD

 Script libre: GPLv3

 Version v0.17

Install de :
 - pthsem  : 2.0.8
 - KnxD    : "git stable version"
 - LinKnx  : 0.0.1.33  ( + mysql pour les logs )
 - KnxWeb  : 2.1.1 ( + serveur web apache2 )
 - créer un "user" : "knx"  mot de passe "knx"
 - possibilité d'installer :
  - Webmin : Dernière version stable


Liste des commandes :

wget https://github.com/linknx/install/archive/master.tar.gz && tar -xzf master.tar.gz

cd install-master

sudo chmod u+x install-trio.sh

sudo sh ./install-trio.sh --with-mysql --login=knx --password=knx --with-webmin

if you want to log the install for debug or other use :

sudo sh ./install-trio.sh --with-mysql --login=knx --password=knx --with-webmin | tee -a logfile.log

