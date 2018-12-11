#Funktionen

!!! Abstract "Lernziele"

    In diesem Kapitel lernst du was Funktionen beim Programmieren sind. Du lernst, wofür Funktionen verwendet werden, was **Parameter** und **Rückgabewerte** sind und wie du deine eigenen Funktionen schreiben kannst.
-----

<!--!!! Abstract "Hinweis"
    In der Objektorientierten Programmierung wird statt Funktion auch oft der Begriff Methode verwendet.-->
-----

##Wofür braucht man Funktionen?

Funktionen (bzw. Methoden) sind kleine *Unterprogramme*.


Vielleicht musst du für dein Spiel den Abstand zwischen zwei Objekten berechnen? Diese Berechnung benötigt man in den meisten Spielen sehr häufig.

Eine Möglichkeit ist: den dafür nötigen Code jedes Mal eintippen, oder: mit Kopieren und Einfügen überall einzufügen, wo du ihn benötigst. 
Das wäre aber nicht nur sehr viel Arbeit, sondern auch sehr schwer zu warten. Wenn du zum Beispiel später merkst, dass deine Berechnung einen Fehler enthält, musst du an allen Stellen im Programm den Fehler ausbessern.

Eine bessere Möglichkeit ist: 

Du erstellst eine **Funktion**, die den Abstand zwischen zwei Punkten berechnet.

```csharp
   // Diese Funktion berechnet den Abstand zwischen zwei Punkten.
   // x1,y1  ... Koordinaten des ersten Punkts
   // x2,y2  ... Koordinaten des zweiten Punkts
   // return ... Der Abstand zwischen den Punkten
   public int Abstand(float x1, float y1, float x2, float y2){
     //Berechne den Abstand mithilfe des Satzes von Pythagoras c=Wurzel(a^2+b^2)
     float entfernung = Mathf.Sqrt((x1-x2)*(x1-x2)+(y1-y2)*(y1-y2)); //Anm.: Mathf.Sqrt(float f) ist ebenfalls eine Funktion. Sie berechnet die Quadratwurzel einer Zahl f.

     return entfernung;
   }
```
Anstatt nun jedes Mal diese Berechnung *händisch* durchzuführen, kannst du diese Funktion aufrufen.

```csharp
  float entfernung = Abstand(elli.x, elli.y, ossi.x, ossi.y);
```

Außerdem musst du Änderungen nur an einer Stelle, nämlich im Code der Funktion, durchführen.

##Funktionen ohne Rückgabewert



##Funktionen mit Rückgabewert

!!!bug "ACHTUNG"
    Je nach Programmiersprache gibt es unterschiedliche Definitionen der Begriffe *Funktion*, *Prozedur* und *Methode*.
    Oft werden als Funktionen nur jene Methoden mit Rückgabewert bezeichnet (In Anlehnung an den Funktionsbegriff aus der Mathematik). Jene ohne Rückgabewert heißen dann *Prozedur*.
    Im Kontext von C,C++ und C# werden jedoch meist sowohl Methoden mit als auch ohne Rückgabewert als Funktionen bezeichnet.
-----

##Weiterführende Resourcen

* [Variables and Functions Tutorial (englisch)](https://unity3d.com/learn/tutorials/topics/scripting/variables-and-functions)
