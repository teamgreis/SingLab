# SingLab – Vollständige Produktspezifikation

**Produktname:** SingLab  
**Dokumentstatus:** Produktanforderungen und Funktionsumfang  
**Ziel:** Eine vollständige, selbst gehostete Plattform zum Einsingen, Aufwärmen und musikalischen Trainieren der Stimme.

---

## 1. Produktvision

SingLab ist ein persönliches Vocal-Training-Studio. Es soll Nutzerinnen und Nutzern helfen, vor dem Singen in die Stimme zu kommen, Tonhöhen sicherer kennenzulernen und musikalische Übungen regelmäßig und gezielt durchzuführen.

SingLab ist ausdrücklich mehr als ein einfacher Tongenerator oder ein einzelner Warm-up-Modus. Es bietet ein eigenständiges, umfangreiches Warm-up Studio sowie weitere Trainings-, Erkundungs- und Planungsbereiche.

### 1.1 Zentrale Leitidee

SingLab spielt Töne, Intervalle, Tonleitern, Akkorde, Rhythmen und Melodien vor. Die Person singt diese selbst nach. Die App unterstützt den Ablauf durch klare visuelle Darstellungen und verständliche Anleitungen.

### 1.2 Bewusste Produktgrenzen

- Kein Mikrofonzugriff erforderlich.
- Keine Sprach- oder Gesangsaufzeichnung.
- Keine automatische Tonhöhenerkennung oder Stimmanalyse.
- Keine Bewertung, ob eine Person einen Ton richtig getroffen hat.
- Keine Übertragung von Audiodaten an Server.
- Die Stimme wird nicht digital verarbeitet; SingLab stellt musikalische Referenzen und Übungen bereit.

Diese Grenzen müssen in der Oberfläche transparent kommuniziert werden.

---

## 2. Zielgruppen und Nutzungssituationen

- Menschen, die vor dem Singen ihre Stimme aufwärmen möchten.
- Anfängerinnen und Anfänger, die Tonhöhen und Intervalle kennenlernen wollen.
- Erfahrene Sängerinnen und Sänger, die gezielte Routinen nutzen möchten.
- Einzelpersonen und kleine Gruppen, die gemeinsam Übungen durchführen.

Typischer Ablauf: SingLab öffnen, eine passende Warm-up-Session auswählen, die Übungen anhören und nachsingen. Bei Bedarf kann danach ein gezieltes Training oder eine freie musikalische Erkundung folgen.

---

## 3. Informationsarchitektur und Hauptnavigation

Die Hauptnavigation umfasst:

1. **Dashboard** – Einstieg, zuletzt verwendete Übungen, Favoriten und schnelle Aktionen.
2. **Warm-up Studio** – vollständiger eigenständiger Bereich zum Einsingen.
3. **Training Studio** – strukturierte Übungen für Tonhöhe, Intervalle, Skalen, Melodien und Rhythmus.
4. **Pitch & Melody Lab** – freie Erkundung von Tönen, Intervallen, Tonleitern, Akkorden und Melodien.
5. **Instrument Studio** – Instrumente und Klangfarben auswählen und Referenzen abspielen.
6. **Exercise Library** – durchsuchbare Sammlung aller Übungen.
7. **Training Generator** – individuelle Übungsfolgen erstellen lassen.
8. **Training Plans** – persönliche Routinen und Trainingspläne.
9. **Progress** – Übersicht über absolvierte Einheiten und Trainingsgewohnheiten, ohne Leistungsbewertung der Stimme.
10. **Settings** – Klang, Darstellung, Bedienung, Datenschutz und persönliche Präferenzen.
11. **Admin** – geschützter Verwaltungsbereich; nur nach erfolgreicher PIN-Eingabe zugänglich.

Die Navigation muss auf Smartphones, Tablets und Desktopgeräten funktionieren.

---

## 4. Dashboard

Das Dashboard soll einen schnellen Einstieg ermöglichen und nicht überladen wirken.

Elemente:
- Begrüßung und kurze Erklärung des aktuellen Einstiegs.
- Schaltfläche „Sofort aufwärmen“.
- Auswahl einer kurzen, mittleren oder ausführlichen Session.
- Zuletzt verwendete Übungen und Trainingspläne.
- Favoriten.
- Fortsetzen einer unterbrochenen Session.
- Übersicht über absolvierte Trainingszeiten und Einheiten.
- Dezenter Hinweis auf verfügbare Updates, wenn eine neuere Version erkannt wurde.

