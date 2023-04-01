# Daizu-Materialien

## Videos

### restart-linode.mkv

In dem Video wird erklärt, wie man den Linode updatet, rebootet und die Skripte,
die darauf laufen, neu startet. Das muss ca. alle vier Wochen gemacht werden.

### edit-credentials-vercel.mkv

In dem Video wird erklärt, wie man so genannte _environmental variables_ bei
Vercel ersetzt. So etwas kann von Zeit zu Zeit nötig sein. Sollte dir ein
Account bei Vercel fehlen, kann ich den noch einrichten.

## Weitere Dateien

Daneben habe ich noch zwei weitere Dateien mitgesendet (per Mail), die den
SSH-Zugriff auf den Linode ermöglichen. Diese Dateien werden auf dem eigenen
Rechner im Verzeichnis `/home/{USERNAME}/.ssh` oder einem Unterordner abgelegt.
Heißt die Datei mit dem private Key (`mygpgkey_sec.gpg`)
`/home/{USERNAME}/.ssh/id_rsa`, kann der Schlüssel mit dem Kommando `ssh-add`
und dem in 1Password abgespeicherten Passwort (**SSH-Key für Linode entsperren**)
entsperrt werden. Bei anderen Dateinamen oder Pfaden, muss der Pfad zum Private
Key beim Aufruf angegeben werden. Dann kann der Login mit dem im Linode
angegebenen Kommando erfolgen. Über diesen Key werden auch bei jedem Neustart
der Skripte auf dem Linode die aktuellen Skripte von der GitHub-Quelle geladen.

**Hinweis**: Das Passwort kann **nicht verändert** werden.