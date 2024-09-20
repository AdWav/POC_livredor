# POC_livredor

## Ubuntu → WSL  (https://bluevps.com/blog/how-to-install-java-on-ubuntu)
## Installer openjdk
sudo apt-get install openjdk-21-jdk
java --version
javac --version

### Lister les différentes version d'openjdk installées
$ sudo update-alternatives --config java

### Ajouter ce PATH aux veriable d'environnement
$ sudo nano /etc/environment

Vous apercevrez une ligne de ce type :
PATH="toutes_vos variable_d'environnement_pour_le_PATH"

aller à la ligne et écrivez : 
JAVA_HOME="/usr/lib/jvm/java-21-openjdk-amd64" 

(Qui doit être le PATH de la précédente commande dans le terminal. Arrêtez-vous avant le "/bin/java")

### "Recharger" le fichier pour le mettre à jour par cette commande :
$ source /etc/environment
