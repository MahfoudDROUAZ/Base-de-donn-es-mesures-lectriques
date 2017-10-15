*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : "ON/OFF".
	- Type appareil : bouilloire électrique de marque Doméos
	- Caractéristiques : 230V~ 50Hz 1000W

*************************************************************************************************

Il est à noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est définit selon la mesure réalisée.

*************************************************************************************************

- Capteur de tension : sonde différentielle ST 1000-II, calibre 1/100
- Capteur de courant 1 : pince ohmétrique Fluke i30 AC/DC 20A RMS max, output = 100mV/A + 5 spires de cable
- capteur de courant 2 : capteur ACS 723 20A output = 100mV/A
- CAN : labjack U3HV +/-10V tension et courant

*************************************************************************************************

Nomination du fichier : "data _bouilloire_1_15KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant 1 | courant 2

Durée de mise en marche = indéfini
Fréquence d'échantillonnage = 15KHz
Le courant et la tension sont a bonne échelle.
**************************************************************************************************

Détails sur les conversions des données depuis les fichiers .dat générés par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit être multipliée par le facteur de la sonde différentielle utilisée *100.
	- Courent : doit être diviser par le nombre de spires du cable et dévisé par le facteur d'échelle du capteur de courant.