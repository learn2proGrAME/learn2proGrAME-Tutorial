# Operatoren

!!!abstract "Lernziele"
    In diesem Kapitel lernst du, was ein Operator ist. Du lernst verschiedene Operatoren kennen und lernst wie du sie in einem Programm verwendest. Wenn du nicht mehr weißt was die Operatoren tun, kannst du in diesem Kapitel nachschauen.

 Ein Operator ist eine Aktion, die man mit einer oder mehreren Variable(n) oder Objekt(en) durchführen kann.


<!--Das Ergebnis bestimmt die Art Operator.-->

<!--Wir beschäftigen uns jetzt mit den wichtigsten Operatoren, die wir beim Spieleprogrammieren brauchen.-->

----

##Wozu Operatoren?

Mit Operatoren kannst du deine Variablen verändern bzw. neu berechnen. Operatoren entsprechen immer einer Rechenmethode in der Mathematik.



## Arithmetische Operatoren
Arithmetische Operatoren erlauben uns einfache Berechnungen durchzuführen, fast so wie ein Taschenrechner!
!!!bug "ACHTUNG"
    Arithmetische Operatoren rechnen in der Regel von Links nach Rechts. Es gilt Punkt vor Strich Rechnung!
    Du kannst Klammern verwenden, um die Reihenfolge der Berechnung anzugeben. Wie in Mathematik werden Begriffe in Klammern zuerst berechnet. <!--Es ist sehr wichtig Klammern zu setzen, damit nichts falsches berechnet wird.-->


| **Operator** | **Rechenmethode**|
|---------------|----------------|
| + | Addition |
| - | Subtraktion |
| * | Multiplikation |
| / | Division |
| % | Modulo (Rest d. Division) |

----

### = Operator

```=``` ist der **Zuweisungsoperator**. Du verwendest ihn, um ein Ergebnis einer Variable zuzuweisen, d.h. das Ergebnis speichern. Der Operator speichert was **rechts** vom ```=``` steht in die Variable links davon.

``` c#
// = speichert den Wert 3 in der Variable x ab.
x = 3;
```

<!--!!!tip "Tipp"
    Zum Initialisieren einer Variable verwendenn wir auch denZuweisungsoperatoren verwenden.-->

Den Zuweisungsoperator ```=``` verwendet man folgendermaßen:

``` c#
//Wir erstellen eine Variable "lieblingszahl" mit dem Wert 1.
int lieblingszahl = 1;
//Wir verwenden = und weisen lieblingszahl einen neuen Wert zu.
lieblingszahl = 3;
//Ab sofort steht in *lieblingszahl* die Zahl 3 anstatt 1.
Debug.Log ("Hallo, meine Lieblingszahl ist" + lieblingszahl);
```
In der Konsole steht nach Aufruf: *"Hallo, meine Lieblingszahl ist 3"*
Wir sehen also, der Wert ```lieblingszahl``` und ```name``` sind jetzt anders, weil wir einen neuen Wert mit dem Operator ```=``` zugewiesen haben.

----

### ```+``` Operator

Der **Additionsoperator** ```+``` addiert Variablen. Du kannst damit die Summe von Variablen berechnen.

``` c#
int a = 1;      
int b = 2;      
int c = 0;

Debug.Log (a+b);
Debug.Log (" ");
Debug.Log (b+3);

c = a+b;
```
In der Konsole steht nach Aufruf *"3 5"*.
3 ist das Ergebnis von *"a+b"* was wir in c gespeichert haben und ausgeben.
5 ist das Ergebnis von *"b+3"* denn in b ist 2 gespeichert.

!!!success "Arbeitsauftrag"
    Verwende den Additionsparameter ```+``` um die Zahlen b und c zu addieren. Gib dein Ergebnis mit Debug.Log() aus. Je nachdem ob du deinen Code vor oder nach ```c = a+b``` einfügst ist das Ergebnis anders. Warum?

Du kannst den Additionsoperator ```+``` auch verwenden, um Strings zu kombinieren.

``` c#
String teil1 = "Wasch";
String teil2 = "maschine";

Debug.Log (teil1 + teil2);
Debug.Log (" Bohr" +teil2);
Debug.Log ("Süßes" + " oder " + "Saures");
```
In der Konsole steht jetzt: *Waschmaschine Bohrmaschine Süßes oder Saures*

!!!success "Arbeitsauftrag"
    Verwende den Additionsparameter ```+``` um einzelne Wörter (```Strings```) zu einem Satz zu verbinden. Gib dein Ergebnis mit Debug.Log() aus.
!!!tip "Tipp"
    Wenn du Strings kombinierst, um einen Satz zu erstellen, musst du Leerzeichen anfügen. Sonst kleben die Wörter zusammen.
----

### ```-``` Operator
Den **Subtraktionsoperator** ```-``` verwendet man um 2 Variablen zu subtrahieren. Die Rechte Zahl wird von der Linken abgezogen.

``` c#
int a = 3;
a = a - 2;
Debug.Log(a);
```
In der Konsole steht nach dem Ausführen *1*.

----

### ```*``` Operator
Den **Multiplikationsoperator** ```*``` verwendet man um 2 Variablen zu multiplizieren. Vergiss nicht Klammern zu verwenden damit du auch wirklich das berechnest was du vor hast.

``` c#
int a = 3;
int b = a*5;
Debug.Log(b);
```

In der Konsole steht nach dem Ausführen *15*.  

* Ohne Klammern:
``` c#
int a = 3;
int b = a+2*5;
Debug.Log(b);
```
In der Konsole steht nach dem Ausführen *13*.  

----

