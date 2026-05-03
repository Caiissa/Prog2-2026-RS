### **Git-Quest**



**1.**

**Was passierte an tag 01?**

Befehle:

git log

git show 33845cec817c47133b15deff3eb796a148ece6e4



Antwort:

+# Questlog

\+

+In einer düsteren und mysteriösen Welt wagte sich ein furchtloser Held namens Markus in einen gefährlichen Dungeon. Es wurde erzählt, dass in diesem Dungeon Monster lauerten, die die Kerkerebenen terrorisierten. Markus war jedoch fest entschlossen, die Monster zu besiegen und das Amulet zu finden.



**Wann hat der Held zum ersten Mal 4 experience Punkte?**

Befehle:

git log stats.md

git show 590fc86774940ef8f05ef6087df9e2e67ecd4001



Antwort:

Tag 01.3



**Wann hat der Held zum ersten Mal 10 hunger Punkte?**

Befehle:

git log stats.md

git show 78f1f499f45451fd3df76c5bbe4b307f48766375



Antwort:

Tag 02



**Wie viele Heiltränke hat der Held insgesamt in seinem Rucksack gehabt?**

Befehle:

git log rucksack.md

git show 13834cd8d9765750e4e520baf2dc7fa2a22af53d

git show 8f88b193ef4365f25bd910ed54f8c035765af5c4



Antwort:

2 Heiltränke





**Was hat der Held im Shop gekauft? Und wie viel Gold hat er dafür bezahlt?**

Befehle:

git log rucksack.md

git show 4ff87262b423cc991268844d1fda3ba09a03ac82

git show ec66cfc258761a63f9074f954959f7dbe881abac



Antwort:

5 Gold für 1 Brot

5 Gold für 1 Heiltrank



**Was passierte zwischen tag 03 und tag 04, d.h. was änderte sich zwischen diesen Commits?**

Befehle:

git log

git diff 2ffebcfd908ad2abcc619429157b0832dac0dad3 39568d5e84832a2f168f3f473a612bc373e1bb63



Antwort:
Mit seinem Schwert in der Hand und und einer leichten Rüstung bekleidet stieg M

&#x20;Immer wieder stieß Markus auf verschiedene Monster wie Goblins, Gnolle und sogar einen gefährlichen Schlammklumpen. Jeder Kampf war ein harter und erbitterter Kampf, bei dem Markus an seine Grenzen ging. Doch sein Wille, seine Quest zu erfüllen und das Amulet zu finden, gab ihm die Kraft, weiterzumachen.



&#x20;Schließlich erreichte Markus einen versteckten Raum im Dungeon, in dem ein mysteriöser alter Zwerg auf ihn wartete. Dieser Zwerg entpuppte sich als ein Händler und besaß einen kleinen Shop, in dem er nützliche Gegenstände und Lebensmittel verkaufte. Markus trat ein und begann mit dem Zwerg zu verhandeln.

\+

+Erfrischt und gestärkt machte sich Markus auf den Weg, um die letzte Etappe seiner Quest zu erfüllen.



&#x20;| Slot | Content                             |

&#x20;|------|-------------------------------------|

\-| 0    | 10 Gold                             |

+| 0    |                                     |

&#x20;| 1    |                                     |

&#x20;| 2    |                                     |

&#x20;| 3    |                                     |





**Hat der Held etwas gegessen? Falls ja, was und wann?**

Befehle:

git log rucksack.md

git show 13834cd8d9765750e4e520baf2dc7fa2a22af53d



Antwort:

Tag 03.17 hat er ein Brot gegessen



**2.**

**Beim letzten Commit (tag 04.5) ist etwas schief gelaufen, es wurden versehentlich zu wenig experience Punkte eingestellt. Ändern Sie diesen letzten Commit und passen Sie die experience Punkte auf 42 an.**

Befehle:

git add stats.md; git commit --amend



Antwort:

# Stats

|Property|Value|
|-|-|
|health|8|
|experience|42|
|hunger|0|
|weapon|sword (3 dmg)|
|armor|light (2 dmg)|





**3.**

**Schreiben Sie die Geschichte in der Datei questlog.md fort und erzeugen Sie einen neuen Commit für tag 04.6. Ändern Sie bitte hierzu nur die eine Datei questlog.md.**

Befehle:

git add questlog.md

git commit -m tag 04.6



Antwort:

"questlog.md verändert"



**4.**

**Schreiben Sie die Geschichte noch weiter fort (tag 04.7), aber ändern Sie diesmal mehrere Dateien, die an diesem Tag (neuer Commit) gemeinsam eingecheckt werden sollen.**

Befehle:

git add ./\*

git commit -m tag 04.7



Antwort:

"questlog.md verändert" und "stats.md verändert"



**5.**

**Fälschlicherweise wurden die Statuspunkte und die Ausrüstung bisher gemeinsam in der Datei stats.md geführt. Korrigieren Sie das und verschieben Sie die Ausrüstungsgegenstände aus der Datei stats.md in eine neue Datei gear.md. Checken Sie Ihre Änderungen als tag 04.8 (neuer Commit) gemeinsam ein. (Hinweis: Es reicht, wenn diese Änderung als letzter Commit auf der Spitze des master-Branches existiert. Sie brauchen/sollen die Trennung von Statuspunkten und Ausrüstung nicht rückwirkend in die Historie einbauen!)**

Befehle:

git add stats.md

git add gear.md

git commit -m tag 04.8



Antwort:

# Stats

|Property|Value|
|-|-|
|health|8|
|experience|40|
|hunger|0|





# Gear

|weapon|sword (3 dmg)|
|-|-|
|armor|light (2 dmg)|







