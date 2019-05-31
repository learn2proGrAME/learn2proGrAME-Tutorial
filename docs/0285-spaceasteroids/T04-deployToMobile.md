#Spiele für Android exportieren

!!! Abstract "Lernziele"

    In diesem Kapitel lernst du wie du ein Unity Projekt für Android veröffentlichst.
-----

##Voraussetzungen

Android SDK, sowie Java JDK 1.8 (Höhere Versionen werden zur Zeit nicht ohne weiteres unterstützt) müssen installiert sein.   **Wichtig:** In Unity muss unter *Edit->Preferences* der Pfad zu diesen Paketen angegegeben werden.

##Zielplatform ändern
Gehe zu *File->Build Settings* und wähle als Platform Android aus.

##Live Testen mit Unity-Remote
Wenn du dein Spiel während dem arbeiten auf dem Smartphone testen willst, kannst du die *Unity-Remote* App auf deinem Smartphone installieren. (Die App Findest du im PlayStore)

Damit die App funtkioniert musst du allerdings *USB-Debugging* auf deinem Android-Smartphone aktivieren. Außerdem musst du unter *Edit->Project Settings->Editor* bei *Device* *Any Anrdoid Device* einstellen. Starte danach Unity neu.

Wenn du nun Play drückst, dein Smartphone an den PC angeschlossen ist und die Unity-Remote läuft, sollte das Spiel auch auf deinem Smartphone laufen.

##Spiel exportieren

Um das Spiel nun für das Smartphone zu exportieren gehe wieder auf *File->Build Settings*. Klicke dann auf *Player Settings* und gib einen Companyname und Productname für dein Spiel ein. Setze dann unter *Other Settings* den Package Name auf "com.*deinProductName*.*deinCompanyName*" (ohne Anführungszeichen)

Stelle nun sicher, dass die Spielszene in *Scenes in Build* eingefügt ist.
![scenes einfügen](img/insertScene.png)

Nun kannst du auf *Build and Run* klicken um das Spiel zu erstellen und auf dein Smartphone zu laden.

Häufige Fehler, weshalb das exportieren nicht funktioniert:
* Packagename nicht richtig gesetzt
* Android-SDK, JDK nicht installiert bzw. Pfad nicht oder falsch gesetzt
* USB-Debugging ist am Smartphone nicht aktiviert


Wenn alles funktioniert, sollte dein Spiel nun am Smartphone laufen. Allerdings hast du noch keine Möglichkeit das Raumschiff zu steuern. Darum kümmern wir uns im nächsten Kapitel.
