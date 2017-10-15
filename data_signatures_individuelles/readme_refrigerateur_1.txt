*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : ON/OFF.
	- Type appareil : réfrigérateur
	- Caractéristiques : petit modèle

mesure 1 : 2 spires de cable

*************************************************************************************************

Il est à noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est définit selon la mesure réalisée.

*************************************************************************************************

- Capteur de tension : sonde différentielle ST 1000-II, calibre 1/100
- Capteur de courant : pince ohmétrique Fluke i30 AC/DC 20A RMS max, output = 100mV/A + 2 spires de cable
- CAN : labjack U3HV +/-5V tension et courant

*************************************************************************************************

Nomination du fichier : "data _refrigerateur_1_20KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant

Temps de mise en marche = varie selon féchier
Fréquence d'échantillonnage = 20KHz
Le courant et la tension sont a bonne échelle.

**************************************************************************************************

Détails sur les conversions des données depuis les fichiers .dat générés par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit être multipliée par le facteur de la sonde différentielle utilisée.
	- Courent : doit être diviser par le nombre de spires du cable et dévisé par le facteur d'échelle du capteur de courant.