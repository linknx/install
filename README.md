# install
Script install LinKnx &amp; KnxWeb

Installation de KnxD / LinKnx / KnxWeb

 Credits : Ivan Morgade, Anthony PENHARD
 Script libre: GPLv3

Install de :
 - pthsem  : 2.0.8
 - KnxD    : "git current version"
 - LinKnx  : 0.0.1.32  ( + mysql pour les logs )
 - KnxWeb  : 2.1.0 ( + serveur web apache2 )
 - créer un "user" : "knx"  mot de passe "knx"
 - possibilité d'installer :
  - Webmin : Dernière version stable
  - YANA4ALL ( TODO ... )

$ unzip install-master.zip
$ cd install-master
$ sudo chmod 777 install-trio.sh
$ sudo chmod u+x install-trio.sh
$ sudo ./install-trio.sh

autres options :
$ sudo sh ./install-trio.sh --with-mysql --login=knx --password=knx
$ sudo sh ./install-trio.sh --with-mysql --with-webmin