---

## 5. Warm-up Studio – eigenständiger Kernbereich

Das Warm-up Studio ist ein vollständiger, zentraler Produktbereich und darf nicht auf eine einzelne Schaltfläche oder einen Untermodus reduziert werden.

### 5.1 Einstieg und Session-Längen

Vorgesehene Einstiegsmöglichkeiten:
- **Quick Warm-up:** sehr kurze Routine für wenig Zeit.
- **Gentle Warm-up:** besonders sanfter Einstieg.
- **Standard Warm-up:** ausgewogene Standardroutine.
- **Extended Warm-up:** längere, umfassendere Routine.
- **Complete Warm-up:** umfangreiche Kombination der verfügbaren Warm-up-Bausteine.
- **Custom Warm-up:** selbst zusammengestellte Routine.

Die Dauer soll je nach gewählter Session variieren und vor dem Start sichtbar sein. Nutzerinnen und Nutzer dürfen Übungen überspringen, wiederholen oder die Session pausieren.

### 5.2 Warm-up-Bausteine

- Sanfter Einstieg mit einzelnen Referenztönen.
- Tonhöhenbewegungen aufwärts und abwärts.
- Kleine und größere Intervalle.
- Einfache Tonfolgen.
- Dur- und Moll-Tonleitern.
- Arpeggien und Dreiklangsbewegungen.
- Kurze Melodie-Echos.
- Rhythmische Sprech- und Singimpulse.
- Vokalübungen mit angezeigten Silben, beispielsweise „Ma“, „Me“, „Mi“, „Mo“, „Mu“, „La“, „Le“, „Li“, „Lo“, „Lu“.
- Vokal-Klangfolgen wie „Aah“, „Ooh“ und „Hum“ als optionale Referenzklänge.
- Entspannende und bewusst langsamere Übergänge.
- Individuell zusammengestellte Übungsfolgen.

Die Anwendung soll keine medizinischen oder therapeutischen Wirkungen versprechen. Übungen müssen mit klaren, unaufdringlichen Hinweisen versehen sein, bei Unwohlsein aufzuhören und die Stimme nicht zu erzwingen.

### 5.3 Geführte Sessions

Jede geführte Session enthält:
- Name und kurze Beschreibung.
- Geschätzte Dauer.
- Schwierigkeitsgrad bzw. Intensität.
- Verwendete Tonart und Tonlage.
- Abspielbare Referenztöne und Übungsfolgen.
- Eine klare visuelle Anzeige des aktuellen Schritts.
- Zurück, Weiter, Pause, Wiederholen und Überspringen.
- Fortschrittsanzeige innerhalb der Session.

### 5.4 Individuelle Warm-up-Routinen

Eigene Routinen müssen:
- Übungen hinzufügen und entfernen können.
- Reihenfolge verändern können.
- Startton, Tonart und Oktavlage je Übung einstellen können.
- Tempo und Wiederholungszahl anpassen können.
- Als Favorit gespeichert werden können.
- Später erneut ausführbar sein.

---

## 6. Globales Tonhöhen- und Tonartensystem

Die Tonhöhen- und Tonartenauswahl ist global verfügbar und darf nicht nur im Warm-up Studio existieren.

### 6.1 Chromatische Tonklassen

Alle zwölf Tonklassen müssen unterstützt werden:
C, Cis/Des, D, Dis/Es, E, F, Fis/Ges, G, Gis/As, A, Ais/B, H.

Die Darstellung soll je nach Kontext sinnvolle enharmonische Schreibweisen verwenden. Deutsche Notennamen sind standardmäßig zu bevorzugen; eine alternative internationale Schreibweise soll auswählbar sein.

### 6.2 Tonarten

Alle Dur- und Molltonarten müssen auswählbar sein. Dazu gehören:
- Dur.
- Natürlich Moll.
- Harmonisch Moll.
- Melodisch Moll.

Die Auswahl muss unabhängig vom jeweiligen Übungsbereich verfügbar sein.

### 6.3 Weitere Skalen und Modi

