# GitHub Pages – Lokale Vorschau mit GitHub Codespaces

## Ausgangssituation

Die persönliche Homepage (cgallier.github.io) ist eine Jekyll-basierte GitHub Pages Seite.
Um Änderungen lokal vorzuschauen, braucht man normalerweise Ruby – das war nicht installiert.

## Lösung: GitHub Codespaces

GitHub Codespaces ist eine vollständige Entwicklungsumgebung im Browser.
Kein lokales Installieren nötig, funktioniert auf jedem Gerät.
GitHub bietet **60 Stunden pro Monat kostenlos** an – für gelegentliche Updates mehr als ausreichend.

---

## Anleitung: Seite bearbeiten und vorschauen

### 1. Codespace starten

1. https://github.com/cgallier/cgallier.github.io aufrufen
2. Grünen Button **"Code"** klicken
3. Tab **"Codespaces"** wählen
4. **"Create codespace on main"** klicken
5. Warten (beim ersten Mal ca. 1–2 Minuten)

### 2. Jekyll starten (im Terminal unten im Codespace)

```bash
bundle install
bundle exec jekyll serve
```

Auf den Button **"Open in Browser"** klicken → Vorschau der Seite öffnet sich.

### 3. Änderungen machen

- Datei im Datei-Explorer links anklicken
- Bearbeiten und speichern (`Ctrl+S`)
- Jekyll aktualisiert die Vorschau automatisch

### 4. Änderungen veröffentlichen

```bash
git add .
git commit -m "kurze Beschreibung der Änderung"
git push
```

Nach ca. 1–2 Minuten sind die Änderungen live auf **https://cgallier.github.io**.

---

## Wichtige Dateien der Seite

| Datei / Ordner | Inhalt |
|---|---|
| `_config.yml` | Grundeinstellungen der Seite (Name, URL, etc.) |
| `_pages/` | Einzelne Seiten (About, CV, etc.) |
| `_posts/` | Blogbeiträge |
| `_publications/` | Publikationen |
| `_talks/` | Vorträge |
| `images/` | Bilder |
