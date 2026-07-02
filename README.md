# d'stärnä bar — Event-Website

Eine One-Page-Website im Retro-70er-Stil für die Standaktion **d'stärnä bar**
(Fritig, 21. August 2026, Lockstadt bim Inseli). Mir sammle Spände für
[Little Big Hero](https://www.littlebighero.ch).

Reine statische Website (HTML + CSS, keine Build-Tools) — direkt auf GitHub Pages hostbar.

## Dateien

| Datei | Zweck |
|-------|-------|
| `index.html` | Inhalt der Seite |
| `style.css` | Design, Farben, Schriften, Sonnenstrahlen |

Schriften werden über Google Fonts geladen (Bagel Fat One + Poppins).

## Lokal anschauen

Einfach `index.html` im Browser öffnen — oder mit einem kleinen Server:

```bash
python3 -m http.server 8000
# dann http://localhost:8000 öffnen
```

## Auf GitHub Pages veröffentliche

1. Es neus Repository uf GitHub erstelle (z. B. `staernae-bar`).
2. D'Dateie ufelade:

   ```bash
   cd staerne-bar
   git init
   git add index.html style.css README.md
   git commit -m "d'stärnä bar Website"
   git branch -M main
   git remote add origin https://github.com/<DIN-USERNAME>/staernae-bar.git
   git push -u origin main
   ```

3. Uf GitHub: **Settings → Pages**.
4. Bi **Source** → *Deploy from a branch*, Branch **`main`** / Ordner **`/ (root)`**, denn **Save**.
5. Nach churzer Ziit isch d'Site under
   `https://<DIN-USERNAME>.github.io/staernae-bar/` erreichbar.

## Aapasse

- **Sponsor-Link:** Im `index.html` isch dä Button uf `mailto:hallo@staernae-bar.ch`
  gsetzt — bitte dur d'richtigi E-Mail-Adrässe ersetze.
- **Farbe & Schrifte:** Ganz obe im `style.css` under `:root` (CSS-Variable).
