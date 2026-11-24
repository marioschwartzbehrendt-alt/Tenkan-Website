# Tenkan – Webseite

Offizielle Webseite von **Tenkan** – Elektrospacerockpop aus Berlin.

Live: https://tenkan-music.netlify.app

## Inhalt

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: neue Single „The Storm“ mit Pre-Save, Cover-Fächer mit Spotify-Playern, Über mich, Fan-Wand, Kontakt, Instagram |
| `impressum.html` | Impressum (für Suchmaschinen gesperrt, E-Mail gegen Adresssammler geschützt) |
| `datenschutz.html` | Datenschutzerklärung (eRecht24, ergänzt um Formspree, Fan-Wand, Sprachspeicher) |
| `covers/` | Song-Cover |

Reine statische Seite (HTML/CSS/JavaScript), kein Build-Schritt nötig.

## Dienste

- **Hosting:** Netlify
- **Kontaktformular & Fan-Wand:** Formspree
- **Musik:** Spotify-Einbettung (lädt erst nach Klick)

## Mit Netlify verbinden

In Netlify beim Projekt unter „Project configuration“ → „Build & deploy“ dieses Repository verknüpfen.
Build-Befehl: leer lassen · Veröffentlichungsordner: `/` (Repository-Wurzel).

## Fan-Wand-Beiträge freigeben

Freigegebene Beiträge in `index.html` im Abschnitt `const FANWALL = [ … ]` eintragen, z. B.:

```js
{ name: 'Anna', text: 'The Storm läuft bei mir in Dauerschleife!' },
```
