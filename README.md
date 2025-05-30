
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

git log
Listet alle bisherigen Commits auf. Mit --graph wird’s übersichtlicher.


3.Git Befehle für die Arbeit mit entfernten Repositories