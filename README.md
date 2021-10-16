# testrepo

## Typische Arbeitsabläufe mit GIT

- Clone: git clone {repoadresse}
- Branch erstellen: git branch {name der branch}
- Auf Branch wechseln: git checkout {name der branch}
- Commit:
- 1. git add {namen der neuen dateien oder "*" für alle}
- 2. git commit -m {commit message}
- Mergen: in der branch, in die hineingemerged werden soll: git merge {name der anderen branch}
- WICHTIG: Nach dem Mergen immer testen, ob alles noch funktioniert!
- Fall etwas mal nicht mehr funktioniert: Zurück zu einem vorherigen Commit!
- 1. 'git log' zeigt die letzten commits - hier die Nummer des gewünschten commits notieren
- 2. ' git reset --hard {nummer des gewünschten commits}' setzt die branch zurück
- Push: git push sendet die Änderungen zu Github 
- Pull: git pull holt den aktuellen Stand der branch von Github

## Best Practices und Regeln

- Die main-branch muss immer funktionieren! D.h. immer ausführlich lokal testen, bevor auf die main gepusht wird.
- 1. Sind alle Änderungen vorheriger commits noch da?
- 2. Funktioniert noch alles, was funktioniert hat, bevor ich gemerged habe?

- Bevor auf die main gemerged wird, immer zuerst folgendes machen:
- 1. main branch pullen
- 2. main lokal in die aktuelle branch mergen
- 3. Testen!
- Erst wenn alles auf der branch funktioniert, pushen
- Änderungen mit zweiter Person reviewen, und wenn alles gut ist:
- 1. lokal auf die main mergen
- 2. main pushen

- Neue branches immer thematisch benennen: z.B. "Seitennavigation"

- Best Practices für commit messages:
- - https://chris.beams.io/posts/git-commit/
