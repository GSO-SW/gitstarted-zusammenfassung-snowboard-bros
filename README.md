
Git Zusammenfassung

Inhaltsverzeichnis

1.Begriffe

2.Git Befehle für die Arbeit mit lokalen Repositories

3.Git Befehle für die Arbeit mit entfernten Repositories



                                                    BEGRIFFE


1.1 Repository:
Ein Container für Projektdateien, der den vollständigen Versionsverlauf und Metadaten speichert.

1.2 Branch:
Eine isolierte Entwicklungslinie, die Änderungen vom Hauptcode trennt, um Features oder Experimente ohne Risiko zu testen.

1.3 Merge:
Der Prozess, Änderungen aus einem Branch in einen anderen zu integrieren (z. B. Feature-Branch → Main-Branch).

1.4 Konflikte:
Kollidierende Änderungen in derselben Datei, die manuell gelöst werden müssen, bevor ein Merge abgeschlossen werden kann.

1.5 Main:
Der standardmäßige primäre Branch in modernen Git-Repositories (ersetzt historisch "Master").

1.6 Master:
Der veraltete Begriff für den primären Branch; heute durch "Main" abgelöst.

1.7 Remote:
Ein externes Repository (z. B. auf GitHub), das als zentrale Quelle für Kollaboration dient.

1.8 Lokal:
Die Kopie eines Repositories auf dem Entwicklungsrechner, unabhängig vom Remote-Server.

1.9 Upstream:
Das übergeordnete Remote-Repository, von dem Änderungen abgeholt ("pull") oder an das gepusht ("push") wird.

1.10 Staging Area:
Ein Zwischenspeicher (auch "Index" genannt), der Änderungen vorbereitet, bevor sie in einem Commit permanent gespeichert werden.


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


# Bewertung der Git-Zusammenfassung
SnowBoard Bros

## 1. Fachbegriffe

**Erreichte Punkte:** 3

**Begründung:**
- Die Begriffe sind **korrekt**, **klar** und **verständlich** erklärt.
- Wichtige Konzepte wie *Repository*, *Branch*, *Staging Area*, *Merge*, *Remote*, *Upstream* usw. sind enthalten.
- Zusätzliche relevante Begriffe wie *Main* und *Master* werden differenziert erklärt, inklusive historischem Kontext.
- Fachliche Tiefe (z. B. Erklärung von *Konflikten*, *Main/Master*) zeigt fundiertes Verständnis.

**Verbesserungsvorschläge:**
- Die Begriffe könnten alphabetisch oder thematisch gruppiert werden, um die Übersichtlichkeit weiter zu verbessern.

---

## 2. Befehle lokale Arbeit

**Erreichte Punkte:** 2

**Begründung:**
- Die lokalen Git-Befehle sind **vollständig**, **korrekt erklärt** und gut **strukturiert**.
- Auch fortgeschrittene Befehle wie `git cherry-pick`, `git rebase`, `git revert` und Varianten von `git reset` sind enthalten.
- Es werden zusätzlich Hinweise gegeben, z. B. zu den Reset-Modi `--soft`, `--mixed`, `--hard`, die Erläuterungen hierzu sind korrekt.
- Hinweise, wann bestimmte Befehle nützlich sind (z. B. „so kannst du …“) erleichtern das Verständnis.

**Verbesserungsvorschläge:**
- Eine klarere Formatierung (z. B. Tabellenstruktur oder visuelle Trennung von Befehl, Beschreibung, Beispiel) könnte die Lesbarkeit verbessern.
- Typische Fehlermeldung und der Umgang damit würden die Zusammenfassung noch lesenswerter machen!

---

## 3. Befehle entfernte Arbeit

**Erreichte Punkte:** 2

**Begründung:**
- Alle zentralen Remote-Befehle (`git clone`, `git pull`, `git push`, `git fetch`, `--set-upstream`) sind enthalten und **verständlich erklärt**.
- Die Funktionen der Befehle sind **präzise**, mit Fokus auf Praxisbezug (z. B. „damit andere sie sehen und nutzen können“).
- Die Abgrenzung zwischen `fetch` und `pull` wird korrekt beschrieben, was oft ein Stolperstein ist.

**Verbesserungsvorschläge:**
- Eine klarere Formatierung (z. B. Tabellenstruktur oder visuelle Trennung von Befehl, Beschreibung, Beispiel) könnte die Lesbarkeit verbessern.
- Hinweise auf potenzielle Konflikte oder empfohlene Reihenfolgen in der Anwendung wären ein wünschenswert.

---

## 4. Zusammenarbeit über GitHub

**Erreichte Punkte:** 3

**Begründung anhand des Git-Graphen:**
- **Branching-Strategie**: Es wurden mehrere Feature-Branches verwendet (`Marwin`, `david`), was auf ein gutes Verständnis der Arbeitsteilung hinweist.
- **Merge-Vorgänge**: Wiederholte Merges aus den Feature-Branches in `master` zeigen, dass Beiträge zusammengeführt wurden. Die Einträge „Merge branch 'Marwin'“ und „Merge branch 'david'“ belegen dies mehrfach.
- **Verlaufsstruktur**: Die saubere Baumstruktur mit regelmäßigen und zahlreichen Commits aus verschiedenen Zweigen zeigt ein durchdachtes Vorgehen und Kollaboration.
- **Commitnachrichten**: Die Commitnachrichten sind (wenn auch knapp) inhaltlich aussagekräftig.





## Zusammenfassung

| Kriterium                 | Punkte (max. 3) |
|---------------------------|-----------------|
| Fachbegriffe              | 3               |
| Befehle lokale Arbeit     | 2               |
| Befehle entfernte Arbeit  | 2               |
| Zusammenarbeit            | 3               |
| **Gesamt**                | **10/12**       |
   
--> **83% --> gut (12 NP.)**




