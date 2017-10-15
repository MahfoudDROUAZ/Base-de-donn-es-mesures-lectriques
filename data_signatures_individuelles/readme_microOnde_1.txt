*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : mise en marche d'un micro Onde
	- Type appareil : micro Onde
	- Caractéristiques : consommation 1400watt, four à micro onde 900watt, grill 1000watt, 230v~ 50Hz fréquence du micro onde 2450Hz.
	- Puissance de mise en marche : P100 = 100%, P60 = 60% et P20 = 20%.

*************************************************************************************************

Il est à noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est définit selon la mesure réalisée.

*************************************************************************************************

- Capteur de tension : sonde différentielle ST 1000-II, calibre 1/100
- Capteur de courant : pince ohmétrique Fluke i30 AC/DC 20A RMS max, output = 100mV/A + 2 spires de cable
- CAN : labjack U3HV +/-10V tension et courant

*************************************************************************************************

Nomination du fichier : "data _microOnde_1_PuissanceUtilisation_20KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant

Temps de mise en marche = différente selon des mesures, jusqu'à 15 secondes
Fréquence d'échantillonnage = 20KHz
Le courant et la tension sont a bonne échelle.
**************************************************************************************************

Détails sur les conversions des données depuis les fichiers .dat générés par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit être multipliée par le facteur de la sonde différentielle utilisée.
	- Courent : doit être diviser par le nombre de spires du cable et dévisé par le facteur d'échelle du capteur de courant.