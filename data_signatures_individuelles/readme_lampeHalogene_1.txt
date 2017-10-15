*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : ON/OFF d'une lampe halogène
	- Type appareil : lampe halogène
	- Caractéristiques : 60-500 watt max, courant, tension ... etc

*************************************************************************************************

Il est à noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est définit selon la mesure réalisée.

*************************************************************************************************

- Capteur de tension : sonde différentielle ST 1000-II, calibre 1/100
- Capteur de courant : pince ohmétrique Flukei30 AC/DC 20A RMS max, output = 100mV/A + 10 spires du cable
	mesure 1, 2 et 3
- Capteur de courant : pince ohmétrique PR20 AC/DC 20A RMS max, output = 100mV/A + 10 spires du cable
	mesure 4, 5 et 6
- CAN : labjack U3HV +/-10V tension et courant

*************************************************************************************************

Nomination du fichier : "data _lampeHalogene_1_20KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant

Temps de mise en marche = 2 secondes
Fréquence d'échantillonnage = 20KHz
Le courant et la tension sont a bonne échelle.
**************************************************************************************************

Détails sur les conversions des données depuis les fichiers .dat générés par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit être multipliée par le facteur de la sonde différentielle utilisée.
	- Courent : doit être diviser par le nombre de spires du cable et dévisé par le facteur d'échelle du capteur de courant.