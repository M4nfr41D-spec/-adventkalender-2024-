# 🎄 Adventkalender Generator – Anleitung

Ein persönlicher Adventkalender-Generator, der aus deinen Fotos eine einzelne HTML-Datei erstellt, die du überall teilen kannst!

## ✨ Features

- ✅ **Vollständig offline** – Deine Bilder bleiben auf deinem Gerät
- ✅ **Eine Datei** – Alle Bilder werden als Base64 eingebettet
- ✅ **Teilbar** – Per WhatsApp, E-Mail, Cloud oder Link
- ✅ **Bildkomprimierung** – Automatische Optimierung für schnelleren Versand
- ✅ **Responsiv** – Perfekt auf Handy, Tablet und Desktop
- ✅ **Kein Server nötig** – Funktioniert direkt im Browser

---

## 📱 So nutzt du den Generator

### Schritt 1: Generator öffnen

Öffne die Datei `Adventkalender_erstellen.html` in deinem Browser:
- **Lokal:** Doppelklick auf die Datei
- **Online:** Über GitHub Pages (siehe unten)

### Schritt 2: Bilder auswählen

1. Klicke auf **"Wähle 1–24 Bilder aus"**
2. Wähle deine Fotos aus (JPG oder PNG)
3. Die Reihenfolge basiert auf den **Dateinamen** (alphabetisch sortiert)

**Tipp:** Benenne deine Dateien sinnvoll:
```
01_weihnachtsbaum.jpg
02_geschenke.jpg
03_schneemann.jpg
...
```

### Schritt 3: Einstellungen anpassen (optional)

- **Bildqualität:** 80% ist ein guter Standard
  - Niedriger = kleinere Dateigröße = schnellerer Versand
  - Höher = bessere Qualität = größere Datei
  
- **Maximale Bildbreite:** 1200px empfohlen
  - Für WhatsApp: 1200px oder weniger
  - Für Vollqualität: 2000px

### Schritt 4: Kalender erstellen

1. Klicke auf **"Kalender erstellen"**
2. Warte, bis die Verarbeitung abgeschlossen ist
3. Die Datei `mein_adventkalender_2024.html` wird automatisch heruntergeladen

### Schritt 5: Teilen

Du hast jetzt eine **einzelne HTML-Datei**, die du teilen kannst:

#### Option A: WhatsApp/Telegram
- Sende die HTML-Datei direkt als Anhang
- Empfänger kann sie mit Browser öffnen

#### Option B: E-Mail
- Hänge die HTML-Datei an eine E-Mail an
- Funktioniert mit jedem E-Mail-Client

#### Option C: Cloud (Google Drive, Dropbox, etc.)
1. Lade die HTML-Datei in deine Cloud hoch
2. Erstelle einen Freigabe-Link
3. Teile den Link

#### Option D: GitHub Pages (Dauerhafter Link)
Siehe Abschnitt unten ⬇️

---

## 🌐 GitHub Pages Deployment

So hostest du deinen Kalender dauerhaft online und erstellst einen Link zum Teilen:

### Variante 1: Über GitHub Web-Interface (einfachst)

