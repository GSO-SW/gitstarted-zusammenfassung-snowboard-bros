
Git Zusammenfassung

Inhaltsverzeichnis

1.Begriffe

2.Git Befehle für die Arbeit mit lokalen Repositories

3.Git Befehle für die Arbeit mit entfernten Repositories

Repository:
Ein Container für Projektdateien, der den vollständigen Versionsverlauf und Metadaten speichert.

Branch:
Eine isolierte Entwicklungslinie, die Änderungen vom Hauptcode trennt, um Features oder Experimente ohne Risiko zu testen.

Merge:
Der Prozess, Änderungen aus einem Branch in einen anderen zu integrieren (z. B. Feature-Branch → Main-Branch).

Konflikte:
Kollidierende Änderungen in derselben Datei, die manuell gelöst werden müssen, bevor ein Merge abgeschlossen werden kann.

Main:
Der standardmäßige primäre Branch in modernen Git-Repositories (ersetzt historisch "Master").

Master:
Der veraltete Begriff für den primären Branch; heute durch "Main" abgelöst.

Remote:
Ein externes Repository (z. B. auf GitHub), das als zentrale Quelle für Kollaboration dient.

Lokal:
Die Kopie eines Repositories auf dem Entwicklungsrechner, unabhängig vom Remote-Server.



                                                      LOKAL


2.1 git init:
Initialisiert ein neues Git-Repository im aktuellen Verzeichnis. Es erstellt einen versteckten .git-Ordner zur Versionsverwaltung.

2.2 git add datei.txt:
Fügt eine bestimmte Datei zur Staging-Area hinzu.

2.3 git add *:
Fügt alle geänderten und neuen Dateien zur Staging Area hinzu. Diese Dateien sind dann bereit für den nächsten Commit.

2.4 git commit -m "Nachricht":
Speichert die gestagten Änderungen dauerhaft im Repository mit einer Kommentar-Nachricht (-m "Nachricht"). Jeder Commit bildet einen Versionspunkt.

2.5 git checkout: Wird verwendet, um zwischen Branches zu wechseln oder einzelne Dateien auf einen früheren Stand zurückzusetzen. So kannst du z. B. von main zu einem Feature-Branch wechseln oder eine Datei aus einem früheren Commit wiederherstellen.

2.6 git Status:
Zeigt, welche Dateien geändert, gestaged oder untracked sind. Sehr hilfreich zum Überprüfen vor dem Commit.

2.7 git branch <name>:
Mit git branch kannst du verschiedene Versionen deines Projekts erstellen. So kannst du z. B. an neuen Funktionen arbeiten, ohne den Hauptcode zu verändern.

2.8 git log (--graph):
Listet alle bisherigen Commits auf. --graph zeigt eine grafische Baumstruktur der Commit-Historie.

2.9 git ignore:
Ist eine Datei zum Definieren, welche Dateien Git ignorieren soll.

2.10 git merge:
Fügt zwei Branches zusammen. Die Änderungen aus einem anderen Branch werden in deinen aktuellen Branch übernommen.

2.11 git cherry-pick:
Holt einen einzelnen Commit aus einem anderen Branch in deinen aktuellen Branch. Nützlich, wenn du nur eine bestimmte Änderung brauchst.

2.12 git rebase:
Verschiebt deine Änderungen auf einen anderen Stand, als ob du später angefangen hättest. Der Verlauf sieht danach sauberer aus.

2.13 git reset:
Setzt dein Projekt zurück auf einen früheren Zustand.

--soft: nur der Commit wird zurückgenommen.

--mixed: auch die Stage (Index) wird geleert.

--hard: alles wird zurückgesetzt – auch deine Dateien!

2.14 git revert:
Erstellt einen neuen Commit, der die Änderungen eines vorherigen Commits rückgängig macht, ohne die Commit-Historie zu verändern. So kannst du Fehler korrigieren, ohne den Verlauf zu löschen oder zu verändern.



                                                      REMOTE



3.1 git clone <URL>:
Lädt ein komplettes Remote-Repository lokal herunter.

3.2 git pull:
Holt neue Änderungen vom Remote-Branch und merged sie lokal.

3.3 git push:
Schiebt deine lokalen Commits zu einem entfernten Repository (z. B. GitHub), damit andere sie sehen und nutzen können.

3.4 git fetch:
Lädt neue Änderungen vom entfernten Repository herunter, ohne sie automatisch in deinen aktuellen Branch zu integrieren

3.5 --set-upstream (oder kurz -u):
Wird beim git push benutzt, um den lokalen Branch mit einem entfernten Branch zu verknüpfen.
