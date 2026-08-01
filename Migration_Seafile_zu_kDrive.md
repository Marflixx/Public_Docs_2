# Migration von Seafile zu kDrive – Anleitung für Teammitglieder

*eartheffect — Umstieg der gemeinsamen Ablage von Seafile Cloud auf Infomaniak kDrive*

Erstellt für: Team eartheffect · Stand: 1. August 2026

## 1. Worum geht es

Wir stellen unsere gemeinsame Dateiablage von Seafile Cloud auf Infomaniak kDrive um. Die Migration der Dateien selbst läuft zentral über einen synchronisierten Abgleich direkt vom Seafile-Server zu kDrive — ihr müsst **keine Dateien selbst hochladen oder manuell verschieben**. Diese Anleitung beschreibt, was ihr als Teammitglied vor, während und nach der Migration tun müsst.

## 2. Vor der Migration

- Stellt sicher, dass euer lokaler Seafile-Client vollständig synchronisiert ist (Status "auf dem neusten Stand", keine ausstehenden Uploads, keine Konfliktdateien). Nur was auf dem Seafile-Server liegt, wird migriert — lokale, noch nicht hochgeladene Änderungen würden sonst nicht übernommen.
- Schliesst nach Möglichkeit laufende Bearbeitungen an Dateien ab (speichern, schliessen), damit keine Datei während des Syncs offen/gesperrt ist.

## 3. Sync-Fenster – bitte keine Änderungen

Sobald der zentrale Sync gestartet ist (Ankündigung folgt jeweils im Team-Chat), bitten wir darum, **keine Dateien in Seafile mehr zu bearbeiten oder neu abzulegen**, bis die Migration bestätigt ist. Das stellt sicher, dass keine Änderung "zwischen" dem Snapshot verloren geht.

Der Sync selbst überträgt nur neue oder geänderte Dateien; bereits identische, unveränderte Dateien auf kDrive werden nicht angerührt.

## 4. Nach der Bestätigung: Umstieg auf kDrive

Erst wenn die Migration im Team-Chat als abgeschlossen und geprüft gemeldet wurde, geht ihr wie folgt vor:

1. **Seafile-Client trennen:** Beendet den Seafile-Desktop-Client bzw. entkoppelt die Synchronisation. Eure Daten sind zu diesem Zeitpunkt bereits doppelt gesichert (auf dem Seafile-Server und auf kDrive) — der lokale Ordner ist danach nicht mehr die einzige Kopie.
2. **Lokalen Seafile-Ordner löschen:** Damit schafft ihr Platz, bevor kDrive lokal synchronisiert wird. Das ist besonders wichtig, wenn der Speicherplatz auf eurem Rechner knapp ist — Seafile-Ordner und kDrive-Ordner sollten nie gleichzeitig vollständig lokal vorliegen.
3. **kDrive-Desktop-App installieren:** [Download-Link kDrive](https://www.infomaniak.com/en/apps/download-kdrive), mit eurem Infomaniak-Konto anmelden.
4. **Lite Sync aktivieren (Windows/macOS):** Damit werden Dateien lokal nur als Platzhalter angezeigt und erst beim Öffnen tatsächlich heruntergeladen. Das spart massiv Speicherplatz — ihr müsst nicht die komplette Ablage lokal vorhalten, sondern nur das, was ihr aktiv braucht.
5. Wählt den Ordner **"Common documents"** zur Synchronisation aus.

## 5. Wichtig: Reihenfolge einhalten

Bitte nicht Seafile- und kDrive-Ordner parallel lokal behalten, um Speicherplatz zu sparen und Verwirrung durch zwei parallele Ablagen zu vermeiden:

Migration abgeschlossen & bestätigt → Seafile-Ordner löschen → kDrive-App installieren & synchronisieren.

## 6. Bei Problemen

Meldet euch bei Martin ([raeber@eartheffect.ch](mailto:raeber@eartheffect.ch)), falls:

- nach dem Umstieg Dateien in kDrive fehlen oder nicht aktuell aussehen,
- der Seafile-Client vor dem Trennen Konflikte oder ausstehende Uploads anzeigt,
- die kDrive-App sich nicht mit dem Infomaniak-Konto verbinden lässt.
