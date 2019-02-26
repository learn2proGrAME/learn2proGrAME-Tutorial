# Teil 10 - Das Spiel veröffentlichen!

Im Moment kann man das Spiel nur über Unity starten. Damit das Spiel auch eigenständig spielbar ist und veröffentlicht werden kann, muss man es noch exportieren.

!!! Abstract "Lernziele"
    In diesem Kapitel lernst du, wie du dein Unityprojekt exportieren kannst, sodass es auch ohne Unity spielbar ist.


## Build & Run

Klicke als erstes auf *File->Build & Run*

![Build&Run](img/T10/T10-build.png)

## Buildsettings

In den Build Settings kannst du nun einstellen für welche Plattform du exportieren möchtest. Hier sollte die Standardeinstellung Windows x86 passen. Wenn du das Spiel für Mac oder Linux exportieren willst, wähle das entsprechende Betriebssystem aus.

![Buildsettings](img/T10/T10-buildSettings.png){: style="height:70%;width:70%"}

!!!Tip "Tipp"
	Wenn du für eine andere Plattform als Windows exportieren willst, kann es sein, dass du zusätzliche Softwarepakete installieren musst. Beispielsweise benötigt man für Android das *Android Software Development Kit* (Android SDK). Außerdem muss man sich für evtl. auch noch einmal um die Eingabe kümmern, da man auf mobilen Endgeräten im Normalfall keine Tastatur hat.

##Playersettings

In den Playersettings kannst du unter anderem festlegen, ob das Spiel standardmäßig im Vollbildmodus und mit welcher Auflösung es gestartet werden soll. (Vollbild solltest du deaktivieren, da es im Moment im Spiel selbst noch keine Möglichkeit gibt das Spiel zu beenden.) Außerdem kannst du auch den Namen und Companyname eingeben.

![Player Settings](img/T10/T10-playerSettings.png){: style="height:40%;width:40%"}

## Build

Wenn du alle Einstellungen vorgenommen hast, klicke in den *Buildsettings* auf *Build*, wähle einen geeigneten Ort, benenne die Datei *Bouncyfant.exe* und klicke auf *Speichern*.

Wenn der Buildvorgang zu Ende ist, findest du in dem von dir festgelegten Ordner die Datei *Bouncyfant.exe* sowie einen Ordner *Bouncyfant_Data*.

![Fertige Spieldateien](img/T10/T10-exportedFiles.png)

## Das Spiel starten und veröffentlichen

Nun kannst du das Spiel mit einem Doppelklick auf Bouncyfant starten. Wenn du das Spiel veröffentlichen, oder einer Freundin/einem Freund geben möchtest, musst du einfach *Bouncyfant.exe* und *Bouncyfant_Data* weitergeben und es kann auf jedem aktuellen Windowscomputer gestartet werden.



