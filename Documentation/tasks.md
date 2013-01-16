Aufgaben des Rahmenprogramms
----------------------------

Das Rahmenprogramm liest die werte aus ui.txt ein und legt sie in zwei Arrays ab.
Dazu werden zwei Arrays f�r die Ergebnisse initialisiert.
Die Pointer und L�ngen der Arrays werden beim Aufruf von calc() �bergeben.
Nachdem die Kapazit�ten berechnet wurden, werden sie auf der Konsole asgegeben.


Aufgabe des Assembler-Teils
------------------------------

Der Assemblerteil des Programms berechnet die angegebene Formel f�r jedes Wertepaar und speichert das Ergebnis im Ausgabearray.

Hierf�r werden mehrere Einsprungpunkte definiert:

- calc
	Liest die n�tigen Werte in feste Register ein und ruft dann _loop_ auf.

- loop
	Holt ein Wertepaar aus den Eingabearrays, ruft zweimal _capacity_ auf (jeweils mit den zwei Dielektrika) und speichert die Ergebnisse in den Ausgabearrays.

- capacity
	Bekommt als Parameter zwei Radien und eine Konstante f�r das Dielektrikum und gibt das Ergebnis zur�ck.

