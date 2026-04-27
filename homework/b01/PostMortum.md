**Post Mortem B01**

Im Rahmen des Übungsblattes B01 habe ich mich mit der Auswertung eines bestehenden Git-Repositories beschäftigt. Ziel war es, mithilfe verschiedener Git-Befehle vergangene Änderungen nachzuvollziehen und daraus konkrete Informationen über den Spielverlauf des Helden Markus zu gewinnen. Dafür nutzte ich insbesondere **git show**, **git log**, **git diff** sowie dateibezogene Verlaufsabfragen für **stats.md** und **rucksack.md**.



Zu Beginn bereitete mir vor allem der Befehl **git show tag 01** Schwierigkeiten, da Git diese Eingabe zunächst nicht erkannte. Nach mehreren Versuchen verstand ich jedoch, dass ich zuerst mit **git log** die korrekte Commit-ID ermitteln und diese anschließend mit **git show** genauer untersuchen musste. Dadurch wurde mir auch die Darstellung der Änderungen im Diff klarer: Der graue Bereich zeigte den vorherigen Zustand der Datei an, während der grüne Bereich die neue Version darstellte. Auf diese Weise konnte ich nachvollziehen, wann Markus beispielsweise Erfahrungspunkte erhielt, Hunger verlor oder seinen Rucksack durch einen gekauften beziehungsweise gefundenen Heiltrank veränderte.

Hilfreich war dabei, gezielt einzelne Dateien zu untersuchen. Mit Befehlen wie **git log rucksack.md** oder **git log stats.md** konnte ich die Suche nach relevanten Änderungen deutlich eingrenzen und dadurch schneller zu den benötigten Antworten gelangen.



Der schwierigste Teil der Bearbeitung war insgesamt das korrekte Navigieren im Versionsverlauf und das Verstehen der teilweise unübersichtlichen Git-Ausgaben. Dieses Problem habe ich gelöst, indem ich verschiedene Log-Ausgaben systematisch verglichen und mir relevante Commit-Stände einzeln anzeigen ließ. Zusätzlich musste ich in Git Quest 2 eine bestehende State-Datei anpassen, die Experience auf 42 setzen und den letzten Commit mithilfe von **git add stats.md; git commit --amend** verändern. Die Aufgaben danach fielen mir deutlich leichter, da ich mein Repository bereits eingerichtet hatte.



Besonders gelernt habe ich den praktischen Umgang mit Git zur Analyse von Projektverläufen sowie die Bedeutung präziser Commit-Meldungen. Unerwartet lehrreich war für mich außerdem die Einrichtung der benötigten Tools für Prog2. Diese war für mich anstrengender als die eigentliche Aufgabenbearbeitung, da es immer wieder kleinere technische Probleme gab und ich zunächst unsicher war, wie ich mein Repository sinnvoll aufbauen und mich sicher darin bewegen sollte. Gerade durch Befehle wie cd .. oder ll -a habe ich das Arbeiten in der Verzeichnisstruktur und den Zusammenhang mit Gradle besser verstanden.



**Repo-Link:** https://github.com/Caiissa/Prog2-2026-RS.git



