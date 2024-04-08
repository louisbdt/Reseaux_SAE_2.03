<center><strong><h1><div class="titre">SAE 2.03</div></strong>
<div class="sous-titre">Module Réseau</div></center>
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
- Consultez le manuel de la commande <code>systemctl</code> dont la syntaxe générale est : <code>systemctl action cible [option(s)]</code><div class="image"><img src="Screenshots/P1Question1.png"></div>
- Affichez la liste des services démarrés avec la commande <code>systemctl</code>
   > Resultat : [fichier texte](commands/CMDP1Question1.txt)
- Si ce n'est déjà fait lors de l'installation, installez le paquet <code>sshd</code> avec la commande suivante : <code>apt-get install openssh-server</code>
   > Resultat : [fichier texte](commands/CMDP1Question1-2.txt)