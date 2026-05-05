### **Git-Quest**

1\.

Befehle:

git clone https://github.com/Programmiermethoden-CampusMinden/prog2\_ybel\_gitquest.git

git branch -a

git log --all --graph --oneline --decorate

git diff 8f88b19 6405bd9 //Nur shopkeeper.md hat sich nicht verändert

git add shopkeeper.md

git commit -m Shopkeeper

git checkout master // Überprüfen, git branch auch möglich

git merge origin/end



2\.

Befehle:

git clone https://github.com/Programmiermethoden-CampusMinden/prog2\_ybel\_gitquest.git

git branch -a

git log --all --graph --oneline --decorate

git diff 8f88b19 6405bd9 

//Hat einen Heiltrank getrunken

git add rucksack.md

git add stats.md

git commit -m Heiltrank

git checkout master // Überprüfen, git branch auch möglich

git merge origin/end



3\.

Befehle:

git clone https://github.com/Programmiermethoden-CampusMinden/prog2\_ybel\_gitquest.git

git branch -a

git log --all --graph --oneline --decorate

git diff 8f88b19 6405bd9

//Hat einen Heiltrank getrunken

git add rucksack.md

git add stats.md

git commit -m Heiltrank

git checkout master // Überprüfen, git branch auch möglich

git merge origin/end

git status // Welche Dateien sind betroffen

nano rucksack.md

nano stats.md

git add rucksack.md

git add stats.md

git commit -m Heiltrank



Antwort:

Was passiert, wenn die Änderung im master identisch zu der in end ist?

Dabei ist bei mir "nicht" passiert, es ist zu keinem Mergeconflict gekommen.



Was passiert, wenn die Änderung im master anders ist als in end?

Dabei kam es zu Mergeconflicten, die ich über den Nano behoben habe.



4\.

Befehle:

git clone https://github.com/Programmiermethoden-CampusMinden/prog2\_ybel\_gitquest.git

git branch -a

git log --all --graph --oneline --decorate

git diff 8f88b19 6405bd9git

git add shopkeeper.md

git commit -m Shopkeeper

git checkout end

git rebase master

git log --all --graph --oneline --decorate // Überprüft