Mindestens:
- Chromatische Tonleiter.
- Dur und natürliche, harmonische sowie melodische Mollvarianten.
- Dur- und Moll-Pentatonik.
- Blues-Skala.
- Ganztonleiter.
- Kirchentonarten: Ionisch, Dorisch, Phrygisch, Lydisch, Mixolydisch, Äolisch und Lokrisch.

Weitere Skalen können ergänzt werden, ohne bestehende Übungen zu verändern.

### 6.4 Tonhöhenbereich und Steuerung

- Breiter, musikalisch sinnvoller Tonhöhenbereich über alle geeigneten Oktavlagen.
- Frei einstellbarer Startton und Endton.
- Frei wählbare Oktave.
- Transposition einer Übung in andere Tonarten.
- Einstellbarer Referenz-Kammerton, Standard: A4 = 440 Hz.
- Anzeige der Notennamen und Frequenz, wo sinnvoll.
- Klare Warnung, wenn eine gewählte Übung außerhalb des für die Übung vorgesehenen Bereichs liegt; keine Aussage über den persönlichen Stimmumfang.

---

## 7. Training Studio

Das Training Studio bietet strukturierte Übungen, die unabhängig vom Warm-up Studio verwendet werden können.

### 7.1 Tone Echo

Ein einzelner Referenzton wird abgespielt. Danach folgt eine einstellbare Pause, in der die Person den Ton nachsingen kann. Die Übung kann mit mehreren Tönen und verschiedenen Oktavlagen wiederholt werden.

### 7.2 Interval Trainer

- Aufwärts- und abwärtsgerichtete Intervalle.
- Kleine und große Sekunden, Terzen, Quarten, Quinten, Sexten, Septimen und Oktaven.
- Reine, übermäßige und verminderte Varianten, soweit musikalisch sinnvoll.
- Anzeige des Intervallnamens und der Noten.
- Einzelne Intervalle oder zufällige Übungsfolgen.

### 7.3 Scale Training

- Tonleitern auf- und abwärts.
- Unterschiedliche Starttöne und Tonarten.
- Einstellbare Geschwindigkeit.
- Verschiedene Oktavumfänge.
- Wiederholungen und Pausen.

### 7.4 Arpeggio Training

- Dur-, Moll-, verminderte und übermäßige Dreiklänge.
- Vierklänge und weitere Akkordtypen.
- Auf- und abwärtsgerichtete Muster.
- Einstellbare Umkehrungen und Oktavlagen.

### 7.5 Melody Echo

Kurze Melodien werden vorgespielt und können nachgesungen werden. Die Schwierigkeit wird über Länge, Intervallsprünge, Rhythmus und Tonumfang der Übungsreferenz gesteuert.

### 7.6 Rhythm & Voice

Rhythmische Muster werden hörbar und visuell dargestellt. Die Person kann sie mit Stimme oder Silben nachbilden.

### 7.7 Chord & Harmony

Akkorde werden als Gesamtklang oder als Einzeltöne abgespielt. Die App zeigt die enthaltenen Noten und den Akkordnamen an.

### 7.8 Random Challenge

Erzeugt zufällige, aber musikalisch sinnvolle Übungen. Filter für Tonart, Tonhöhenbereich, Übungstyp und Schwierigkeitsgrad sind verfügbar.

---

## 8. Pitch & Melody Lab

Ein freier Erkundungsbereich mit:

- Virtueller Klaviatur.
- Tonhöhenexplorer.
- Anzeige von Notenname, Oktave und Frequenz.
- Intervallvisualisierung.
- Tonleiternavigator.
- Akkordexplorer.
- Melodieeditor für kurze Tonfolgen.
- Noten- und vereinfachter Intervallanzeige.
- Abspielen einzelner Töne, Folgen und Akkorde.
- Transposition und Änderung der Oktavlage.

Die Bedienung soll sowohl mit Touch als auch mit Maus und Tastatur möglich sein.

---

## 9. Instrument Studio

SingLab bietet eine breite Auswahl an Klangwelten. Die Klangfarbe soll unabhängig von der musikalischen Übung gewählt werden können.

Vorgesehene Instrumentfamilien:
- Klavier und E-Piano.
- Orgel.
- Streicher.
- Holzbläser.
- Blechbläser.
- Akustische und elektrische Gitarren.
- Synthesizer und elektronische Klangfarben.
- Vocal-like Referenzklänge, etwa Aah, Ooh und Hum.
- Percussion und rhythmische Klänge.

