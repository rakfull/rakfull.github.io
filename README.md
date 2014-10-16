rakfull.github.io
=================

Github:

Repository name : rakfull / site
SSH key : 5e:ed:d6:fb:bf:c0:6f:2f:69:a4:6d:a3:0e:83:f8:b2

Procédure :

créer une machine virtuelle
sudo apt-get install apache2
                     mysql-server
                     ruby
                     jekyll
                     git

Créer un compte github
Créer un nouveau répertoire
On prend l'URL du clone répertoire, par exemple :
https://github.com/rakfull/rakfull.github.io.git

On génère use SSH key :
settings > SSH key > generating SSH keys > Download GitHub for Mac > Install > Saisir données compte github
Une SSH key est générée à l'email du compte github

Terminal :
xubuntu/site (création d'un dossier/répertoire site), ouvrir un terminal ici
git clone https://github.com/rakfull/rakfull.github.io.git

sudo -s (pour être en admin tout le temps)
apt-get install edit
cd (à la racine racine) /etc/apache2/sites-avalaible/
gedit 000-default.conf
Modifier la ligne suivante : DocumentRoot /home/xubuntu/site/

Dans /etc/apache2/ faire : ledit apache2.conf
Rajouter :
<Directory /home/xubuntu/site/>
	Options Indexes FollowSymLinks
	AllowOverride None
	Require all granted
</Directory>

service apache2 restart

Puis saisir 127.0.0.1 pour voir le répertoire

Mettre un monsieur en collaborateur:
rakfull > rakfull > settings > Collaborators
