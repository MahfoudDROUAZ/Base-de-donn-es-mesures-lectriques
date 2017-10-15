*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : mise sous tension d'un pc portable est déjà en marche à 49% de charge
	- Type d'appareil : pc portable
	- Caractéristiques : 100-240V~ 1.7A 50-60Hz

*************************************************************************************************

Il est à noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est définit selon la mesure réalisée.

*************************************************************************************************

- Capteur de tension : sonde différentielle ST 1000-II, calibre 1/100
- Capteur de courant : pince ohmétrique Fluke i30 AC/DC 20A RMS max, output = 100mV/A + 10 spires cable
- CAN : labjack U3HV +/-5V tension et courant

*************************************************************************************************

Nomination du fichier : "data _pcPOrtable_1_20KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant

Temps de mise en marche = 20 secondes
Fréquence d'échantillonnage = 20KHz
Le courant et la tension sont a bonne échelle.

**************************************************************************************************

Détails sur les conversions des données depuis les fichiers .dat générés par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit être multipliée par le facteur de la sonde différentielle utilisée.
	- Courent : doit être diviser par le nombre de spires du cable et dévisé par le facteur d'échelle du capteur de courant.