Einstellmöglichkeiten:
- Instrument/Klangfarbe.
- Lautstärke.
- Tempo, soweit relevant.
- Tonhöhe und Oktave.
- Einzelton, Intervall, Akkord oder Melodie.
- Vorschau vor Übernahme in eine Übung.

---

## 10. Exercise Library

Die Übungsbibliothek ist durchsuchbar und filterbar.

Filter:
- Bereich und Übungstyp.
- Dauer.
- Schwierigkeitsgrad.
- Tonart.
- Tonhöhenbereich.
- Instrument/Klangfarbe.
- Warm-up oder Training.
- Favoriten und eigene Übungen.

Jede Übung besitzt einen Titel, eine verständliche Beschreibung, eine geschätzte Dauer, Einstellungen und eine Vorschau.

Eigene Übungen müssen erstellt, bearbeitet, dupliziert und gelöscht werden können.

---

## 11. Training Generator

Der Generator erstellt Trainingsfolgen anhand der gewählten Kriterien:
- Zielbereich, beispielsweise Warm-up, Intervalle, Skalen oder Melodien.
- Gewünschte Dauer.
- Tonart und Startton.
- Instrument/Klangfarbe.
- Intensität bzw. Schwierigkeitsgrad.
- Anzahl der Übungen.
- Wiederholungen und Pausen.

Das Ergebnis muss vor dem Start überprüfbar und veränderbar sein. Generierte Trainings können gespeichert und später erneut verwendet werden.

---

## 12. Training Plans

Nutzerinnen und Nutzer können persönliche Routinen anlegen, beispielsweise:
- Kurzes Einsingen vor einer Gesangseinheit.
- Regelmäßiges Warm-up.
- Intervall- und Tonhöhentraining.
- Melodie- und Rhythmustraining.
- Freies musikalisches Erkunden.

Trainingspläne enthalten Reihenfolge, Dauer, Übungsparameter und optionale Wiederholungstage. Erinnerungen sind optional und standardmäßig zurückhaltend.

---

## 13. Progress

Der Fortschrittsbereich dokumentiert ausschließlich die Nutzung der App, nicht die Qualität der Stimme.

Mögliche Kennzahlen:
- Absolvierte Sessions.
- Trainingsdauer.
- Häufigkeit der Nutzung.
- Häufig genutzte Übungen.
- Persönliche Favoriten.
- Verlauf eigener Trainingspläne.

Es gibt keine automatische Bewertung der Stimme und keine fingierten Genauigkeits- oder Leistungswerte.

---

## 14. Audio- und Bedienkonzept

- Alle Übungen müssen hörbar vorgespielt werden.
- Audioausgabe erfolgt über Lautsprecher oder Kopfhörer.
- Kein Mikrofonzugriff und keine Aufnahmefunktion.
- Lautstärke und Tempo müssen leicht erreichbar sein.
- Start, Pause, Fortsetzen, Wiederholen und Stoppen müssen eindeutig bedienbar sein.
- Bei längeren Sessions muss der aktuelle Übungsschritt klar erkennbar sein.
- Ein visueller Takt- oder Fortschrittsindikator unterstützt die Orientierung.
- Klang und Lautstärke müssen auch bei längerer Nutzung angenehm und kontrollierbar bleiben.

---

## 15. Oberfläche und Design

Designrichtung:
- Modern, hochwertig, ruhig und musikalisch.
- Dunkles Grunddesign mit violetten Akzenten.
- Optionaler heller Modus.
- Gute Lesbarkeit und klare visuelle Hierarchie.
- Keine unnötig überladenen Dashboards.
- Große, gut erreichbare Bedienelemente für Smartphones und Tablets.
- Responsives Layout für Smartphone, Tablet und Desktop.
- Barrierearme Kontraste, Tastaturbedienung und verständliche Beschriftungen.

---

## 16. Profile, Einstellungen und Datenschutz

Einstellungen:
- Sprache.
- Helles/dunkles Design.
- Standardinstrument.
- Standardtonart und Referenzton.
- Standardtempo.
- Audio-Lautstärke.
- Bevorzugte Notennamendarstellung.
- Session- und Bedienpräferenzen.