### ```/``` Operator
Den **Divisionsoperator** ```/``` verwendet man um 2 Variablen miteinander zu dividieren.
``` c#
int a = 15;
int b = a/3;
Debug.Log(b);
```
In der Konsole steht nach dem Ausführen *5*.  
!!!bug "ACHTUNG"
    Es gilt Punkt vor Strich Rechnung. Pass also auf, dass du die richtigen Klammern setzt.
``` c#
int a = 15;
int b = a/3+2;
Debug.Log(b);
```
In der Konsole steht nach dem Ausführen *7*.

``` c#
int a = 15;
int b = a/(3+2);
Debug.Log(b);
```
In der Konsole steht nach dem Ausführen *3*.  

----

### % Operator

Der **Modulo** Operator ```%``` wird verwendet, um eine Division mit Rest durchzuführen. Das Ergebnis dieser Berechnung ist aber **nur der Restbetrag**.

```c#
int a = 10;
int b = 10%3;
Debug.Log(b);
```
In der Konsole steht nach dem Ausführen *1*, denn 10 dividiert durch 3 ist 3 + 1 Rest. Der **Modulo** Operator ```%``` liefert nur den Rest zurück.

----

## Logische Operatoren

Die Auswertung von **logischen Operatoren**
gibt an, ob ein logischer Ausdruck (auch genannt ```boolean``` nach George Boole)- oder eine Verknüpfung mehrerer  Wahr (true) oder Falsch (false) ist.  Mit diesen Operatoren kann man also Bedingungen schreiben. In einigen Programmiersprachen werden statt ```true``` und ```false``` auch die int-Zahlenwerte 1 und 0 akzeptiert.

Logischen Operatoren sind besonders wichtig bei [Verzweigungen](T08-conditionals.md). Wie noch gezeigt wird, wird der Code innerhalb einer Verzweigung nur ausgeführt, wenn die Bedinung Wahr ergibt.



| Vergleichsoperator | Bedeutung          |
| ------------------ | ------------------ |
| >                  | ist größer als     |
| >                  | ist kleiner als    |
| >=                 | ist größer gleich  |
| <=                 | ist kleiner gleich |

Neben den Vergleichsoperatoren in der oberen Tabelle die du bestimmt aus dem Mathematikunterricht kennst gibt es noch weitere Operatoren die wir beim Programmieren brauchen.

| Vergleichsoperator | Funktion |
|----------|----------|
| ```&&``` | UND |
| ```||``` | ODER |
| ```!```  | NICHT |
| ```==``` | GLEICH |
| ```!=``` | UNGLEICH |


!!!Tip "Tipp"
	Wenn es dir schwer fällt diese Operatoren zu verstehen, stell dir am besten immer die Frage:"Ist dieser Ausdruck wahr? Falls ja, ist das Ergebnis ```true```. Falls nein, ist das Ergebnis ```false```. Zum Beispiel bei dem Begriff ``` 5 < 10``` fragst du dich: "Ist 5 kleiner als 10?" - "Ja." Das Ergebnis ist also ```true```.


----
### ```&&``` Operator (UND)
Der ```&&``` Operator wird verwendet um Aussagen zu verknüpfen. Damit der zusammengesetzte Begriff in der Klammer ```true``` ergibt müssen alle mit ```&&``` verknüpften Aussagen ```true``` sein.
``` c#
int a = 2
(a < 3) && ( a < 5)   // Dieser Ausdruck ergibt true, weil beide Aussagen wahr sind.

(a < 1) && ( a < 5)   // Dieser Ausdruck ergibt false, weil zumindest eine der beiden Aussagen falsch ist.
```
----

### ```|| ``` Operator (ODER)
Der ```||``` Operator wird verwendet um Aussagen zu verknüpfen. Damit der zusammengesetzte Begriff in der Klammer ```true``` ergibt muss mindestens eine Aussage ```true``` sein. Nur wenn keine einzige ```true``` Aussage ist, ist der gesamte Begriff ```false```.
``` c#
int a = 2
(a < 3) || ( a < 5)   // Dieser Ausdruck ergibt true, da zumindest eine Aussage wahr ist.
(a < 1) || ( a > 100)   // Dieser Ausdruck ergibt false, weil ALLE Aussagen falsch ist.
```
----
### ```!``` Operator (NICHT)
Wenn du den ```!``` Operator vor einen Ausdruck schreibst, drehst du du das Ergebnis um wie am Gegenteil Tag.
``` c#
int a = 2
(a < 0)   // Dieser Ausdruck ergibt false.
!(a < 0)  // Dieser Ausdruck ergibt true, weil der NOT Operator das Ergebnis umdreht.

(a < 1) || ( a > 100)   // Dieser Ausdruck ergibt false, weil ALLE Aussagen falsch ist.
```
----
### ```==``` Operator (GLEICH)
Der ```==``` Operator prüft ob die Ausdrücke auf beiden Seiten identisch oder gleich sind. Er gibt ```true``` zurück wenn sie gleich sind und ```false``` wenn sie nicht gleich sind.

``` c#
int a = 2
(a == 2)   	// Dieser Ausdruck ergibt true.
(10 == 10) 	// Auch das ergibt true.
(a == 5) 	// Das ergibt false, weil der Wert in a (2) nicht gleich 5 ist.
```
----
### ```!=``` Operator (NICHT GLEICH)
Der ```!=``` Operator prüft ob die Ausdrücke auf beiden Seiten nicht gleich sind. Er gibt ```false``` zurück wenn sie gleich sind und ```true``` wenn sie nicht gleich sind.
``` c#
int a = 2
(a != 2)   	// Dieser Ausdruck ergibt false.
(10 != 10) 	// Auch false.
(a != 5) 	// Das ergibt true, weil der Wert in a (2) nicht gleich 5 ist.
```
----
