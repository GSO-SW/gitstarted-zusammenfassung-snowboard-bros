
Git Zusammenfassung

Inhaltsverzeichnis

1.Begriffe

2.Git Befehle für die Arbeit mit lokalen Repositories

git init:
Initialisiert ein neues Git-Repository im aktuellen Verzeichnis. Es erstellt einen versteckten .git-Ordner zur Versionsverwaltung.

git add *:
Fügt alle geänderten und neuen Dateien zur Staging Area hinzu. Diese Dateien sind dann bereit für den nächsten Commit.

git commit -m "Nachricht":
Speichert die gestagten Änderungen dauerhaft im Repository mit einer Kommentar-Nachricht (-m "Nachricht"). Jeder Commit bildet einen Versionspunkt.

git Status:
Zeigt, welche Dateien geändert, gestaged oder untracked sind. Sehr hilfreich zum Überprüfen vor dem Commit.

git branch <name>:
Mit git branch kannst du verschiedene Versionen deines Projekts erstellen. So kannst du z. B. an neuen Funktionen arbeiten, ohne den Hauptcode zu verändern.

git log (--graph):
Listet alle bisherigen Commits auf. --graph zeigt eine grafische Baumstruktur der Commit-Historie.

git ignore:
Ist eine Datei zum Definieren, welche Dateien Git ignorieren soll.

git merge:
Fügt zwei Branches zusammen. Die Änderungen aus einem anderen Branch werden in deinen aktuellen Branch übernommen.



3.Git Befehle für die Arbeit mit entfernten Repositories

