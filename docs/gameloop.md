#Die Spielschleife

##Was ist eine Spielschleife?

In einer Spielschleife werden neben Kollisionsabfragen und der Bewegungsteuerung sogar noch viel grundlegendere Dinge, wie etwa das Zeichnen des Spieleinhalts erledigt. Eine Spielschleife ist eine Schleife, die fortlaufend wieder wiederholt wird und eine Handvoll wichtiger Grundfunktionen für ein Spiel beinhaltet. Eine typische Spielschleife sieht vom Konzept her etwa folgendermaßen aus:

![Grafik einer Spielschleife](img/GameLoop.png)

##Weshalb benötigt man eine Spielschleife?
Die Spielschleife sorgt dafür, dass Ereignisse, die zum Spiel gehören, fortlaufend stattfinden. 
Frage: "Kann man die Spielschleife nicht einfach selbst mit einer While-Schleife implementieren?" 
Antwort: "Möglich ist das schon, aber die Spielschleife von Spieleentwicklungswerkzeugen beinhaltet auch Geschwindigkeitsoptimierungen, d.h. sie trägt die Verantwortung dafür, dass Spiele in der uns bekannten Geschwindigkeit auf gängiger Hardware ablaufen können. Mit einer selbstgemachten, nicht-optimierten Spielschleife, kann es leicht passieren, dass Spieler und Spielerinnen in einem halbwegs komplexen Spiel gerade mal alle 30 Sekunden einen Schritt machen können - Nicht gerade der größte Spielspaß!"

Ein weiteres Problem ist, dass das Spiel auf unterschiedlicher Hardware unterschiedlich schnell läuft. Um eine professionelle Implementierung einer Spielschleife kommt man in der Spieleentwicklung nicht herum. 


##Einklinken in die Spielschleife in Unity

Folgende Funktionen eines Spielobjekt-Skripts werden in der Unity-Spielschleife ausgeführt:




Eine genaue Beschreibung der Funktionen findest du in der [offiziellen Unity Programmier-Referenz](https://docs.unity3d.com/ScriptReference/).