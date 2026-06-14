**Aufgabe 2.1:**



**Äquivalenzklassen**



**Fahrradtyp:**

* Gültig: {RACE, SINGLE\_SPEED, FIXIE}
* Ungültig 1: {GRAVEL}
* Ungültig 2: {EBIKE}



**Offener Auftrag des Kunden:**

* Gültig: Kunde hat keinen offenen Auftrag
* Ungültig: Kunde hat bereits einen offenen Auftrag



**Anzahl bestehender offener Aufträge:**

* Gültig: size() ≤ 4` (0,1,2,3,4)
* Ungültig: size() > 4` (5, 6, ...)



**Grenzwertanalyse**

Die Bedingung `pendingOrders.size() > 4` hat die Grenzwerte:

* **4** – letzter gültiger Wert (Auftrag wird angenommen, Queue wächst auf 5)
* **5** – erster ungültiger Wert (Auftrag wird abgelehnt)



**Konkrete Testfälle**

|TC|Fahrradtyp|Kunde hat offenen Auftrag?|Anzahl vorhandener offener Aufträge|Erwartung|Abdeckung|
|-|-|-|-|-|-|
|TC1|RACE|nein|0|true|gültige Klasse Typ (RACE) + alle anderen gültig|
|TC2|SINGLE\_SPEED|nein|0|true|gültige Klasse Typ (SINGLE\_SPEED)|
|TC3|FIXIE|nein|0|true|gültige Klasse Typ (FIXIE)|
|TC4|GRAVEL|nein|0|false|ungültige Klasse Typ (GRAVEL)|
|TC5|EBIKE|nein|0|false|ungültige Klasse Typ (EBIKE)|
|TC6|RACE|ja|0|false|ungültige Klasse "Kunde hat offenen Auftrag"|
|TC7|RACE|nein|4|true|Grenzwert: genau 4 → 5. Auftrag wird noch angenommen|
|TC8|RACE|nein|5|false|Grenzwert: genau 5 → Ablehnung|



