# Sozialraum Berliner Platz

Interaktive Sozialraumkarte für das Umfeld des Berliner Platzes in Ludwigshafen am Rhein, erstellt als Arbeitsmaterial für das Projekt Räume der Utopie und Räume des Zweifels. Die Karte zeigt rund 560 Einrichtungen in elf Kategorien, eine Konfliktebene mit Zeitleiste von 2008 bis 2026, eine Tag-Nacht-Ansicht auf Grundlage von Öffnungszeiten, Stadtteilstatistik sowie eine gemeinsame Nadelmethode für Werkstätten.

## Dateien

`index.html` ist die vollständige Karte. Alle Daten stecken in der Datei, sie läuft ohne Server in jedem aktuellen Browser.

`Code.gs` ist das Backend für die gemeinsame Nadelmethode. Es gehört in den Apps-Script-Editor der Google-Tabelle „Sozialraum Berliner Platz – Nadeln“.

## Einrichtung

Die Tabelle öffnen, über Erweiterungen den Apps-Script-Editor aufrufen, den Beispielcode durch den Inhalt von `Code.gs` ersetzen und speichern. Über Bereitstellen eine neue Bereitstellung vom Typ Web-App anlegen, bei „Ausführen als“ die eigene Person und bei „Zugriff“ die Option „Jeder“ wählen, die Berechtigungen bestätigen und die Web-App-URL kopieren. Diese URL in `index.html` im Block `CONFIG` bei `APPS_SCRIPT_URL` eintragen, dort auch die Adressen von Impressum und Datenschutzerklärung der veröffentlichenden Stelle. Anschließend `index.html` in das Repository hochladen und unter Settings, Pages die Veröffentlichung aus dem Hauptzweig aktivieren.

Ohne eingetragene URL bleiben Einträge der Nadelmethode im jeweiligen Browser. Die Karte lädt Einträge anderer nur beim Öffnen und wenn jemand auf „Einträge aktualisieren“ klickt. Nach einem eigenen Eintrag oder dem Entfernen eines eigenen Eintrags wird der Stand ebenfalls neu geladen.

## Datenschutz

Die Karte lädt keine externen Schriften, Skripte oder Kartenkacheln. Externe Anfragen gehen nur an die Apps-Script-Web-App, sofern sie eingetragen ist. Dort gespeichert werden Art des Ortes, freiwillige Bezeichnung, freiwillige Gruppe, Kartenposition und Zeitstempel, außerdem pro Browsersitzung ein Besuch mit Datum. Namen und IP-Adressen speichert das Skript nicht. GitHub protokolliert nach eigenen Angaben die IP-Adressen von Besuchenden der Pages-Seite, Google verarbeitet beim Aufruf der Web-App technische Verbindungsdaten. Beide Anbieter sitzen in den USA. Vor dem Einsatz sollte die Datenschutzerklärung der veröffentlichenden Stelle das abdecken. Freitextfelder sollten Teilnehmende nicht für personenbezogene Angaben nutzen, die Moderation kann Einträge direkt in der Tabelle löschen.

## Daten und Quellen

Kartendaten © OpenStreetMap-Mitwirkende, verfügbar unter der Open Database License (ODbL 1.0), https://www.openstreetmap.org/copyright. Abfrage über die Overpass-API am 26.10.2026, Öffnungszeiten ausgewertet für die Woche vom 9. bis 15. November 2026.

Bevölkerungsdaten aus den Stadtteilpässen 2026 der Stadt Ludwigshafen am Rhein, Bereich Stadtentwicklung, Statistikstelle.

Die Konfliktebene beruht auf 34 Dokumenten von Stadt, Polizei, Presse, Parteien und Initiativen sowie Fachliteratur. Alle Quellen sind in der Karte unter den Reitern Konflikte und Quellen verlinkt.

Die Befunde sind Hypothesen aus öffentlich verfügbaren Daten und ersetzen keine Sozialraumanalyse mit Beteiligung der Menschen vor Ort.
