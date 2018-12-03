#Variablen

!!! Abstract "Lernziele"
    In diesem Kapitel lernst du was Variablen beim Programmieren sind. Du lernst, wie du eine Variable erzeugen kannst durch **Deklarieren** und **Initialisieren**. Außerdem lernst du, was **Datentypen** sind.

-----

![Variable Initialisierung](img/variablenBeschr.png)

Das bedeutet: *Der Integer-Variable "meineVariable" wird der Wert 1 zugewiesen.* Man kann auch sagen: *Die Integer-Variable "meineVariable" wird mit dem Wert 1 initialisiert.*

##Wozu Variablen?

* Mit Variablen kannst du Daten speichern und ändern.

Ein Beispiel:
``` c#
int x = 1;
int y = 2;
int z = x + y;
```

!!!success "Übung"
    Welchen Wert hat z?

* Letztlich bezeichnen Variablen einen Speicherplatz.
Man kann sich das etwa wie ein Postfach vorstellen, auf dem eine Address-Bezeichnung steht.

* Diesem Speicherplatz können Werte (also Daten) zugewiesen werden. Zuweisen kann man in C*#* mit dem Zuweisungs-Operator ```=```.

![Variable](img/variableMetaphor.png) 


##Deklarieren und Initialisieren

**Deklarieren** bedeutet, dass man eine Variable benennt und ihr einen **Datentyp** zuordnet. 

Datentypen bezeichnen die Form der Daten, also was die Nullen und Einser in einer Bit-Folge jeweils bedeuten.

!!!tip "Tipp"
    Ein Bit ist die kleinste Einheit, mit der Computer rechnen. Ein Bit ist entweder 0 oder 1. Mit Bits kann man [im Binärsystem rechnen](https://www.studienkreis.de/mathematik/zweiersystem/). 

**Initialisieren** bedeutet, dass man einer Variable einen Wert zuweist.

!!!success "Übung"
    Analysiere folgenden Quellcode. In welcher Zeile wird eine Variable deklariert? Wo wird eine Variable deklariert und initialisiert?
	
	
```
	int x;
	int y = 2;
```
   

## Datentypen

Datentypen zeigen an, welche Art von Daten einer Variable zugewiesen werden können. Sie zeigen an, wie Daten (also Folgen von Nullen und Einsen) interpretiert werden sollen.


###Umwandlung von Datentypen

## Variablen-Bereich (Scope)


##Weiterführende Resourcen