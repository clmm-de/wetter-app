# ⛅ Wetter-App

Eine Progressive Web App (PWA) für Wettervorhersagen, basierend auf der kostenlosen [Open-Meteo API](https://open-meteo.com).

![Wetter-App Screenshot](https://img.shields.io/badge/PWA-installierbar-5eead4?style=for-the-badge)
![Open-Meteo](https://img.shields.io/badge/API-Open--Meteo-38bdf8?style=for-the-badge)

## ✨ Features

- 🌡️ **Aktuelles Wetter** – Temperatur, Gefühlt, Wind, Böen, Feuchte, Druck, Wolken
- 📅 **16-Tage Vorhersage** – mit Temperaturbalken und Wettericons
- ⏰ **Stunden-Detail** – tippe auf einen Tag für 2h-Intervall-Prognosen
- 📍 **Ortsverwaltung** – beliebig viele Orte speichern und verwalten
- ⭐ **Standardort** – wird beim Öffnen automatisch geladen
- 🔍 **Ortsuche** – über Open-Meteo Geocoding API (Stadt oder PLZ)
- 📱 **Installierbar** – als App auf iOS und Android
- 📡 **Offline-fähig** – letzte Wetterdaten werden gecacht
- 🇩🇪 **Komplett deutsch** – Oberfläche und Wetterbeschreibungen

## 🚀 Installation

### Option 1: GitHub Pages (empfohlen)

1. Forke dieses Repository
2. Gehe zu **Settings → Pages**
3. Wähle Branch `main` und Ordner `/ (root)`
4. Klicke **Save**
5. Nach ~1 Minute erreichbar unter `https://DEIN-USERNAME.github.io/wetter-app/`

### Option 2: Netlify

1. Gehe zu [app.netlify.com/drop](https://app.netlify.com/drop)
2. Ziehe den gesamten Projektordner per Drag & Drop
3. Sofort live unter einer `*.netlify.app` URL

### Option 3: Beliebiger Webserver

Kopiere alle Dateien auf einen Webserver. HTTPS ist für die PWA-Installation erforderlich.

## 📱 Auf dem Handy installieren

### iPhone (Safari)
1. Seite in **Safari** öffnen
2. **Teilen-Button** (□↑) tippen
3. **„Zum Home-Bildschirm"** wählen

### Android (Chrome)
1. Seite in **Chrome** öffnen
2. **Drei-Punkte-Menü** (⋮)
3. **„App installieren"** oder **„Zum Startbildschirm hinzufügen"**

## 📁 Projektstruktur

```
wetter-app/
├── index.html        ← Haupt-App (HTML/CSS/JS in einer Datei)
├── manifest.json     ← PWA-Manifest
├── sw.js             ← Service Worker (Offline-Cache)
├── icons/
│   ├── favicon.svg   ← Browser-Favicon
│   ├── icon-192.png  ← PWA-Icon (192x192)
│   └── icon-512.png  ← PWA-Icon (512x512)
└── README.md
```

## 🔧 Technologie

- **Vanilla HTML/CSS/JS** – keine Build-Tools, keine Dependencies
- **Open-Meteo Forecast API** – 16-Tage Vorhersage, stündliche Daten
- **Open-Meteo Geocoding API** – Ortssuche weltweit
- **Service Worker** – Offline-Cache für App-Shell und API-Daten
- **localStorage** – persistente Ortsliste und Wetter-Cache

## 📄 Lizenz

App-Code: MIT License  
Wetterdaten: [Open-Meteo](https://open-meteo.com) – [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