Datenschutz:
- Mikrofon ist für den Produktumfang nicht erforderlich.
- Keine Aufzeichnung oder Analyse der Stimme.
- Persönliche Routinen und Nutzungsdaten bleiben im eigenen SingLab-System.
- Es dürfen keine unnötigen personenbezogenen Daten erhoben werden.
- Update-Prüfungen dürfen keine Trainings- oder Nutzungsdaten übertragen.

---

## 17. Hosting und Verfügbarkeit

Zielumgebung ist ein selbst gehosteter Betrieb auf YunoHost, zunächst auf einem Raspberry Pi 5 mit 8 GB RAM und ARM64-System.

Vorgesehene Domain: `singlab.ebase.ynh.fr` – noch nicht verbindlich festgelegt.

Anforderungen:
- Betrieb als eigenständige Webanwendung.
- Gute Bedienbarkeit im mobilen Browser.
- Installierbar bzw. als Web-App nutzbar, sofern vom Endgerät unterstützt.
- Kernfunktionen sollen bei geeigneter lokaler Verfügbarkeit auch ohne dauerhafte Internetverbindung nutzbar sein.
- Bei Server- oder Netzwerkproblemen müssen klare Fehlermeldungen erscheinen.
- Nutzerdaten und persönliche Übungen müssen gesichert und wiederherstellbar sein.

---

## 18. Gruppen- und gemeinsame Nutzung

Als ergänzende Nutzungsmöglichkeit soll SingLab gemeinsame Übungen unterstützen:
- Eine Session kann auf einem gemeinsamen Bildschirm angezeigt werden.
- Töne und Übungen können über Lautsprecher abgespielt werden.
- Die Gruppe kann dieselbe Übungsfolge gemeinsam durchführen.
- Die Bedienperson kann Übungen pausieren, wiederholen und wechseln.

Eine individuelle Stimmüberwachung oder Aufnahme ist auch in diesem Modus nicht vorgesehen.

---

## 19. Update- und Administrationsfunktionen

Der Adminbereich ist durch eine sechsstellige PIN geschützt. Beim allerersten Start wird die PIN eingerichtet. Vor dem Zugriff auf Adminfunktionen muss sie erneut eingegeben werden.

SingLab prüft regelmäßig, ob eine neuere Version des Projekts verfügbar ist. Ist die Anwendung geöffnet, zeigt sie eine In-App-Benachrichtigung mit Versionsnummer und Änderungsübersicht an. Updates werden bewusst durch eine administrative Aktion gestartet und unterbrechen keine laufende Session ungefragt.

Details und Sicherheitsanforderungen stehen in [ADMIN_AND_UPDATES.md](ADMIN_AND_UPDATES.md).

---

## 20. Priorisierung

### Produktkern
- Dashboard.
- Vollständiges Warm-up Studio.
- Globales Tonhöhen- und Tonartensystem.
- Tone Echo, Intervalle, Skalen, Arpeggien und Melodieübungen.
- Instrument Studio.
- Exercise Library.
- Responsives Design.
- Kein Mikrofon, keine Aufnahme.

### Vollständige Produktversion
- Pitch & Melody Lab.
- Training Generator.
- Training Plans.
- Progress.
- Eigene Übungen und Favoriten.
- Gruppenmodus.
- In-App-Updatehinweise und geschützter Adminbereich.

---

## 21. Produktprinzipien

1. SingLab soll sich wie ein vollständiges Gesangs- und Einsingstudio anfühlen.
2. Das Warm-up Studio ist ein eigenständiger Hauptbereich.
3. Alle Tonhöhen und Tonarten sind systemweit verfügbar.
4. Jede Übung muss ohne Mikrofon und ohne Aufnahme nutzbar sein.
5. Klang und visuelle Anzeige ergänzen sich.
6. Nutzerinnen und Nutzer behalten Kontrolle über Tempo, Tonart, Oktave und Ablauf.
7. Die Anwendung bewertet nicht die Stimme.
8. Privatsphäre und Selbsthosting haben einen hohen Stellenwert.
9. Updates sind transparent und werden nicht ungefragt während einer Session installiert.
10. Die Oberfläche bleibt auch für spontane, kurze Nutzung schnell verständlich.
