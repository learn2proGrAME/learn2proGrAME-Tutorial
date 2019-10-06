#Fertige Partikelsysteme verwenden

!!! Abstract "Lernziele"

    In diesem Kapitel lernst du wie du die vorgefertigten Partikelsystem von Unity importierst und wie du sie in deinem Spiel verwenden kannst.
-----

Falls du die Tutorials [Programmierung der Asteroiden](T01-spaceasteroids.md) und [Partikelsysteme erstellen](T02-particles1.md) schon absolviert hast, verwende nun dieses Unityprojekt, ansonsten kannst du dir [hier](https://github.com/learn2proGrAME/proGrAME-Beispiele-und-Quellcodes/blob/master/SpaceAsteroids/SpaceAsteroids3.zip) das Projekt herunterladen.

##Particle-Package importierten
Unity hat standardmäßig schon eine Reihe von tollen Extrapackages eingebaut, die man ganz einfach für die eigenen Spiele verwenden kann. So zum Beispiel auch ein Particle-Package.


Um das Package zu importieren klicke auf *Assets->Import Package->ParticleSystems*. Nach einigen Sekunden öffnet sich ein Fenster, klicke dort auf *import*.


Wenn der Import abgeschlossen ist, findest du im Assetsbereich einen neuen Ordner namens *Standard Assets*

Navigiere dort in den Unterordner *Standard Assets->ParticleSystems->Prefabs*. In diesem Ordner sind die Vorlagen (*Prefabs*) für Spielobjekte, welche die enstprechenden Partikelsysteme enthalten.

Probiere einfach einmal ein paar aus, indem du sie in deine Sceneview oder die Hierarchy ziehst.

![Prefabs testen](img/prefabstest.png)

Lösche dann die nicht benötigten Objekte wieder aus der Hierarchy.

##Explosionen ins Spiel einbauen

Nun wollen wir die vorgefertigte Explosion ins Spiel einbauen. Jedes Mal wenn ein Asteroid oder das Raumschiff der Spielerin/des Spielers zerstört wird soll eine Explosion erzeugt werden.

Alles was du dafür tun musst, ist:

1. Öffne die Scripts *PlayerController* und *Asteroid*
2. Erstelle in beiden Scripts jeweils eine *public* Variable vom Typ *GameObject* mit dem Namen *explosionseffekt*
3. Nun kannst du mit dem Befehl ```Instantiate(explosionseffekt, transform.position, Quaternion.identity); ``` eine neue Instanz des Explosionseffekts erzeugen. Füge diesen Befehl in beiden Scripts in die Methode *OnTriggerEnter* so ein, dass eine Explosion erzeugt wird, wenn das Raumschiff, bzw. der Asteroid zerstört wird.
4. Speichere das Skript, gehe wieder zu Unity.
5. Wähle das Player Objekt in der Hierarchy aus und weise im Inspector der Variable *explosionseffekt* die Vorlage *Explosion* zu.  
![explosion zuweisen1](img/explosionseffektzuweisenPlayer.png)
6. Wähle die Vorlage Asteroid (Assets->Vorlagen) aus und weise der Variable *explosionseffekt* die Vorlage *ExplosionMobile* zu.  
![explosion zuweisen2](img/explosionseffektzuweisenAsteroid.png)

**Fertig!**

![Explosionseffekte eingebaut](img/finalExplosions.gif)
