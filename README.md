Code pour la connection d'une raspberry pi à un serveur openvpn. Lors de l'utilisation de la pi en version lite (sans desktop), se code vous permettra de vous connecter à votre serveur.

1 - Installation de OpenVPN sur la pi

sudo apt-get update
sudo apt-get upgrade
sudo apt install openvpn
sudo update-rc.d -f openvpn remove
sudo mkdir /home/pi/Python_OpenVPN

Mettre votre fichier de configuration dans /home/pi/Python_OpenVPN et nommer le config.ovpn

Importation du code sur la pi
sudo apt-get install git
cd /home/pi/Python_OpenVPN
git clone github.com/domosolution67/Python_OpenVPN.git

Pour lancer la connexion au VPN 
python /home/pi/Python_OpenVPN/vpn.py
