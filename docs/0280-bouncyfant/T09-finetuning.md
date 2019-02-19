# Teil 9 - Finetuning

!!!Abstract "Ziele"
    Einen Platform Effector hinzufügen, damit die Figur nicht an der Wand hängen bleibt.

In diesem Kapitel wirst du... | Erledigt?
----------------------------- | ----------
Lernen wie man einen PlatformEffector verwendet |


## Platform Effector
Momentan ist das Spiel schon ganz gut spielbar, doch eine Kleinigkeit trübt noch die Freude. Wenn man mit dem Elefanten gegen die Wand springt und dann gleichzeitig die Richtungstaste weiter in diese Richtung gedrückt hält, dann bleibt die Spielfigur in der Luft hängen.

![Ossi bleibt hängen](img/T09/T09-a0-Ossi haengt.gif)

Um das Hängenbleiben zu vermeiden, bringen wir einen *Platform Effector* zum Einsatz. Dazu klicken wir zuerst im der Hierarchy auf die *Spielfeldgrenzen* und dann im Inspector auf *Add Component/Physics 2D/Platform Effector 2D*

![PlatformEffektor hinzufügen](img/T09/T09-a-a-Plattform Effector erstellen.png)
![PlatformEffector hinzufügen](img/T09/T09-a-Plattform Effector erstellen.png)

Haben wir den Effector den Spielfeldgrenzen hinzugefügt, erhalten wir vorerst noch eine Warnung, dass der Effector erst funktionieren wird, wenn er von einem Collider verwendet wird.

![Warnung](img/T09/T09-b-Effector Warning.png)

Daher klicken wir bei den entsprechenden Spielfeldgrenzen, nämlich den Wänden links und rechts, einfach auf *Used by Effector* und schon sollte der Elefant, wenn wir das Spiel starten,nicht mehr in der Wand hängen bleiben, sondern nach unten rutschen.

![PlatformEffector verwenden](img/T09/T09-c-Plattform Effector verwenden.png)

##Sourcecode

Download Sourcecode Teil 09: [http://comber.at/dev/BouncyFant09.zip](http://comber.at/dev/BouncyFant09.zip)

Für’s erste war es das einmal mit unserem Tutorial. Schön, dass ihr dabei wart. Man könnte auch sagen, jetzt geht es erst richtig los: Neue Levels, neue Features, neue Spielfiguren, …  
Lasst eurer Fantasie freien Lauf.

**Have Fun!**
