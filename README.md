# JumpDock

**Dynamischer Schnellstarter für Windows** – integriert sich nahtlos in die
Windows-Taskleiste (Jump Lists) und den System Tray.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-blue)
![Version](https://img.shields.io/badge/version-1.1.0-brightgreen)
![Language](https://img.shields.io/badge/language-DE%20%7C%20EN-lightgrey)
![License](https://img.shields.io/badge/license-Proprietary-red)

---

## Über JumpDock

JumpDock ist ein schlanker App-Launcher, der im Hintergrund läuft und deine
Lieblingsprogramme blitzschnell erreichbar macht – **ohne** den Desktop
zuzumüllen. Statt Verknüpfungen auf dem Desktop oder im Startmenü zu suchen,
startest du deine Programme direkt per:

- **Rechtsklick auf das Taskleisten-Icon** → Kategorie „Schnellstart"
  (Windows Jump List)
- **Rechtsklick auf das Tray-Icon** → sortierte Liste deiner Apps

Alles wird zentral in einem modernen Einstellungsfenster verwaltet, inklusive
Kategorien, Icons, Reihenfolge und optionalem Autostart.

**Entwickler:** Vecchio Lopez Consulting

---

## Features

- 📌 **Taskleisten-Jump-List** – deine Apps erscheinen beim Rechtsklick auf
  das gepinnte Taskleisten-Icon
- 🔔 **System-Tray-Menü** – dynamische App-Liste mit Kategorien
- 🗂️ **Kategorien** – eigene Gruppen anlegen, umbenennen, sortieren, löschen
- 🌍 **Zweisprachig** – Deutsch & Englisch, Live-Umschaltung in der Toolbar
- 🎨 **Modernes UI** – CustomTkinter, Dark/Light/System-Theme
- ⚡ **Admin-Ausführung pro App** – UAC-Prompt bei Bedarf
- 🔍 **Suche & Icon-Anzeige** in der App-Liste
- 📥 **Import/Export** der Konfiguration (JSON)
- 🔁 **Autostart** mit Windows
- 🖥️ **Start minimiert** im Tray
- 🛡️ **Robustheit** – atomares Speichern, versionierte Config, rotierendes Logfile

---

## Download

**Aktuelle Version:** v1.1.0

[![Download JumpDock.exe](https://img.shields.io/badge/Download-JumpDock.exe-1e90ff?style=for-the-badge&logo=windows)](https://github.com/dvelop/JumpDock-Releases/releases/latest/download/JumpDock.exe)

➡️ **[JumpDock.exe herunterladen](https://github.com/dvelop/JumpDock-Releases/releases/latest/download/JumpDock.exe)**

Alle Versionen: [Releases](https://github.com/dvelop/JumpDock-Releases/releases)

> **Systemvoraussetzungen:** Windows 10 oder 11 (64-bit). Kein Python, keine
> Installation nötig – die `.exe` ist eine eigenständige Single-File-Anwendung.

---

## Installation

JumpDock ist **portabel** im Sinne der Ausführung: Du musst nichts installieren.
Einfach herunterladen und starten.

### Schritt 1 – Herunterladen

Lade die aktuellste `JumpDock.exe` aus dem
[Releases-Bereich](https://github.com/dvelop/JumpDock-Releases/releases/latest)
herunter.

### Schritt 2 – SmartScreen-Warnung umgehen

Da JumpDock **nicht code-signiert** ist, zeigt Windows beim ersten Start
folgende Warnung (SmartScreen):

> „Der Computer wurde durch Windows geschützt – Unbekannter Herausgeber."

**So startest du trotzdem:**

1. Im Dialog auf **„Weitere Informationen"** klicken
2. Dann auf **„Trotzdem ausführen"** klicken

Die Datei wird danach nicht mehr gewarnt, sofern sie am selben Ort bleibt.

> 💡 Wenn du willst, kannst du die `.exe` vor dem Start mit einem Virenscanner
> prüfen. Der Quellcode ist auf Anfrage beim Entwickler einsehbar.

### Schritt 3 – An einen festen Ort verschieben

Empfohlen: `C:\Program Files\JumpDock\` oder `C:\Tools\JumpDock\`

**Wichtig:** Lege die `.exe` an einen **lokalen Pfad** (nicht auf ein
Netzlaufwerk) – das beschleunigt den Start und sorgt dafür, dass Windows die
Jump List korrekt zuordnet.

### Schritt 4 – Starten

Doppelklick auf `JumpDock.exe`. Beim ersten Start:

- Es öffnet sich das **Einstellungsfenster** (oder das Tray-Icon erscheint
  in der Taskleiste, falls „Minimiert starten" aktiv ist)
- Du kannst sofort loslegen

---

## Erste Schritte

### 1. Apps hinzufügen

1. Rechtsklick auf das **Tray-Icon** (unten rechts in der Taskleiste)
2. **„Einstellungen öffnen"** wählen
3. Toolbar → **„+ App hinzufügen"** klicken
4. Datei auswählen: `.exe`, `.lnk`, `.bat` oder `.cmd`
5. Anzeigename und Kategorie anpassen (optional)
6. **„Speichern"** klicken

Deine Apps erscheinen jetzt sofort im Tray-Menü und in der Taskleisten-Jump-List.

### 2. Kategorien anlegen

1. Toolbar → **„Kategorien"** klicken
2. Kategorie erscheint automatisch, sobald du sie im App-Bearbeiten-Dialog
   vergibst – oder du legst sie dort direkt an
3. Mit **↑ / ↓** die Reihenfolge festlegen (gilt für Tray-Menü & Jump List)
4. Mit **✎** umbenennen, mit **🗑** löschen (betroffene Apps werden
   unkategorisiert)

### 3. Sprache wechseln

Toolbar → Sprach-Dropdown → **Deutsch / English / Auto**

Der Wechsel wirkt sofort auf alle Labels, Dialoge und die Jump-List-Kategorie
(„Schnellstart" ↔ „Quick Start"). Die Wahl wird gespeichert.

### 4. Taskleisten-Jump-List aktivieren

Damit deine Apps im **Rechtsklick-Menü des Taskleisten-Icons** erscheinen:

1. JumpDock starten (aus dem lokalen Pfad, siehe [Installation](#installation))
2. Rechtsklick auf das **Taskleisten-Icon** von JumpDock
3. **„An Taskleiste anheften"** wählen
4. Jetzt: Rechtsklick auf das **gepinnte** Icon
5. Kategorie **„Schnellstart"** (bzw. deine Kategorien) erscheint

> ⚠️ Die Jump List funktioniert **nur** mit der angehefteten Verknüpfung.
> Wenn die Kategorie nicht sofort sichtbar ist: einmal ab- und wieder
> anheften, oder den Windows-Explorer neu starten.

### 5. Autostart einrichten

Einstellungen → Toggle **„Mit Windows starten"** aktivieren → Speichern.

---

## System Tray

Das Tray-Icon ist der zentrale Einstiegspunkt:

| Aktion | Ergebnis |
|---|---|
| **Linksklick** auf Tray-Icon | Einstellungen öffnen |
| **Rechtsklick** auf Tray-Icon | Kontextmenü mit allen Apps + Optionen |
| Rechtsklick → App-Name | App starten |
| Rechtsklick → Kategorie | Untermenü mit Apps dieser Kategorie |
| Rechtsklick → Einstellungen öffnen | Einstellungsfenster nach vorne holen |
| Rechtsklick → Beenden | JumpDock sauber beenden |

**Tray-Icon nicht sichtbar?** Windows 11 blendet neue Icons standardmäßig aus:

→ Taskleiste-Einstellungen → **„Andere Systemtray-Symbole"** → JumpDock
auf **„Ein"** stellen.

---

## Konfiguration

Alle Daten liegen unter:

```
%APPDATA%\JumpDock\
├── config.json          ← Apps, Kategorien, Sprache, Theme
├── logs\jumpdock.log    ← Logdatei (bei Problemen hilfreich)
└── tasks\*.lnk          ← Jump-List-Cache (automatisch verwaltet)
```

**Schnellzugriff:**

```powershell
explorer "$env:APPDATA\JumpDock"
```

### Backup & Umzug

- **Export:** Einstellungen → **„Exportieren"** → JSON-Datei speichern
- **Import:** Einstellungen → **„Importieren"** → JSON-Datei auswählen
- **Manuell:** `%APPDATA%\JumpDock\config.json` kopieren

---

## Deinstallation

JumpDock hinterlässt keine Spuren im System außer:

1. **Autostart-Eintrag entfernen** (falls aktiviert):
   - Einstellungen → Toggle „Mit Windows starten" ausschalten → Speichern
   - Oder per Registry:
     ```powershell
     reg delete "HKCU\Software\Microsoft\Windows\CurrentVersion\Run" /v JumpDock /f
     ```

2. **Taskleisten-Verknüpfung lösen:** Rechtsklick auf das gepinnte Icon →
   **„Von Taskleiste lösen"**

3. **Konfiguration & Logs löschen:**
   ```powershell
   Remove-Item -Recurse -Force "$env:APPDATA\JumpDock"
   ```

4. **`.exe` löschen** – einfach die Datei entfernen.

---

## Fehlerbehebung

| Symptom | Lösung |
|---|---|
| **SmartScreen blockiert den Start** | „Weitere Informationen" → „Trotzdem ausführen" |
| **Tray-Icon nicht sichtbar** | Windows 11: Einstellungen → Taskleiste → Andere Systemtray-Symbole → JumpDock auf „Ein" |
| **Jump List bleibt leer** | App muss über `.exe` laufen UND an Taskleiste angeheftet sein (siehe [Schritt 4](#4-taskleisten-jump-list-aktivieren)) |
| **Apps erscheinen nicht im Tray nach dem Speichern** | Log prüfen: `%APPDATA%\JumpDock\logs\jumpdock.log` |
| **Start dauert lange** | `.exe` liegt auf Netzlaufwerk → nach `C:\` kopieren |
| **Zweite Instanz startet nicht** | Normal (Single-Instance-Schutz). Nutze `JumpDock.exe --show` oder klicke das Tray-Icon |
| **Sprache wechselt nicht** | Prüfe `config.json` → `"language"`-Wert; App neu starten |
| **Autostart funktioniert nicht** | `reg query "HKCU\Software\Microsoft\Windows\CurrentVersion\Run" /v JumpDock` |

**Bei Problemen:** Logfile-Auszug aus `%APPDATA%\JumpDock\logs\jumpdock.log`
mitbringen (letzte 50 Zeilen reichen) – entweder als
[GitHub Issue](https://github.com/dvelop/JumpDock-Releases/issues) oder direkt
an den Entwickler.

---

## CLI-Optionen

JumpDock unterstützt auch Kommandozeilen-Aufrufe:

```powershell
JumpDock.exe --list                    # Alle konfigurierten Apps anzeigen
JumpDock.exe --launch "Notepad"        # App per Name starten
JumpDock.exe --show                    # Fenster der laufenden Instanz holen
JumpDock.exe --quit                    # Laufende Instanz beenden
JumpDock.exe --portable                # Config neben der .exe
JumpDock.exe --debug                   # Debug-Logging auf stderr
```

---

## Quellcode

Der Quellcode wird **separat** gepflegt und ist auf Anfrage beim Entwickler
erhältlich.

**Vecchio Lopez Consulting**

Falls du als Contributor Interesse hast oder die App in deinem Umfeld eingesetzt
wird und Anpassungen brauchst – gerne Kontakt aufnehmen.

---

## Changelog

### v1.1.0 (aktuell)
- ✨ Info-Dialog mit Version & Entwickler
- ✨ Sprache live umschaltbar (Toolbar) – Deutsch / English / Auto
- ✨ Jump-List-Kategorienamen werden übersetzt
- ✨ Eigenes App-Icon (Multi-Resolution-ICO)
- 🐛 Tray-Menü: App-Einträge erscheinen jetzt zuverlässig nach dem Speichern
- 🐛 Stabilität: atomares Config-Speichern, versionierte Config (v4)

### v1.0.0
- 🎉 Erste öffentliche Version
- Taskleisten-Jump-List, System Tray, Kategorien, Autostart, Import/Export

---

## Lizenz

**Proprietär** – © Vecchio Lopez Consulting. Alle Rechte vorbehalten.

Die `.exe` darf **kostenlos** für private und geschäftliche Zwecke genutzt
werden. Weiterverbreitung, Dekompilierung oder Modifikation sind ohne
schriftliche Genehmigung nicht gestattet.

Für kommerzielle Lizenzen oder individuelle Anpassungen:
**Kontakt: Vecchio Lopez Consulting**

---

## Danksagung

JumpDock nutzt folgende Open-Source-Projekte:

- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) – Modernes Tkinter-UI
- [pystray](https://github.com/moses-palmer/pystray) – System-Tray-Integration
- [Pillow](https://python-pillow.org/) – Bildverarbeitung
- [pywin32](https://github.com/mhammond/pywin32) – Windows-Integration
- [comtypes](https://github.com/enthought/comtypes) – COM-Schnittstellen (Jump Lists)
- [PyInstaller](https://pyinstaller.org/) – `.exe`-Packaging

Ohne diese Projekte wäre JumpDock nicht möglich. Danke an alle Maintainer!

---

<div align="center">

**Made with ☕ in Germany**

[⬆ Nach oben](#jumpdock) · [Releases](https://github.com/dvelop/JumpDock-Releases/releases) · [Issues](https://github.com/dvelop/JumpDock-Releases/issues)

</div>
