*************************************************************************************************

Mesures de tension/courant:

	- Type de mesure : "ON/OFF".
	- Type appareil : bouilloire �lectrique de marque Dom�os
	- Caract�ristiques : 230V~ 50Hz 1000W

*************************************************************************************************

Il est � noter que : 

Le temps d'acquision varie selon les mesures.
Le temps de mise en marche est d�finit selon la mesure r�alis�e.

*************************************************************************************************

- Capteur de tension : sonde diff�rentielle ST 1000-II, calibre 1/100
- Capteur de courant 1 : pince ohm�trique Fluke i30 AC/DC 20A RMS max, output = 100mV/A + 5 spires de cable
- capteur de courant 2 : capteur ACS 723 20A output = 100mV/A
- CAN : labjack U3HV +/-10V tension et courant

*************************************************************************************************

Nomination du fichier : "data _bouilloire_1_15KHz_mesureX.mat"

Contenu du fichier.mat

Temps  |  tension  |  courant 1 | courant 2

Dur�e de mise en marche = ind�fini
Fr�quence d'�chantillonnage = 15KHz
Le courant et la tension sont a bonne �chelle.
**************************************************************************************************

D�tails sur les conversions des donn�es depuis les fichiers .dat g�n�r�s par l'application LJStreamUD en fichier .mat:

Pour obtenir les bonnes valeurs dans les Fichiers.dat, il faut:

	- Tension : doit �tre multipli�e par le facteur de la sonde diff�rentielle utilis�e *100.
	- Courent : doit �tre diviser par le nombre de spires du cable et d�vis� par le facteur d'�chelle du capteur de courant.