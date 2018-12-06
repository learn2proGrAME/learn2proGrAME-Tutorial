# Operatoren  - Beispiele überarbeiten

!!!abstract "Lernziele"
    In diesem Kapitel lernst du, was ein Operator ist. Du lernst verschiedene Operatoren kennen und lernst wie du sie in deinem Projekt verwenden kannst. Wenn du nicht mehr weißt welchen Operator du brauchst, kannst du in diesem Kapitel nachschauen.
    

Ein Operator repräsentiert eine Aktion die man mit einer Variable oder einem ganzen Objekt in C*#* durchführen kann. Man könnte sagen, man lässt die zwei Objekte miteinander agieren. Das Ergebnis bestimmt die Art Operator.

<!--Wir beschäftigen uns jetzt mit den wichtigsten Operatoren, die wir beim Spieleprogrammieren brauchen.-->

## Arithmetische Operatoren
Arithmetische Operatoren erlauben uns einfache Berechnungen durchzuführen, fast so wie ein Taschenrechner!

!!!bug "Achtung"
    Arithmetische Operatoren funktionieren in der Regel von Links nach Rechts, aber ignorieren die Punkt vor Strich Regel!
    Du kannst Klammern verwenden, um die Reihenfolge der Berechnung anzugeben. Wie in Mathematik werden Begriffe in Klammern zuerst berechnet. <!--Es ist sehr wichtig Klammern zu setzen, damit nichts falsche berechnet wird.-->


### = Operator 

= ist der **Zuweisungsoperator**. Er speichert was **rechts** davon steht in die Variable links davon. 

<!--!!!tip "Tipp" 
    Zum Initialisieren einer Variable kannst du auch den Zuweisungsoperatoren verwenden.-->

Den Zuweisungsoperator = verwendet man folgendermaßen:

``` c#
//1. Teil
//Wir deklarieren und initialisieren  zuerst einmal unsere Variablen int x und String name.
//In *name* ist "Kein Name" gespeichert. 
String name = "Kein Name";
//In *lieblingszahl* ist die Zahl 1 gespeichert.
int lieblingszahl = 1;

//2. Teil
//Wir weisen wir dem String *name* "Ossi der Elefant" mit dem Zuweisungsoperator = zu.
name = "Ossi der Elefant";
//Ab sofort steht in name "Ossi der Elefant" anstatt "Null".


//Wir weisen dem Integer *lieblingszahl* die Zahl 3 zu.
x = 3
//Ab sofort steht in *lieblingszahl* die Zahl 3 anstatt 1.


Debug.Log ("Hallo ich bin " + name+ " und meine Lieblingszahl ist" + lieblingszahl);
```

!!!success "Arbeitsauftrag"
    Ergänze die Funktion ```OnDisable()``` in HalloElli.cs mit oben stehendem Programm-Code.

In der Konsole steht nach Aufruf: *Hallo ich bin Ossi der Elefant und meine Lieblingszahl ist 3.* 
Wir sehen also, die Werte in x und name sind jetzt anders weil wir neue Werte mit = zugewiesen haben.

### + Operator

Der Additionsoperator + addiert Variablen.

``` c#
int a = 1;      
int b = 2;      
int c = 0;

Debug.Log (a+b);
Debug.Log (" ");
Debug.Log (b+3);

c = a+b;
```

!!!success "Arbeitsauftrag"
    Ergänze die Funktion ```OnEnable()``` in HalloElli.cs mit oben stehendem Programm-Code.

In der Konsole steht nach Aufruf *3 5*. 
3 ist das Ergebnis von *a+b* was wir in c gespeichert haben und ausgeben. 
5 ist das Ergebnis von *b+3* denn in b ist 2 gespeichert.

!!!success "Arbeitsauftrag" 
    Verwende den Additionsparameter + um die Zahlen b und c zu addieren. Gib dein Ergebnis mit Debug.Log() aus. Je nachdem ob du deinen Code vor oder nach "c + a+b" einfügst ist das Ergebnis anders. Warum?

Du kannst den Additionsoperator + auch verwenden, um Strings zu kombinieren.

``` c#
String teil1 = "Wasch";
String teil2 = "maschine";

Debug.Log (teil1 + teil2);
Debug.Log (" Bohr" +teil2);
Debug Log ("Süßes" + " oder " + "Saures");
```
Im Debug Log steht jetzt: *Waschmaschine Bohrmaschine Süßes oder Saures*

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
Den Multiplikationsoperator * verwendet man um 2 Variablen zu multiplizieren.
```
int a = 3
int b = a*5;
Debug.Log(b);
```
Im Debug Log steht jetzt *15*.  

Ohne Klammern:
```
int a = 3
int b = a+2*5;
Debug.Log(b);
```
Im Debug Log steht jetzt *25*.  

Mit Klammern:
```
int a = 3
int b = a+(2*5);
Debug.Log(b);
```
Im Debug Log steht jetzt *13*.  


### / Operator
Den Divisionsoperator / verwendet man um 2 Variablen miteinander zu dividieren. 
Es wird immer die Zahl auf der linken Seite durch die Zahl auf der rechten Seite dividiert.
```
int a = 15
int b = a/3;
Debug.Log(b);
```
Im Debug Log steht jetzt *5*.  
```
int a = 15
int b = a/3+2;
Debug.Log(b);
```
Im Debug Log steht jetzt *7*. 

```
int a = 15
int b = a/(3+2);
Debug.Log(b);
```
Im Debug Log steht jetzt *3*.  

### % Operator

Den Modulo Operator % wird verwendet um Division mit Rest durchzuführen. Das Ergebnis dieser Berechnung ist aber **nur der Restbetrag**.
```
int a = 10
int b = 10%3
Debug.Log(b);
```
Im Debug Log steht jetzt *1*, denn 10 dividiert durch 3 ist 3 + 1 Rest. Der Modulo operator % liefert nur den Rest zurück.



## Logische Operatoren

Logische Operatoren unterscheiden sich von Arithmetischen Operatoren darin, dass sie dir kein Ergebnis an sich zurückgeben, sondern stattdessen angeben ob etwas Wahr oder Falsch ist, wir nennen diesen Wahr oder Falsch Zustand ein boolean. Mit Logischen Operatoren können wir zwei Aussagen zusammensetzen und Abfragen ob das Ergebnis beider Aussagen Wahr oder Falsch ist.

Wie wir die Ergebnisse von logischen Operatoren verwenden lernen wir genauer im Kapitel Verzweigungen.
### NICHT Operator ( ! )
### UND Operator ( && )
### ODER Operator ( || )


!!! danger "Vorsicht!" Wenn du etwas berechnest, aber das Ergebnis nicht sofort weiterverwendest oder einer Variablen zuweist verschwindet es noch vor deinem nächste Programmierbefehl.
