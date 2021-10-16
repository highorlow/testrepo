# testrepo

## Typische Arbeitsabläufe mit GIT

- Clone: git clone {repoadresse}
- Branch erstellen: git branch {name der branch}
- Auf Branch wechseln: git checkout {name der branch}
- Commit:
- 1. git add {namen der neuen dateien oder "*" für all}
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