1. **Repository erstellen:**
   - Gehe zu [github.com](https://github.com)
   - Klicke auf "New Repository"
   - Name: `adventkalender-2024` (oder beliebig)
   - ✅ Public
   - ✅ Add README file
   - Klicke "Create repository"

2. **Generator hochladen:**
   - Im Repository: "Add file" → "Upload files"
   - Ziehe `Adventkalender_erstellen.html` ins Fenster
   - Klicke "Commit changes"

3. **GitHub Pages aktivieren:**
   - Gehe zu "Settings" → "Pages"
   - Source: "Deploy from a branch"
   - Branch: "main" → Ordner: "/ (root)"
   - Klicke "Save"

4. **Generator nutzen:**
   - Deine URL: `https://DEIN-USERNAME.github.io/adventkalender-2024/Adventkalender_erstellen.html`
   - Öffne diese URL im Browser
   - Erstelle deinen Kalender

5. **Kalender hochladen und teilen:**
   - Lade die generierte `mein_adventkalender_2024.html` ins Repository hoch
   - Benenne sie um in `index.html`
   - Deine Kalender-URL: `https://DEIN-USERNAME.github.io/adventkalender-2024/`
   - **Teile diesen Link!** ✨

### Variante 2: Über Git Command Line (fortgeschritten)

```bash
# Repository klonen
git clone https://github.com/DEIN-USERNAME/adventkalender-2024.git
cd adventkalender-2024

# Generator hinzufügen
cp /pfad/zu/Adventkalender_erstellen.html .

# Commit und Push
git add Adventkalender_erstellen.html
git commit -m "Generator hinzugefügt"
git push

# Kalender erstellen (lokal im Browser)
# Dann generierte Datei als index.html hochladen:
cp /pfad/zu/mein_adventkalender_2024.html index.html
git add index.html
git commit -m "Adventkalender hinzugefügt"
git push
```

---

## 🎁 Wie funktioniert der Kalender?

### Türchen öffnen
- **Gesperrt:** Türchen öffnen sich erst ab dem jeweiligen Dezember-Tag
- **Entsperrt:** Ab dem Tag kann das Türchen geöffnet werden
- **Geöffnet:** Status wird im Browser-Speicher gespeichert

### Features
- ✅ Automatisches Entsperren basierend auf aktuellem Datum
- ✅ Geöffnete Türchen bleiben geöffnet (localStorage)
- ✅ Bilder können heruntergeladen werden
- ✅ Vollbild-Ansicht mit Zoom-Möglichkeit
- ✅ Dark Mode Design
- ✅ Responsive für alle Geräte

---

## 🔧 Technische Details

### Was macht der Generator?

1. **Bilder einlesen:** Verwendet FileReader API
2. **Komprimierung:** Canvas API für Resize und Qualitätsanpassung
3. **Base64-Encoding:** Konvertiert Bilder zu Data-URLs
4. **HTML-Generation:** Erstellt vollständige, eigenständige HTML-Datei
5. **Download:** Bietet Datei zum Download an

### Dateigrößen

- **Ohne Komprimierung:** ca. 500-800 KB pro Bild → 12-19 MB für 24 Bilder
- **Mit Komprimierung (80%, 1200px):** ca. 150-250 KB pro Bild → 3-6 MB für 24 Bilder

**Empfehlung für WhatsApp:** Max. 5-8 MB Gesamtgröße
- Verwende 70-80% Qualität
- Max. 1200px Breite
- Ca. 10-15 Bilder für optimale Performance

### Browser-Kompatibilität

✅ Chrome/Edge (alle Versionen)
✅ Firefox (alle Versionen)
✅ Safari (iOS 12+, macOS 10.14+)
✅ Samsung Internet
✅ Opera

---

## 💡 Tipps & Tricks

### Bilder vorbereiten

```
✅ DO:
- Verwende aussagekräftige Dateinamen (01_name.jpg, 02_name.jpg)
- Optimiere Bilder vor dem Upload (bereits komprimiert)
- Nutze einheitliche Formate (alle JPG oder alle PNG)

❌ DON'T:
- Sehr große Bilder (>5000px) → dauert lange
- Zu viele Bilder auf einmal → Browser kann abstürzen
- Sonderzeichen in Dateinamen → Sortierung könnte falsch sein
```

### WhatsApp-Versand

```
Problem: Datei zu groß für WhatsApp
Lösung:
1. Reduziere Bildqualität auf 60-70%
2. Verkleinere Bildbreite auf 800-1000px
3. Verwende weniger Bilder (z.B. 12 statt 24)
4. Teile in zwei Kalender auf (1-12 und 13-24)
```

### Performance

```
Bei vielen/großen Bildern:
1. Schließe andere Browser-Tabs
2. Warte nach jedem Bild kurz
3. Verwende Chrome/Edge (schnellere Canvas-Performance)
4. Auf älteren Geräten: Max. 12 Bilder
```

---

## 🐛 Fehlerbehebung

### Generator lädt nicht

```
Problem: Datei öffnet sich nicht im Browser
Lösung: 
- Rechtsklick → Öffnen mit → Chrome/Firefox
- Dateiendung prüfen: Muss .html sein
- Auf macOS: Sicherheitseinstellungen prüfen
```

### Bilder werden nicht verarbeitet

```
Problem: "Fehler beim Erstellen des Kalenders"
Lösung:
- Nur JPG/PNG verwenden (kein HEIC, WEBP, etc.)
- Bildgröße prüfen (max. 20 MB pro Bild)
- Einzeln testen: Erst 1 Bild, dann mehr
- Browser-Console öffnen (F12) für Details
```

### Kalender zeigt keine Bilder

```
Problem: Türchen öffnen sich, aber Bilder fehlen
Lösung:
- Prüfe, ob HTML-Datei vollständig heruntergeladen wurde
- Öffne Datei mit "Rechtsklick → Öffnen mit → Browser"
- Nicht mit Texteditor öffnen!
- Dateigröße prüfen: Muss mehrere MB groß sein
```

### Datum ist falsch

```
Problem: Türchen entsperren sich nicht/zu früh
Lösung:
- Systemzeit deines Geräts prüfen
- Zeitzone korrekt einstellen
- Browser-Cache leeren
- In Entwickler-Tools (F12) Datum simulieren
```

---

## 📝 Beispiel-Workflow

### Szenario: Kalender für Familie erstellen

1. **Vorbereitung (10 Min):**
   - 24 Familienfotos aus 2024 sammeln
   - Umbenennen: `01_silvester.jpg`, `02_skiurlaub.jpg`, etc.
   - Fotos in einen Ordner legen

2. **Erstellung (5 Min):**
   - Generator öffnen
   - Alle 24 Bilder auswählen
   - Qualität: 75%, Breite: 1200px
   - "Kalender erstellen" klicken

3. **Teilen (2 Min):**
   
   **Option A – WhatsApp:**
   - Datei direkt an Familie-Gruppe senden
   - Nachricht: "Unser Familienkalender 2024! 🎄"
   
   **Option B – Link:**
   - Auf GitHub Pages hochladen
   - Link teilen: `https://username.github.io/familie-advent-2024/`

4. **Nutzen:**
   - Familie öffnet täglich ein Türchen
   - Schöne Erinnerungen werden geteilt
   - Jeder kann Bilder herunterladen

---

## 🎨 Anpassungen

### Farben ändern

Öffne die generierte HTML und suche nach:
```css
:root {
  --bg-dark:#020617;          /* Hintergrund */
  --accent-gold:#facc15;      /* Akzentfarbe */
  --accent-green:#16a34a;     /* Grün für geöffnete Türchen */
}
```

### Text ändern

Suche in der HTML nach:
```html
<h1>Dein <span>Weihnachts-Adventkalender</span></h1>
```

### Mehr/weniger Türchen

Ändere in Generator und Kalender:
```javascript
const TOTAL_DAYS = 24; // Z.B. auf 12 für nur erste Dezember-Hälfte
```

---

## 🚀 Updates & Erweiterungen

### Geplante Features

- [ ] Unterstützung für Videos
- [ ] Custom Nachrichten pro Türchen
- [ ] Countdown bis Weihnachten
- [ ] Schneeflocken-Animation
- [ ] Sound-Effekte beim Öffnen
- [ ] Vorschau vor dem Erstellen

### Mitmachen

Hast du Ideen oder Verbesserungen? 
- Erstelle ein Issue auf GitHub
- Fork das Repository und erstelle einen Pull Request
- Teile deine Version!

---

## 📄 Lizenz

MIT License – Nutze und verändere den Code nach Belieben!

---

## 💖 Credits

Made with ❤️ for creating personal advent calendars

---

## 🆘 Support

Bei Fragen oder Problemen:
1. Lies die Fehlerbehebung oben
2. Erstelle ein Issue auf GitHub
3. Kontaktiere mich über GitHub

---

**Viel Spaß beim Erstellen deines Adventkalenders! 🎄✨**
