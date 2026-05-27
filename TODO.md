# TODO — Cees de Controller Website

Open items uit de strategische verbeterronde van 2026-05-21.

## Content nog aan te leveren

- **Testimonials (1–2 quotes).** Naam, functie, bedrijf, citaat. Plaats in `.testimonials` op `index.html` (HTML-structuur staat al klaar als placeholder-comment tussen `klanten` en `pills`-secties).
- **Mini-case (1 stuks).** Klant, situatie, aanpak, meetbaar resultaat. Format: korte alinea + 1 cijfer dat het verschil maakt. Plek: zelfde sectie als testimonials of als losse case-card.
- **Odoo-case (1 stuks).** Klant, fase (vóór/tijdens/na implementatie of herstel), aanpak, resultaat. Placeholder-structuur staat klaar als HTML-comment op `odoo.html`. Vervangt dat blok zodra geleverd.
- ~~**Lead-magnet PDF.**~~ Klaar — `assets/checklist-7-signalen.pdf` staat in de repo, source-files in `lead-magnet/`. Homepage-form geeft nu een directe downloadlink op de bevestigingspagina. Aanvragers landen nog steeds via Web3Forms in je inbox, dus je hebt de lead én ze hebben de PDF.

## Latere kandidaten

- **Checklist-download-flow opnieuw bekijken (na deploy).** Na de tekstreview van 2026-05-27 is signaal 5 in de checklist vervangen door een systeem/ERP-signaal en is Over Cees herschreven. De HTML/MD-bron is bijgewerkt, de PDF wordt door Cees handmatig per mail nagestuurd. Twee opties om weer in lijn te brengen: (1) nieuwe PDF in `assets/checklist-7-signalen.pdf` zetten zodat de directe downloadlink op de homepage weer klopt, of (2) op `index.html` de directe downloadlink in `#checklist-success` weghalen en het bericht aanpassen naar "Bedankt — je ontvangt de checklist binnen X uur per mail". Beslissen zodra de huidige push live staat.
- **Autoresponse per e-mail naar aanvragers** (zinvol zodra je structureel meer dan 1-2 PDF-aanvragen per week ziet). Web3Forms-autoresponder is een Pro-feature (~$8/mnd) — werkt point-and-click via hun dashboard, geen code-changes nodig. Goedkoper alternatief: webhook van Web3Forms naar een serverless function (Vercel/Netlify) die via Resend/Postmark/MailerSend een welkomstmail met PDF-link stuurt. In beide gevallen: success-bericht op homepage moet dan weer aangevuld worden met *"Je ontvangt 'm ook in je inbox"*.
- Webhook van Web3Forms naar Notion of Odoo CRM zodat lead-magnet aanvragen en contactformulier automatisch in één lijst landen — kan gecombineerd met bovenstaande autoresponder-flow in dezelfde serverless function.
- Daadwerkelijke testimonials/case-content verzamelen via klantvraag (e.g. Jeugdeducatiefonds, Humble Recruitment, Infinitas Learning).
- **Blogpost over Odoo + finance.** Onderwerp: *"Wat een Odoo-implementatiepartner finance-technisch vaak overslaat"*. Doel: longtail SEO-verkeer naar `/odoo.html`. Plek: `blog/odoo-implementatie-finance.html` (of vergelijkbare slug); ook toevoegen aan `blog/index.html` en `sitemap.xml`.
- **Tweede visual op odoo.html** (optioneel). Eerste foto staat ingebouwd. Een Odoo-screenshot of diagram implementatiepartner ↔ Cees ↔ klant zou het verhaal verder completeren — maar de pagina werkt nu al met één menselijke visual.
