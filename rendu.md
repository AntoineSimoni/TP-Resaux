I -
		Afficher nom, adresse MAC et adresse IP de l'interface WiFi et de l'interface ethernet
	~>taper dans le CLI : ipconfig /all
	
Wifi : 
	~>Nom :
	~>Adresse MAC : 30-E3-7A-EC-62-FB
	~>Adresse IP : 10.33.2.32

Ethernet :
	~>Nom :
	~>Adresse MAC : 4C-CC-6A-85-68-DE
	~>Adresse IP : N'en a pas

Passerelle :
	~> IP passerelle : 10.33.3.253

-----------------------------------------------------------------------------------------------

		Afficher IP, MAC et Gateway via Graphical User Interface: 
~>Il suffit de faire clic droit sur le bouton windows (en bas a gauche généralement) puis de cliquer
sur connexions réseau. Ensuite, allez dans l'onglet "ÉTAT" puis cliquez sur affichez
 vos propriétés réseau et c'est gagné !

	~>Adresse IP : 10.33.2.32/22
	~>Adresse MAC : 30:e7:7a:ec:62:fb
	~>Gateway : 10.33.3.253

~>La Gateway (ou passerelle) sert a relier le réseau local d'ynov a Internet.

-----------------------------------------------------------------------------------------------
II -
	Utilisez l'interface graphique de vorte OS pour changer d'adresse IP :

- calculez la première et la dernière IP du réseau
~> première 10.33.0.1
~> dernière 10.33.3.254

- changez l'adresse IP de votre carte WiFi pour une autre (mais toujours dans le même réseau)
~> Il suffit de faire clic droit sur le bouton windows (en bas a gauche généralement) puis de cliquer
sur connexions réseau. Ensuite, allez dans l'onglet "WIFI" et cliquez sur "Modifier les options d'adaptateur"
Une nouvelle page se présente, Clic droit sur "Wi-fi" et sélectionnez "Propriétés".
Encore une fois, une nouvelle fenêtre apparait, cliquez sur "Protocole Internet version 4 (TCP/IPv4) puis propriétés.
Choisissez "Utiliser l'adresse IP suivante : et modifiez comme bon vous semble.

Réponse : il suffit de mettre une adresse entre 10.33.0.1 et 10.33.3.254 


nmap : Afin de scanner son réseau wifi, il suffit d'installer nmap et taper la commande "nmap -sP <adresse réseau>" dans mon cas : 10.33.0.0/22
Je choisis mon adresse parmis celles de libre, met le masque et la gateway.
-----------------------------------------------------------------------------------------------











