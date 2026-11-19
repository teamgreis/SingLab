# SingLab – Adminbereich, PIN-Schutz und Updateverwaltung

Dieses Dokument definiert die fachlichen Anforderungen für die Administration und Aktualisierung von SingLab.

## 1. Adminbereich und Ersteinrichtung

### 1.1 Erste Inbetriebnahme

Beim allerersten Start von SingLab wird die Einrichtung einer Admin-PIN verlangt, bevor administrative Funktionen genutzt werden können.

- Die PIN besteht exakt aus sechs Ziffern.
- Die PIN muss zweimal eingegeben werden, damit Tippfehler erkannt werden.
- Die PIN darf nicht leer, unvollständig oder offensichtlich ungültig sein.
- Die Einrichtung wird erst abgeschlossen, wenn beide Eingaben übereinstimmen.
- Die Anwendung bestätigt anschließend, dass der Adminzugang eingerichtet wurde.
- Die PIN wird geschützt gespeichert. Sie darf weder im Klartext abgelegt noch in Protokollen, Fehlermeldungen, Exporten oder Git-Dateien ausgegeben werden.
- Die PIN und ihr geschützter Speicherwert dürfen niemals in dieses Repository eingecheckt werden.

### 1.2 Zugriff auf Adminfunktionen

- Der Adminbereich ist standardmäßig gesperrt.
- Beim Öffnen wird die sechsstellige PIN abgefragt.
- Erst nach korrekter Eingabe wird der Adminbereich freigegeben.
- Eine erfolgreiche Anmeldung darf nicht dauerhaft und unbegrenzt gültig bleiben.
- Nach einer konfigurierbaren Inaktivitätszeit wird der Adminbereich automatisch gesperrt.
- Beim manuellen Verlassen des Adminbereichs kann die Sperre sofort aktiviert werden.
- Falsche PIN-Eingaben werden neutral gemeldet; die richtige PIN darf nicht durch Hinweise oder Fehlermeldungen ableitbar sein.
- Wiederholte Fehlversuche müssen durch zeitlich zunehmende Verzögerung oder eine vergleichbare Schutzmaßnahme begrenzt werden.
- Die Adminfreigabe darf nicht automatisch auf andere Browser oder Geräte übertragen werden.

### 1.3 PIN ändern und wiederherstellen

- Eine angemeldete Administration kann die PIN ändern, indem sie die aktuelle PIN und anschließend die neue PIN zweimal eingibt.
- Ein Wiederherstellungsweg muss vorgesehen werden, damit ein Verlust der PIN nicht zu einer dauerhaften Aussperrung führt.
- Die Wiederherstellung muss bewusst durch eine berechtigte Serveradministration erfolgen und darf keine geheime Standard-PIN oder Hintertür enthalten.
- Jede Wiederherstellung beendet bestehende Admin-Sitzungen.

### 1.4 Admin-Dashboard

Der Adminbereich soll mindestens enthalten:
- Installierte SingLab-Version.
- Verfügbare neuere Version, falls vorhanden.
- Zeitpunkt der letzten Update-Prüfung.
- Schaltfläche „Jetzt nach Updates suchen“.
- Änderungsübersicht der verfügbaren Version.
- Schaltfläche zum Starten eines Updates.
- Status laufender oder zuletzt ausgeführter Aktualisierungen.
- Hinweise zu Sicherung und Wiederherstellung.
- Möglichkeit, den Adminbereich zu sperren.

## 2. Update-Erkennung

### 2.1 Updatequelle

SingLab verwendet das offizielle Projekt-Repository bzw. die dort veröffentlichten Versionen als Quelle für Versionsinformationen. Es muss eindeutig erkennbar sein, welche Version installiert ist und welche Version aktuell angeboten wird.

### 2.2 Regelmäßige Prüfung

- SingLab prüft in sinnvollen Abständen, ob eine neuere stabile Version verfügbar ist.
- Die Prüfung darf die Bedienung und Audiowiedergabe nicht spürbar beeinträchtigen.
- Die Prüfung muss manuell im Adminbereich ausgelöst werden können.
- Bei fehlender Internetverbindung wird kein falscher Fehlerzustand erzeugt; der letzte bekannte Stand bleibt sichtbar und die nächste Prüfung kann später erfolgen.
- Die Anwendung darf keine persönlichen Trainingsdaten, PIN-Daten oder sonstige Nutzungsdaten an die Updatequelle übertragen.
- Vorabversionen dürfen nicht als stabile Updates angezeigt werden, sofern sie nicht ausdrücklich aktiviert wurden.

