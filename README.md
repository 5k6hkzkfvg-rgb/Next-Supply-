# Next Supply — Website

Statische Single-File-Website (Vertrieb & Steuersparmodell / Mitarbeiterverpflegung).
Alle Seiten laufen über eine einzige `index.html` (Hash-Routing), Bilder sind eingebettet.

## Dateien in diesem Ordner
- `index.html` — komplette Website (Start · Modell · Ablauf · Steuervorteil · Partner · Über uns · Kontakt)
- `CNAME` — Custom Domain für GitHub Pages (`next-supply.de`)
- `.nojekyll` — schaltet die Jekyll-Verarbeitung aus (reine statische Auslieferung)

## Upload / Deployment (GitHub Pages)
1. Diese drei Dateien ins **Repo-Root** pushen (Branch `main`).
2. GitHub → **Settings → Pages** → Source: `main` / `/(root)` → **Save**.
3. Unter **Custom domain** steht durch die `CNAME`-Datei bereits `next-supply.de`.
4. Beim Domain-Anbieter die **DNS-Einträge** setzen:
   - Apex `next-supply.de` → vier A-Records auf GitHub Pages:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - optional `www` → CNAME auf `<dein-github-user>.github.io`
5. Sobald das Zertifikat bereit ist: **„Enforce HTTPS"** aktivieren.

## Kontaktformular
Eingebettetes Tally-Formular (`tally.so/embed/aQXLpq`). Jede Anfrage landet automatisch
als Lead in Notion („Leads — Next Supply CRM").

## Hinweis
Die Steuer-Zahlen (Sachbezugswert/Essenszuschuss 2026, Beispielrechnung) vor dem Go-Live
einmal vom Steuerberater bestätigen lassen.
