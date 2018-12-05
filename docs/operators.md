# Operatoren

!!! Abstract "Lernziele"
    In diesem Kapitel lernst du, was ein Operator ist. Du lernst verschiedene Operatoren kennen und lernst wie du sie in deinem Projekt verwenden kannst. Wenn du nicht mehr weißt welchen Operator du brauchst, schau in diesem Kapitel nach.
    

Ein Operator repräsentiert eine Aktion die man mit einer Variable oder einem ganzen Objekt in C*#* durchführen kann. Man könnte sagen, man lässt die zwei Objekte miteinander agieren und das gewünschte Ergebnis bestimmt der Operator den man gewählt hat.

In Programmiersprachen gibt es eine große Zahl verschiedener Operatoren und manchmal kann man sogar seine eigenen erstellen. Wir beschränken uns in dem Tutorial aber nur auf die wichtigsten Operatoren die wir zum Spieleprogrammieren brauchen werden. Diese Operatoren können wir in zwei Kategorien aufteilen.
## Arithmetische Operatoren
Arithmetische Operatoren erlauben uns einfache Berechnungen durchzuführen, fast so wie ein Taschenrechner!
### = Operator -- Beispiel überarbeiten

Der = ist der Zuweisungsoperator. Er weißt einer Variable das zu was auf der **rechten** Seite davon im Programmcode steht. 

!!! tip "Hinweis" Beim Initialisieren einer Variable verwenden wir auch den Zuweisungsoperatoren, denn wir geben ihr einen Wert.

Den Zuweisungsoperator = verwendet man folgendermaßen:
```
int x = 1;
String name = "Benjamin";

x = x+3
name = "Ossi der Elefant";
Debug.Log ("Hallo ich bin " + name+ " und meine Lieblingszahl ist" + x;);

```
In der ersten Zeile deklarieren und initialisieren wir die Integer Variable x mit dem Wert 1.
In der zweiten Zeile weisen wir der Variable mit = die Zahl 7 zu.  Ab jetzt steht in ihr 7 und nicht mehr der alte Wert 1.

In der ersten Zeile deklarieren und initialisieren wir den String mit dem Wert "Kein Name".
In der zweiten Zeile weisen wir dem String mit = den Wert "Ossi der Elefant" zu. Ab sofort steht in unserem String name "Ossi der Elefant" anstatt "Kein Name".

Wenn wir das über die Debug Konsole ausgeben steht dort: *Hallo ich bin Ossi der Elefant und meine Lieblingszahl ist 7.* 
Wir sehen also, die Werte in x und name sind jetzt anders weil wir neue mit = zugewiesen haben.

### + Operator

Den Additionsoperator + verwendet man um 2 Variablen zu addieren.
```
int a = 1;      
int b = 2;      
int c = 0;

Debug.Log (a+b);
Debug.Log (" ");
Debug.Log (b+3);

c = a+b;
```
Im Debug Log steht jetzt *3 5*. 
3 ist das Ergebnis von *a+b* was wir in c gespeichert haben und ausgeben. 
5 ist das Ergebnis von *b+3* denn in b ist 2 gespeichert.

!!! success "Aufgabe" Verwende den Additionsparameter + um die Zahlen b und c zu addieren. Gib dein Ergebnis mit Debug.Log() aus. Je nachdem ob du deinen Code vor oder nach "c + a+b" einfügst ist das Ergebnis anders. Warum?

Wir können den Additionsoperator + auch verwenden um Strings zu kombinieren.
```
String teil1 = "Wasch";
String teil2 = "maschine";

Debug.Log (teil1 + teil2);
Debug.Log (" Bohr" +teil2);
Debug Log ("Süßes" + " oder " + "Saures");
```
Wenn wir das über die Debug Konsole ausgeben steht dort: *Waschmaschine Bohrmaschine Süßes oder Saures*

!!! tip "Hinweis" Wenn du Strings kombinierst um einen Satz zu erstellen musst du darauf achten auch Leerzeichen anzufügen, sonst kleben deine Wörter zusammen.
### - Operator
Den Additionsoperator + verwendet man um 2 Variablen zu subtrahieren

```
int a = 3; 
a = a - 2;
Debug.Log(a);
```
Im Debug Log steht jetzt *1*. 


### * Operator
### / Operator
### % Operator



## Logische Operatoren

Logische Operatoren unterscheiden sich von Arithmetischen Operatoren darin, dass sie dir kein Ergebnis an sich zurückgeben, sondern stattdessen die ob etwas Wahr oder Falsch ist, wir nennen diesen Wahr oder Falsch Zustand ein boolean. Mit Logischen Operatoren können wir zwei Aussagen zusammensetzen und Abfragen ob das Ergebnis beider Aussagen Wahr oder Falsch ist.

### UND Operator ( && )
### ODER Operator ( || )


!!! danger "Vorsicht!" Wenn du etwas berechnest, aber das Ergebnis nicht sofort weiterverwendest oder einer Variablen zuweist verschwindet es noch vor deinem nächste Programmierbefehl.
