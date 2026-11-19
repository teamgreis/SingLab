# SingLab

**SingLab** ist eine selbst gehostete Vocal-Training-Plattform. Sie hilft dabei, die Stimme vor dem Singen gezielt aufzuwärmen, Tonhöhen kennenzulernen und musikalische Übungen durchzuführen – ohne Mikrofon, ohne Sprachaufnahme und ohne automatische Stimmanalyse.

## Projektstatus

Aktuell wird das Produktkonzept und die vollständige fachliche Spezifikation vorbereitet. Dieses Repository dient als zentrale Quelle für Produktumfang, Nutzererlebnis, Anforderungen und Abnahmekriterien. Die Umsetzung kann anschließend durch die vorgesehenen Entwicklungsagenten erfolgen.

## Dokumentation

- [Vollständige Produktspezifikation](docs/PRODUCT_SPECIFICATION.md)
- [Adminbereich, PIN-Schutz und Updates](docs/ADMIN_AND_UPDATES.md)
- [Abnahmekriterien](docs/ACCEPTANCE_CRITERIA.md)

## Grundprinzipien

- Audioausgabe über Lautsprecher oder Kopfhörer; kein Mikrofon erforderlich.
- Keine Aufnahme, Speicherung oder Übertragung der Stimme.
- Ein vollständiges, eigenständiges Warm-up Studio.
- Alle zwölf chromatischen Tonklassen, Tonarten, Skalen und geeigneten Oktavlagen.
- Individuell konfigurierbare Übungen und Trainingsprogramme.
- Selbst gehosteter Betrieb, zunächst auf dem Raspberry Pi 5 mit YunoHost.
- Verständliche Update-Hinweise und ein separat geschützter Adminbereich.

## Geplante Standardumgebung

- Hosting: YunoHost
- Hostsystem: Raspberry Pi 5 (ARM64)
- Vorgesehene Adresse: `singlab.ebase.ynh.fr` (noch nicht verbindlich festgelegt)

## Sicherheit und Privatsphäre

Die Admin-PIN wird ausschließlich lokal und geschützt gespeichert. Zugangsdaten, PINs, PIN-Hashes und sonstige Geheimnisse dürfen niemals in dieses Repository eingecheckt werden. SingLab benötigt für die beschriebenen Kernfunktionen keinen Mikrofonzugriff.

## Lizenz

Noch festzulegen.
