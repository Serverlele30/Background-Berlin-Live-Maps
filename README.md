# 🚇 Berlin Live Transit

Echtzeit-Dashboard zur Visualisierung aller öffentlichen Verkehrsmittel in Berlin – perfekt als animierter Background oder Wallpaper.

![Berlin Live Transit Demo](https://img.shields.io/badge/Status-Live-brightgreen)

## ✨ Features

- 🗺️ **Live-Tracking** aller Verkehrsmittel (U-Bahn, S-Bahn, Bus, Tram, Fähre)
- 🌙 **Dark Mode** mit animierten Fahrzeugmarkern
- ⏰ **Echtzeit-Uhr** mit deutschem Datum
- 📍 **Standorterkennung** (optional)
- ✨ **Smooth Animationen** zwischen Position-Updates
- 💫 **Kein Cursor** - perfekt als Hintergrund

## 🚀 Installation & Start

### Option 1: GitHub Pages (Empfohlen)

Einfach die GitHub Pages aktivieren:

1. Fork/Clone das Repo
2. GitHub → Settings → Pages → Source: `main` branch
3. Fertig! URL: `https://username.github.io/berlin-live-transit`

### Option 2: Lokaler Start

```bash
# Repository klonen
git clone https://github.com/username/berlin-live-transit.git
cd berlin-live-transit

# Starten mit Node.js
npm start

# ODER mit Python
python -m http.server 8000
```

Dann öffne: `http://localhost:8000`

### Option 3: Direkt öffnen

Einfach `index.html` im Browser öffnen – funktioniert sofort!

## 🎨 Verkehrsmittel-Farben

| Typ | Farbe | Icon |
|-----|-------|------|
| U-Bahn | 🔵 Blau | U |
| S-Bahn | 🟢 Grün | S |
| Straßenbahn | 🔴 Rot | T |
| Bus | 🟣 Lila | B |
| Fähre | 🔵 Cyan | F |
| Regional | 🟠 Orange | R |

## ⚙️ Konfiguration

Anpassbare Parameter in `index.html`:

```javascript
// Zoom-Level (Standard: 16)
map.setView([lat, lon], 16);

// Update-Intervall in ms (Standard: 15s)
setInterval(() => { loadRadarData(); }, 15000);

// Max. Fahrzeuge pro Request
&results=150
```

## 🛠️ Technologien

- **Leaflet.js** - Karten
- **VBB Transport REST API** - Live-Daten
- **CartoDB Dark Matter** - Dark Mode Tiles
- **Vanilla JS** - Keine Dependencies

## 📝 Nutzung als Wallpaper

1. Im Browser öffnen
2. `F11` für Vollbild
3. Optional: Als Browser-Startseite setzen
4. Auf zweitem Monitor laufen lassen

## 🌍 Browser-Support

✅ Chrome/Edge | ✅ Firefox | ✅ Safari | ✅ Opera

## 📡 API-Details

- **Quelle:** [VBB Transport REST API](https://v6.vbb.transport.rest/)
- **Update:** Alle 15 Sekunden
- **Limit:** 150 Fahrzeuge pro Request
- **Kostenlos:** Ja, mit Rate-Limit

## 📄 Lizenz & Credits

- Kartendaten: © OpenStreetMap
- Kartenstil: © CartoDB  
- Verkehrsdaten: © VBB
- Code: Open Source

---

**Made with ❤️ for Berlin** | [Report Bug](../../issues) | [Request Feature](../../issues)