### 2.3 Versionsanzeige

Die Updateansicht zeigt:
- Installierte Version.
- Verfügbare Version.
- Veröffentlichungsdatum, sofern verfügbar.
- Kurze Änderungsübersicht.
- Kennzeichnung, ob es sich um ein reguläres Update oder ein sicherheitsrelevantes Update handelt, sofern diese Information vorliegt.

## 3. In-App-Benachrichtigungen

Wenn SingLab geöffnet ist und eine neuere Version erkannt wird, soll eine sichtbare, aber nicht störende Benachrichtigung erscheinen.

Anforderungen:
- Hinweis mit verfügbarer Versionsnummer.
- Kurze Zusammenfassung der Änderungen.
- Aktion „Details ansehen“.
- Aktion „Später erinnern“.
- Für Administratoren eine Aktion „Zum Adminbereich“.
- Der Hinweis darf keine laufende Übung unterbrechen oder die Audioausgabe stoppen.
- Die Benachrichtigung kann während einer Session dezent angezeigt und nach der Session erneut hervorgehoben werden.
- Ein bereits zur Kenntnis genommener Hinweis soll nicht bei jedem Seitenwechsel erneut erscheinen.
- Sicherheitsrelevante Updates dürfen deutlicher gekennzeichnet werden.
- Es wird nicht behauptet, ein Update sei installiert, bevor die Aktualisierung tatsächlich erfolgreich abgeschlossen ist.

Die In-App-Benachrichtigung ist die verbindliche Grundfunktion. Betriebssystem-Push-Mitteilungen können optional ergänzt werden, sind aber keine Voraussetzung.

## 4. Updateinstallation

- Ein Update wird nur durch eine bewusste administrative Aktion gestartet.
- Vor dem Update wird die Versionsänderung angezeigt.
- Vor einer Aktualisierung wird eine Sicherung der relevanten SingLab-Daten vorgesehen.
- Eine laufende Warm-up- oder Trainingssession darf nicht ohne Warnung unterbrochen werden.
- Ist eine Session aktiv, soll das Update bis zum Ende oder bis zu einer ausdrücklichen Bestätigung warten.
- Während der Aktualisierung wird ein klarer Status angezeigt.
- Nach erfolgreichem Update wird die neue Version bestätigt.
- Bei einem fehlgeschlagenen Update bleibt SingLab in einem möglichst funktionsfähigen Zustand; die Anwendung zeigt verständliche nächste Schritte.
- Ein Rückkehr- bzw. Wiederherstellungsweg zur vorherigen funktionsfähigen Version ist vorzusehen.
- Ein Update darf niemals die Admin-PIN zurücksetzen oder offenlegen.

## 5. Update-Sicherheit

- Nur die festgelegte offizielle Quelle darf als Updatequelle gelten.
- Die Herkunft und Integrität eines Updates müssen überprüft werden.
- Unvollständige oder nicht verifizierbare Updates dürfen nicht installiert werden.
- Zugangsdaten, private Schlüssel, Tokens und PIN-Daten dürfen nicht im Repository liegen.
- Updatefehler dürfen keine vertraulichen Informationen in der Oberfläche oder in Logs offenlegen.

## 6. Status und Zustände

Die Oberfläche muss mindestens diese Zustände verständlich darstellen:
- Aktuell – keine neuere stabile Version gefunden.
- Update verfügbar – neue Version erkannt.
- Prüfung läuft.
- Update vorbereitet.
- Update wird ausgeführt.
- Update erfolgreich.
- Update fehlgeschlagen.
- Prüfung derzeit nicht möglich.

## 7. Abnahmebedingungen

Die Administration ist erst dann vollständig, wenn:
1. Beim ersten Start eine sechsstellige PIN eingerichtet werden muss.
2. Eine falsche PIN den Zugang verweigert.
3. Die PIN nicht im Klartext gespeichert oder im Repository abgelegt wird.
4. Adminfunktionen nach Inaktivität wieder gesperrt werden.
5. SingLab eine neue stabile Version erkennen kann.
6. Bei geöffneter Anwendung ein In-App-Hinweis erscheint.
7. Der Hinweis eine laufende Session nicht ungefragt unterbricht.
8. Ein Update nur nach bewusster administrativer Freigabe startet.
9. Ein Updatefehler verständlich angezeigt wird.
10. Die installierte Version nach erfolgreichem Update korrekt angezeigt wird.
