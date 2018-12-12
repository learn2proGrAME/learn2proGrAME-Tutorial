#Unity Transform Spielobjektkomponente

!!!abstract "Lernziele"
     Hier lernst du die wichtigste Spielobjekt-Komponente in Unity kennen: **Transform**.

----

Jedes Spielobjekt (GameObject) in Unity hat die Komponente **Transform** (oder **RectTransform** bei User Interface GameObjects).

##Eigenschaften von Transform

Mit **Transform** können

* die **Position** eines Spielobjekts, 
* **Drehungen** und 
* die Größe, oder **Skalierung**, 

eines Spielobjekts definiert werden.

Alle 3 Eigenschaften haben einen x-, y-, und z-Wert. 

In 2D-Spielen sind vor allem x-, und y-Werte wichtig.

* Bei **Position** stehen diese Werte jeweils für eine Koordinate im Koordinatensystem der **Szene**.

* Bei **Rotation** stehen die Werte für die Drehung des Spielobjekts um die X-Achse, die Y-Achse und die Z-Achse. Die Werte werden hierbei als Winkel *in Grad* angegeben. In 2D-Spielen kann vor allem eine Drehung um die Z-Achse effektiv eingesetzt werden.

* Bei **Scale** geht es um die relative Größe eines Spielobjekts. Standardmäßig ist hier der Wert 1 gesetzt. Werte sind hier als Veränderungs-Faktoren zum Standardwert zu verstehen.

Klarerweise können die Werte der Eigenschaften der Transform-Komponente in einem C*#*-Skript verändert werden.

##Krapfenklicker Erweiterung

Die Mehlspeise größer werden, wenn man darauf klickt! 

Wie kann man das programmieren?

![Donut Clicker Extension](img/donutclickerextension.gif)

Im GameController Spielobjekt des Krapfenklicker Spiels hast du bereits eine Variable angelegt, in der das Krapfen Spielobjekt gespeichert ist: ```public Button clickButton;```.

!!!bug "ACHTUNG"
    ```public``` bedeutet, dass diese Variable für andere Teile des eigenen Spiels (und damit in Unity) aufscheint und beschreibbar ist. Deshalb kannst du dem Skript in Unity ein Spielobjekt zuweisen. Siehe hierfür die [Fertigstellung des Krapfenklicker Spiels](donutclicker.md)!

