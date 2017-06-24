QKan - Umgang mit Flächenarten
==============================

Die Oberfläche wird durch 2 Gruppen von Parametern charakterisiert: Oberflächenverluste und Versickerungsparameter. 
Dies sind in HYSTEM-EXTRAN:

Oberflächenverluste:
- Muldenverlust
- Anfangsmuldenfüllung (Default: 0)
- Verdunstungsverlust
- Anfangsverdunstungsverlust
- Anfangsabflussbeiwert
- Endabflussbeiwert
- Dauerverlust

Versickerungsparameter:
- Anfangsinfiltrationsrate
- Endinfiltrationsrate
- Startwert Infiltrationsrate
- Rückgangskonstante
- Regenerationskonstante

In HYSTEM-EXTRAN sind die beiden Gruppen auf zwei Tabelle aufgeteilt, wobei die Oberflächenverluste auf die Tabelle der 
Versickerungsparameter unter dem Namen "Bodenklasse" verweisen. 

In QKan werden die Werte ebenfalls in zwei Tabellen verwaltet. Befestigte Flächen sind dadurch gekennzeichnet, dass sie
auf einen Datensatz mit Versickerungsparametern mit dem Wert 0 verweisen. Hier wird eine entsprechende 
Bezeichnung "befestigt" empfohlen. 


Befestigte und unbefestigte Flächen
===================================

In der Praxis werden nur die befestigten Flächen erfasst. Die unbefestigten Flächen stellen sich als Zwischenräume dar. 
In QKan werden die unbefestigten Flächen mit Hilfe der Teileinzugsgebietsflächen verwaltet. Nachdem die befestigten 
Flächen in der Tabelle "flaechen" erstellt sind, können mit Hilfe des Plugins "Erzeuge unbefestigte Flächen" für jede
tezg-Fläche ein unbefestigtes Flächenobjekt erzeugt werden, das genau die Lücken zwischen der Teileinzugsgebietsläche 
(Tabelle "tezg") und den darin enthaltenen Flächenobjekten (Tabelle "flaechen") ausfüllt. Dabei werdern alle Parameter 
zu den Oberflächeneigenschaften einschließlich der Bodenklasse aus den Teileinzugsgebieten (Tabelle "tezg") übernommen. 
