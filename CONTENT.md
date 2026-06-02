# Contentplanning Cees de Controller — 8 weken

Intern werkdocument. Geen webpagina. Bijgewerkt 2026-05-28.

## Publicatiestatus

- **2026-05-28 (do):** ✅ Gepubliceerd — *"Je hebt een controller aangenomen. Je data is nog steeds een chaos."* — [blog/controller-aangenomen-data-chaos.html](blog/controller-aangenomen-data-chaos.html). Kick-off; verschuift de donderdag-rij van week 1 naar voren.
- **2026-06-02 (di):** ✅ Gepubliceerd — *"Claude als je financieel analist — wat werkt en wat niet"* — [blog/claude-als-financieel-analist.html](blog/claude-als-financieel-analist.html). Eerste post in nieuwe categorie *AI in finance*. Eigen lead magnet meegeleverd: *5 data-checks vóór je AI op je cijfers loslaat* (zie hieronder). **Actie Cees vóór live:** magnet [lead-magnet/ai-datachecks.html](lead-magnet/ai-datachecks.html) afdrukken naar PDF en opslaan als `assets/5-data-checks-ai-finance.pdf` (anders werkt de downloadlink in het artikel nog niet).

## Uitgangspunten

- **Mix per ~10 posts:** 50% MKB-herkenning, 30% praktische tips, 20% persoonlijk.
- **Posttijden LinkedIn:** dinsdag/woensdag/donderdag, 8–9u of 17–18u. Geen weekend.
- **Ritme:** LinkedIn-versie eerst, één à twee dagen later het volledige artikel op de site.
- **Reageren:** MKB-herkenningsposts altijd afsluiten met een concrete vraag. Binnen 24 uur op elke reactie reageren.
- **Tempo:** 1–2 publicaties per week. Niet alles in één keer — dat verzwakt zowel het LinkedIn-distributie-effect als het SEO-signaal naar Google.

## Kalender

Startdatum week 1: dinsdag 2 juni 2026.

| Wk | Datum di | Datum do | Thema | Type | Onderwerp |
|----|----------|----------|-------|------|-----------|
| 1 | — | 2026-05-28 | Controle & Grip | MKB | Je hebt een controller aangenomen. Je data is nog steeds een chaos. *(gepubliceerd)* |
| 1 | 2026-06-02 | — | AI in finance | AI-tip | Claude als je financieel analist — wat werkt en wat niet *(gepubliceerd)* |
| 2 | 2026-06-09 | — | AI in finance | Tip | 3 dingen die je vandaag in Excel kunt automatiseren (zonder VBA) |
| 3 | 2026-06-16 | — | Cashflow & sturen | MKB | Wanneer is een controller eigenlijk geldverspilling? |
| 3 | — | 2026-06-18 | Cashflow & sturen | Tip | Cashflow runway: wat het is en hoe je het zelf berekent |
| 4 | 2026-06-23 | — | Cashflow & sturen | Persoonlijk | "AI neemt mijn werk over" — met de nodige zelfspot |
| 4 | — | 2026-06-25 | AI in finance | Opinie | Waarom Claude wél met je agenda kan praten, maar niet met Exact — pleidooi voor MCP-koppelingen in NL-software |
| 5 | 2026-06-30 | — | Fractioneel & DBA | MKB | Waarom je misschien geen fulltime controller nodig hebt |
| 5 | — | 2026-07-02 | Fractioneel & DBA | Tip | DBA en ZZP-inhuur: het risico en hoe fractioneel dat oplost |
| 6 | 2026-07-07 | — | Odoo + finance | SEO | Wat een Odoo-implementatiepartner finance-technisch vaak overslaat |
| 6 | — | 2026-07-09 | Fractioneel & DBA | AI-tip | Power BI + AI: rapportages die zichzelf bijwerken |
| 7 | 2026-07-14 | — | Data & beslissen | MKB | Vijf mensen met vijf Excels: data-eigenaarschap in de praktijk |
| 8 | 2026-07-21 | — | Data & beslissen | Persoonlijk | Beschikbaarheid: wat ik doe en voor wie |

## Categorieën

