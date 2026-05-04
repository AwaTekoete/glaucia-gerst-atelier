# Gláucia Gerst · Atelier — Website

Offizielle Website der Aquarellkünstlerin Gláucia Gerst.

**Live URL:** https://glauciagerst-atelier.com

---

## Projektübersicht

Statische HTML-Website für ein Aquarell-Atelier mit Auftragsportraits für Tierbilder.
Dreisprachig (Deutsch / Englisch / Portugiesisch), mobiloptimiert, internationales Publikum (DE, EN, BR).

---

## Technologien

- **HTML / CSS / JavaScript** — reines Vanilla, kein Framework
- **Cloudflare Pages** — Hosting, automatisches Deploy via GitHub
- **Formspree** — Kontaktformular (Endpoint: mvzlklyk)
- **GitHub** — Versionskontrolle (Repo: AwaTekoete/glaucia-gerst-atelier)

---

## Projektstruktur
/
├── index.html          → Hauptseite (alle Inhalte)
├── translations.js     → Alle Texte in DE / EN / PT
├── assests/            → QR Code Instagram
├── images/
│   ├── about/          → Foto der Künstlerin
│   └── gallery/        → Alle Galeriebilder

---

## Workflow — Änderungen deployen

Jede Änderung wird so deployed:

```bash
git add .
git commit -m "kurze beschreibung der änderung"
git push
```

Cloudflare Pages deployt automatisch innerhalb von ~30 Sekunden.

---

## Wichtige Accounts

| Service | Account | Zweck |
|---|---|---|
| GitHub | AwaTekoete | Code-Verwaltung |
| Cloudflare | glauciagerst.atelier@gmail.com | Hosting + Domain |
| Formspree | glauciagerst.atelier@gmail.com | Kontaktformular |
| Domain | glauciagerst-atelier.com | Registriert bei Cloudflare |

---

## Galerie — Bilder hinzufügen

Neue Bilder in `images/gallery/` ablegen, dann in `index.html` im `galleryImages` Block eintragen:

```javascript
const galleryImages = {
  hund: [ 'images/gallery/DATEINAME.jpg', ... ],
  auftrag: [ 'images/gallery/DATEINAME.jpg', ... ],
  katze: [ 'images/gallery/DATEINAME.jpg', ... ]
};
```

---

## Mehrsprachigkeit — Texte ändern

Alle Texte sind in `translations.js` — dort DE / EN / PT separat bearbeiten.
Nach Änderung wie gewohnt pushen.

---

## Formspree — E-Mail Empfänger ändern

Bei Launch: in Formspree Dashboard (formspree.io) unter dem Konto
glauciagerst.atelier@gmail.com → Formular "Kontaktformular Atelier" → Settings → E-Mail anpassen.

---

## Nächste geplante Schritte

- [ ] Stripe-Konto einrichten für Zahlungsabwicklung