# 📁 GitHub Repository Struktur

So sollte dein GitHub Repository am Ende aussehen:

```
adventkalender-2024/
│
├── README.md                           # Projekt-Beschreibung
├── Adventkalender_erstellen.html      # Generator-Tool
├── index.html                          # Dein fertiger Kalender (optional)
│
└── (optional weitere Dateien)
    ├── mein_adventkalender_2024.html   # Alternative Kalender-Version
    ├── images/                         # Für Screenshots/Vorschau
    └── docs/                           # Für zusätzliche Dokumentation
```

---

## 🎯 Minimale Struktur (empfohlen)

Für den Start brauchst du nur:

```
adventkalender-2024/
│
├── README.md                      # Wird automatisch erstellt
└── Adventkalender_erstellen.html  # Dein Generator
```

**URL des Generators:**
```
https://DEIN-USERNAME.github.io/adventkalender-2024/Adventkalender_erstellen.html
```

---

## 🎄 Mit fertigem Kalender

Wenn du deinen Kalender auch online stellen möchtest:

```
adventkalender-2024/
│
├── README.md                      # Projekt-Beschreibung
├── Adventkalender_erstellen.html  # Generator
└── index.html                     # Dein Kalender (umbenennt!)
```

**URLs:**
- **Generator:** `https://DEIN-USERNAME.github.io/adventkalender-2024/Adventkalender_erstellen.html`
- **Kalender:** `https://DEIN-USERNAME.github.io/adventkalender-2024/` (oder `/index.html`)

---

## 🗂️ Erweiterte Struktur (optional)

Für mehrere Kalender oder professionellere Präsentation:

```
adventkalender-2024/
│
├── README.md
├── LICENSE
│
├── generator/
│   └── Adventkalender_erstellen.html
│
├── kalender/
│   ├── familie.html
│   ├── freunde.html
│   └── arbeit.html
│
├── assets/
│   ├── preview.png
│   └── logo.svg
│
└── docs/
    ├── anleitung.md
    └── faq.md
```

**Beispiel-URLs:**
- Generator: `.../adventkalender-2024/generator/Adventkalender_erstellen.html`
- Kalender Familie: `.../adventkalender-2024/kalender/familie.html`
- Kalender Freunde: `.../adventkalender-2024/kalender/freunde.html`

---

## 📝 README.md Vorlage

Erstelle eine `README.md` im Repository mit folgendem Inhalt:

```markdown
# 🎄 Mein Adventkalender 2024

Persönlicher Adventkalender erstellt mit dem Adventkalender-Generator.

## 🔗 Links

**🎁 Kalender öffnen:**  
[Zum Adventkalender](https://DEIN-USERNAME.github.io/adventkalender-2024/)

**🛠️ Eigenen Kalender erstellen:**  
[Zum Generator](https://DEIN-USERNAME.github.io/adventkalender-2024/Adventkalender_erstellen.html)

## 📱 Teilen

Teile diesen Link mit Familie und Freunden:
```
https://DEIN-USERNAME.github.io/adventkalender-2024/
```

## 🎯 Features

- ✨ 24 Türchen mit persönlichen Fotos
- 📱 Funktioniert auf allen Geräten
- 🔒 Türchen öffnen sich automatisch zum richtigen Datum
- 💾 Geöffnete Türchen bleiben gespeichert
- 📥 Bilder können heruntergeladen werden

## 💡 Anleitung

1. Besuche den Kalender-Link
2. Klicke auf ein entsperrtes Türchen
3. Genieße die Überraschung! 🎁

---

Made with ❤️ | [Generator Repository](https://github.com/M4nfr41D-spec/ADVENT-ANDROID)
```

---

## 🚀 Deployment-Checkliste

Stelle sicher, dass du folgende Schritte erledigt hast:

- [ ] Repository ist **Public**
- [ ] GitHub Pages ist aktiviert (Settings → Pages)
- [ ] Branch: **main**, Folder: **/ (root)**
- [ ] `Adventkalender_erstellen.html` ist hochgeladen
- [ ] (Optional) `index.html` ist hochgeladen
- [ ] README.md beschreibt das Projekt
- [ ] Alle Links funktionieren

---

## 🔄 Dateien hinzufügen

### Via Web-Interface:
1. "Add file" → "Upload files"
2. Datei hineinziehen
3. "Commit changes"

### Via Git:
```bash
git add DATEINAME
git commit -m "Beschreibung"
git push
```

---

## 🎨 Anpassungen

### Repository-Name ändern:
Settings → Repository name → Umbenennen → "Rename"

**⚠️ Achtung:** Die URL ändert sich dann auch!

### Repository löschen:
Settings → Danger Zone → Delete this repository

---

## 📊 Statistiken (optional)

Du kannst GitHub Insights nutzen, um zu sehen:
- Wie viele Besucher deine Seite hat
- Von wo sie kommen
- Welche Seiten am beliebtesten sind

**Insights → Traffic**

---

## 🆘 Häufige Probleme

### Problem: "404 - File not found"

**Ursachen:**
- Dateiname falsch geschrieben (Groß-/Kleinschreibung!)
- Datei nicht im richtigen Ordner
- GitHub Pages noch nicht fertig deployed (warte 2-3 Min)

**Lösung:**
1. Prüfe exakten Dateinamen im Repository
2. URL exakt mit Dateinamen abgleichen
3. Browser-Cache leeren

### Problem: Seite zeigt nur Code

**Ursachen:**
- Datei hat keine `.html` Endung
- Browser interpretiert Datei als Text

**Lösung:**
1. Stelle sicher, dass Datei `.html` am Ende hat
2. Im Repository umbenennen falls nötig
3. Browser neu laden

---

**Viel Erfolg mit deinem GitHub Repository! 🎄✨**