De site gebruikt nu drie categorieën: *Controle & Grip*, *Reporting & Inzicht*, *Fractioneel controller*. De thema's uit de kalender mappen daarop als volgt:

- **AI in finance** → nieuwe categorie *AI in finance* (toevoegen op blog/index.html).
- **Cashflow & sturen** → *Controle & Grip*.
- **Fractioneel & DBA** → *Fractioneel controller*.
- **Odoo + finance** → *Odoo* (nieuwe categorie; sluit aan op odoo.html).
- **Data & beslissen** → *Reporting & Inzicht*.

## Open beslissingen vóór publicatie

- **"Power BI + AI" en "Excel zonder VBA":** passen die nog bij de huidige positionering (fractioneel / Odoo / cashflow)? Of zijn dat resten van een bredere strategie? Beslissen vóór week 2.
- **"AI neemt mijn werk over" (persoonlijk):** toon afstemmen — zelfspot werkt alleen als de rest van de site al een serieuze toon heeft. Vóór week 4 een ruwe versie schrijven en toetsen.
- ~~**Lead magnet onder AI-artikel (week 1):**~~ ✅ Beslist (2026-06-02): optie (a) gekozen — tweede magnet *"5 data-checks vóór je AI op je cijfers loslaat"* gemaakt ([lead-magnet/ai-datachecks.html](lead-magnet/ai-datachecks.html) + `.md`). Ingebouwd als Web3Forms-formulier in het artikel. Restactie: HTML afdrukken naar `assets/5-data-checks-ai-finance.pdf`.
- ~~**Nieuwe categorie *AI in finance*:**~~ ✅ Toegevoegd als `meta-cat`-label op [blog/index.html](blog/index.html) (de blogindex heeft geen aparte categoriefilter; categorie = label per rij).

## Inhoudelijke notitie bij de MCP-post (week 4 do)

**Onderwerp:** Nederlandse zakelijke software (Exact, AFAS, Twinfield, Yuki, Visma) biedt zelf nauwelijks MCP-koppelingen aan. Er zijn wel **third-party MCP-servers** die op deze API's bouwen, maar dat is niet hetzelfde als een officiële koppeling van de leverancier. Moneybird is de uitzondering: zelf een MCP-server beschikbaar, sinds kort.

**Hoek:** geen technisch artikel, maar een opiniestuk vanuit het perspectief van een fractioneel controller die *dagelijks* tussen Claude en meerdere Nederlandse systemen werkt. Twee concrete observaties:
1. Vergelijking: "Ik kan Claude vragen wat er morgen in mijn agenda staat. Vragen wat er vorige maand omgezet is in Exact? Dan val ik terug op een third-party MCP-server of een CSV-export."
2. **Het kernpunt:** voor finance-data wil je géén onbekende derde partij tussen jou en je administratie. Een officiële MCP van de leverancier — met heldere OAuth-scopes, audit-logs en SLA's — is geen luxe maar een randvoorwaarde voor serieuze AI-inzet op vertrouwelijke cijfers.

**Doel:** positionering als finance-pro die AI niet als hype ziet, maar ook de risico-kant ziet die een gemiddelde IT-pro of marketeer mist. Indirect signaal naar softwareleveranciers (kom op) én naar klanten (AI in finance is concreet, niet vaag).

**Eerlijk te noemen in het stuk:**
- Moneybird loopt voor met een eigen MCP-server.
- Third-party MCP-servers bestaan en zijn nuttig voor experimenteren — maar voor productie met vertrouwelijke data moet de leverancier zelf eigenaarschap nemen.
- Wat een first-party MCP minimaal zou moeten regelen: scoped tokens (alleen-lezen voor analyse, schrijven apart), audit-trail per AI-call, helder dataverwerkingsbeleid.

## Bestaande artikelen (referentie)

Staan al live, niet opnieuw publiceren:

- [Controle op je boekhouding](blog/controle-op-je-boekhouding.html) — Controle & Grip, 7 min
- [Drie signalen dat je cijfers je bedrijf remmen](blog/drie-signalen.html) — Reporting & Inzicht, 4 min
- [Controller, boekhouder of accountant: wie heb jij nodig?](blog/controller-vs-boekhouder.html) — Fractioneel controller, 7 min
