# KC-Kodi Repository

Ein vollständig funktionierendes Kodi Repository mit Add-ons, Plugins und IPTV-Unterstützung.

## Inhaltsverzeichnis

- [Features](#features)
- [Repository-Struktur](#repository-struktur)
- [Installation](#installation)
- [Verfügbare Add-ons](#verfügbare-add-ons)
- [TV Streaming](#tv-streaming)
- [EPG Guide](#epg-guide)

## Features

✅ Kodi-kompatible Add-ons und Repositories
✅ Video-Streaming-Plugins
✅ IPTV/M3U TV-Listen
✅ EPG (Electronic Program Guide) Integration
✅ Automatische Add-on-Updates
✅ Web-Interface für Repository-Verwaltung

## Repository-Struktur

```
├── repo/                    # Kodi Add-ons und Repositories
│   ├── plugin.video.*      # Video-Streaming Add-ons
│   ├── plugin.program.*    # Programm-Add-ons
│   ├── script.module.*     # Skript-Module
│   ├── service.*           # Service-Add-ons
│   ├── repository.*        # Link zu anderen Repositories
│   ├── addons.xml          # Manifest aller Add-ons
│   └── addons.xml.md5      # MD5-Checksumme
├── assets/                 # Zusätzliche Assets
├── logos/                  # Channel-Logos
├── tvs-logos/              # TV-Sender Logos
├── guide.xml               # EPG-Daten (unkomprimiert)
├── guide.xml.gz            # EPG-Daten (komprimiert)
├── tv.m3u                  # Haupt-TV-Liste
├── tv2.m3u                 # Alternative TV-Liste
├── maclist.json            # MAC-Adresse Liste
└── index.html              # Web-Interface
```

## Installation

### Methode 1: Direktes Hinzufügen in Kodi

1. Öffne Kodi und gehe zu **Einstellungen → Add-ons → Meine Add-ons**
2. Wähle **Repository installieren**
3. Gib folgende URL ein:
   ```
   https://raw.githubusercontent.com/chrisklietsch/repository.kc-kodi/main/
   ```

### Methode 2: ZIP-Datei
1. Lade das Repository als ZIP herunter
2. In Kodi: **Einstellungen → Add-ons → Aus ZIP-Datei installieren**
3. Wähle die heruntergeladene ZIP-Datei

## Verfügbare Add-ons

Das Repository enthält folgende Add-on-Kategorien:

### Video-Plugins
- `plugin.video.stalkermod` - Stalker IPTV Plugin
- `plugin.video.xstream` - xStream Video Plugin
- `plugin.video.xship` - xShip Video Streaming
- `plugin.video.vavooto` - Vavooto Video Service
- `plugin.video.vavoo` - Vavooto Video Service (Pure Version ohne Stalker)
- `plugin.video.tools` - Video Tools & Utilities

### Program & Tools
- `plugin.program.autocompletion` - Auto-Completion Tool
- `script.module.asyn` - Async Module
- `script.module.download-m3u8` - M3U8 Download Module
- `script.module.xstreamcscraper` - xStream Scraper

### Repositories (Abhängigkeiten)
- `repository.michaz` - Michaz Repository
- `repository.gujal` - Gujal Repository
- `repository.kodinerds` - Kodi Nerds Repository
- `repository.slyguy` - SlyGuy Repository
- Und weitere...

### Services
- `service.takealug.epg-grabber` - EPG Grabber Service

## TV-Streaming

### M3U-Listen

Das Repository enthält zwei M3U-Playlisten für IPTV:

- **tv.m3u** - Hauptliste der verfügbaren TV-Kanäle
- **tv2.m3u** - Alternative TV-Kanalliste

Diese können in folgendem Format in Kodi verwendet werden:
```
http://raw.githubusercontent.com/chrisklietsch/repository.kc-kodi/main/tv.m3u
```

### Verwendung in Kodi

1. Installiere ein IPTV-Plugin (z.B. PVR IPTV Simple Client)
2. Konfiguriere die Playlist-URL zu einer der M3U-Dateien
3. Aktiviere das Plugin

## EPG-Guide

Das Repository enthält Electronic Program Guide (EPG) Daten:

- **guide.xml** - Vollständige EPG-Daten (unkomprimiert)
- **guide.xml.gz** - Komprimierte EPG-Daten (empfohlen)

Dateigröße:
- Unkomprimiert: ~4.5 MB
- Komprimiert: ~900 KB

## Verwendung

```bash
# Repository lokal testen
python3 -m http.server 8000

# Dann in Kodi:
# http://localhost:8000
```

## Web-Interface

Das Repository hat ein Web-Interface zur Verwaltung:
- **main/index.html** - Repository Startseite
- **repo/index.html** - Add-ons Übersicht

## Lizenz

Dieses Repository teilt die Community-Nutzung als Sammlung von Streaming- und IPTV-Add-ons.

## Support

- 📧 Issues und Feature-Anfragen über GitHub
- 🔗 Links zu den einzelnen Add-on-Repositories

## Hinweise

⚠️ Dieses Repository kann inoffizieller Inhalte enthalten. Die Nutzung liegt in der Verantwortung des Benutzers.
⚠️ Stelle sicher, dass deine lokale Kodi-Installation aktualisiert ist.

### Angepasste Add-ons

Folgende Add-ons wurden vollständig neu angepasst und optimiert:

- **plugin.video.xship** - Mit erweiterten deutschen Scrapern
  - 28 funktionierende Scraper

- **plugin.video.xstream** - Mit erweiterten deutschen Streamingquellen  
  - 26 funktionierende Streaming-Seiten

---

*Zuletzt aktualisiert: Februar 2026*