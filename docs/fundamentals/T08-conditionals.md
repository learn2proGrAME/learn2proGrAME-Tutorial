#Verzweigungen

!!!abstract "Lernziele"
    In diesem Kapitel lernst du **Verzweigungen** kennen. **If (Wenn)** Abfragen erlauben, den Programmfluss zu steuern. Du lernst, wie diese Kontrollstruktur erzeugt werden kann, und wie **Bedingungen** formuliert werden.

![Verzweigung](img/conditional.png)

---

##Wenn (if) - Sonst (else)

``` C#

if(Bedingung) //kann wahr oder falsch sein
{
	//Hier schreibst du, was passieren soll, wenn die Bedingung wahr ist
}
else
{
	//Hier schreibst du, was passieren soll, wenn die Bedingung falsch ist
}

```

###Ein Beispiel

``` C#

String passwort = "meinPasswort";

if(passwort == "PASS")
{
	Debug.Log("Access granted.");
}
else
{
	Debug.Log("Access denied.");
}

```

!!!success "Arbeitsauftrag"
    Ergänze die Funktion ```OnDisable()``` im Projekt "HalloElli" in "HalloElli.cs" mit oben angeführtem Beispiel. Verändere den Programmcode, sodass in der Konsole beim Ausführen der Funktion "Access granted." steht.

---

###Vergleichsoperatoren

Um als Bedingung zwei Ausdrücke miteinander zu vergleichen, können Vergleichsoperatoren verwendet werden. In C*#* kannst du folgende Vergleichsoperatoren verwenden:

| Vergleichsoperator | Bedeutung          |
| ------------------ | ------------------ |
| ```==```           | ist gleich         |
| ```!=```           | ist ungleich       |
| ```>```            | ist größer als     |
| ```>```            | ist kleiner als    |
| ```>=```           | ist größer gleich  |
| ```<=```           | ist kleiner gleich |

!!!bug "ACHTUNG"
    Ein Vergleich gibt als Ergebnis einen Wahrheitswert (wahr/falsch) - einen Boolean - zurück.

---

###Logische Operatoren

[Logische Operatoren](T05-operators.md) ermöglichen komplexere Bedingungen, indem Verknüpfungen von Wahrheitswerten erstellt werden können.
Häufig verwendete logische Operatoren sind:

| Logische Operatoren | Bedeutung          |
| ------------------- | ------------------ |
| ```!```             | nicht              |
| ```&&```            | und                |
| ```||```            | oder               |


---

###Verknüpfungen von Bedingungen - Beispiel

``` C#

int elefantenAnzahl;//die Variable "elefantenAnzahl" wird deklariert
elefantenAnzahl = 8;//die Variable "elefantenAnzahl" wird mit dem Integer-Wert 8 initialisiert.

void OnDisable() //Funkionsdefinition
{
	if(elefantenAnzahl > -1 && elefantenAnzahl < 5)
	{
		if(elefantenAnzahl == 0)
		{
			Debug.Log("Keine Elefanten hier.");
		}
		else if (elefantenAnzahl == 1) //Ein oder mehrere Else If können eine If-Abfrage ergänzen.
		{
			Debug.Log("Ein Elefant im Spiel.");
		}
		else
		{
			Debug.Log("Juhu! Endlich mehrere Elefanten!");
		}
	}
	else
	{
		Debug.Log("Bisher können nur 0 bis 4 Elefanten im Spiel sein.");
	}
}

```

!!!success "Übung"
	Was ist der Unterschied zwischen mehreren **if**-Abfragen hintereinander und mehreren **else if**-Abfragen hintereinander nach einem **if**?

---

###Verschachtelte Bedingungen - Beispiel

``` C#
bool ersterWahrheitswert = true;
bool zweiterWahrheitswert = false;
int spielerInnen = 4;

//In der nachfolgenden Verzweigung ist der "ersterWahrheitswert" die erste Bedingung der ODER-Verknüpfung, die Klammer der zweite.
//Nur wenn sowohl "zweiterWahrheitswert" wahr ist und "spielerInnen" größer 1 ist, ist die zweite Bedingung wahr.
//ODER bedeutet, dass eine der beiden Bedingungen wahr sein muss, damit die Verknüpfung wahr ist.
if(ersterWahrheitswert || (zweiterWahrheitswert && spielerInnen > 1))
{
	Debug.Log("Stimmt!");
}
```

!!!success "Arbeitsauftrag"
    Ergänze die Funktion ```OnDisable()``` im Projekt "HalloElli" in "HalloElli.cs" mit oben angeführtem Beispiel. Verändere den Programmcode.

!!!success "Arbeitsauftrag"
    De-Bugge folgenden Quellcode, sodass auf der Konsole 42 ausgegeben wird.


``` C#
bool sollFortsetzen = true;

void OnDisable()
{
	int wert = 46;
	bool sollFortsetzen = false;
	if (sollFortsetzen)
	{
		int neuerWert = 6;
	}
	Debug.Log((wert + neuerWert) + " = 42.");
}

```

!!!bug "ACHTUNG"
    Beachte den Gültigkeits-Bereich der Varialben! Siehe dazu auch [Variablen-Bereich (Scope)](T04-variables.md).

---

##Weiterführende Resourcen

* [IF-Statements Video-Tutorial in Unity (englisch)](https://unity3d.com/learn/tutorials/topics/scripting/if-statements)
