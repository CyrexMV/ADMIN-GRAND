# GRAND RP · Admin-Bewerbung

Persönliche Bewerbung von **Scott Sanchez** für das Admin-Team von GRAND RP – als statische, moderne Website ohne Build-Schritt.

## Seiten

| Datei | Inhalt |
| --- | --- |
| `index.html` | Startseite mit Hero, Kennzahlen, Absicht und Kapitelübersicht |
| `ueber-mich.html` | Kapitel 01 – Profil, Haltung und Werte |
| `voraussetzungen.html` | Kapitel 02 – Alle Kriterien mit Statuscheck (4 / 4) |
| `erfahrung.html` | Kapitel 03 – Organisationen, Regelwerk, Motivation, Wochenplan |
| `bewerbung.html` | Kapitel 04 – Vollständige Bewerbung mit Inhaltsverzeichnis, Kopier- und Druckfunktion |

## Struktur

```
assets/
  css/main.css   Design-System (Tokens, Layout, Komponenten, Seiten, Druck)
  js/main.js     Interaktionen (Theme, Menü, Reveal, Spotlight, Tilt, Kopieren, Scrollspy)
  img/           Logo als WebP (96 / 400 / 800 px), JPEG-Fallback, Social-Preview
favicon.svg
apple-touch-icon.png
```

## Features

- **Hell- & Dunkelmodus** per Umschalter (wird im Browser gemerkt), umgesetzt mit `light-dark()`
- **Seitenübergänge** über die View Transitions API, Scroll-Fortschritt und Text-Einfärbung über Scroll-Driven Animations
- **Interaktive Details**: 3D-Tilt des Wappens, Spotlight-Karten, animierte Zähler und Checkmarks
- **Mobil zuerst**: responsives Layout, eigenes Mobil-Menü, kein horizontales Scrollen
- **Barrierearm**: Skip-Link, Fokus-Stile, ARIA-Labels, `prefers-reduced-motion` wird respektiert
- **Druck / PDF**: eigenes Druck-Layout für die vollständige Bewerbung
- **Schnell**: Bilder von 865 KB auf ~76 KB (WebP) reduziert, keine Abhängigkeiten außer Google Fonts
- Alles ist *progressive enhancement* – ohne JavaScript bleibt jede Seite vollständig lesbar.

## Lokal ansehen

Einfach `index.html` im Browser öffnen oder einen lokalen Server starten:

```bash
npx serve .
```

## Hinweise

- Die Seiten sind mit `noindex` markiert, damit das private Dokument nicht in Suchmaschinen landet.
- Für Link-Vorschauen (z. B. in Discord) brauchen `og:image`-Angaben eine absolute URL. Sobald die Seite gehostet ist (z. B. GitHub Pages), den Pfad `assets/img/og-image.jpg` in den `<head>`-Bereichen durch die vollständige URL ersetzen.
