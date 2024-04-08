<strong><h1><div class="titre">SAE 2.03</div></h1></strong>
<h2><div class="sous-titre">Module Réseau</div></h2>
<br>

<u>Objectifs :</u>
- Installer et configurer un serveur Web complet sur votre machine virtuelle Linux Ubuntu créée en TD R2.05
- Installer et configurer un serveur Web Apache
- Installer et configurer PHP
- Installer et configurer MySQL
- Installer et configurer phpMyAdmin
- Gérer des services sur un système Linux


<u>Sommaire :</u>
1. [Gestion des services : <code>systemd</code>](#1)
   1.1. 



## 1. Gestion des services : <code>systemd</code><a name="1"></a>

<u>Travail à réaliser :</u>
- Consultez le manuel de la commande <code>systemctl</code> dont la syntaxe générale est : <code>systemctl action cible [option(s)]</code><div><img src="Screenshots/P1Question1.png"></div>
- Affichez la liste des services démarrés avec la commande <code>systemctl</code>
   > Resultat : [fichier texte](commands/CMDP1Question1.txt)
- Si ce n'est déjà fait lors de l'installation, installez le paquet <code>sshd</code> avec la commande suivante : <code>apt-get install openssh-server</code>
   > Resultat : [fichier texte](commands/CMDP1Question1-2.txt)
- Vérifiez que le service <code>sshd</code> est démarré en faisant une connexion ssh sur votre propre machine <code>ssh <adresse_IP_de_votre_VM></code><div>
   > Resultat de la commande : <code>ssh iut@audi0010-ubuntu-server</code><div><img src="Screenshots/P1Question1-2.png">
- Déconnectez-vous en tapant <code>exit</code> ou CTRL+D<div><img src="Screenshots/P1Question1-3.png"></div>
- Stoppez le service sshd puis tentez de vous reconnecter. Que constatez-vous ?
   > Après la commande : <code>sudo systemctl stop ssh.service</code>
   
   > Il n'est pas possible de se reconnecter : <div><img src="Screenshots/P1Question1-4.png"></div>
   Car le service ssh est stopper
- Redémarrez le service <code>sshd</code>
   > Après la commande : <code>sudo systemctl start ssh.service</code>
   
   > On peut se reconnecter : <div><img src="Screenshots/P1Question1-5.png"></div>

## 2. Serveur Web Apache<a name="2"></a>
### 2.1. Configuration de base<a name="21"></a>