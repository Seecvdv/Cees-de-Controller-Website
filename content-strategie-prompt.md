# Claude Code prompt — één blogartikel publiceren

Herhaalbare prompt. Gebruik deze elke keer dat je een artikel uit `CONTENT.md` op de site
zet. Voorwaarde: het artikel staat klaar als markdown in `/content-input/<slug>.md`
met meta-titel, meta-beschrijving, categorie, eventueel header-afbeelding en de volledige
tekst.

---

## DE PROMPT

Je publiceert één nieuw blogartikel op de site van Cees de Controller.

### Context van de site

- Pure HTML, gehost op **GitHub Pages** met custom domein `ceesdecontroller.nl` (zie `CNAME`). Géén Netlify, géén build-tools, géén dependencies.
- Huisstijl staat al vast in elke pagina (inline `<style>`-block bovenaan). Achtergrond `#0c0d0c`, accent groen `#4a7c59`/`#5b9069`, fonts **Inter** en **JetBrains Mono**. Niet wijzigen, niet "verbeteren".
- De blog-sectie bestaat al: [blog/index.html](blog/index.html) met drie live artikelen (`controle-op-je-boekhouding.html`, `drie-signalen.html`, `controller-vs-boekhouder.html`). Het artikel-template heeft een sidebar met TOC, "Meer lezen" en een Calendly-CTA. Gebruik een bestaand artikel als sjabloon — niet vanaf nul bouwen.
- Calendly-link: `https://calendly.com/cees-ceesdecontroller/30min`.
- Lead magnet (checklist 7 signalen, `assets/checklist-7-signalen.pdf`) draait via **Web3Forms** en zit op de homepage. Niet aanpassen. Als een artikel om een eigen magnet vraagt: eerst overleggen, geen Netlify Forms gebruiken (werken niet op GitHub Pages).
- Redactiekalender en open beslissingen staan in [CONTENT.md](CONTENT.md).

### Werkwijze

1. **Verkennen.** Lees het aangeleverde markdown-bestand in `/content-input/` en open één bestaand artikel als referentie (bijvoorbeeld `blog/drie-signalen.html`). Vat in één alinea samen wat je gaat doen vóór je iets schrijft.
2. **Kopiëren.** Maak `blog/<slug>.html` door een bestaand artikel te dupliceren. Behoud `<nav>`, `<footer>`, mobile-menu, script-blok en het hele inline `<style>`-blok exact zoals daar.
3. **Head bijwerken.** In `<head>`: `<title>`, `<meta name="description">`, `<link rel="canonical" href="https://ceesdecontroller.nl/blog/<slug>.html">`, `og:title`, `og:description`, `og:url`. Gebruik de meta-titel en meta-beschrijving uit de markdown.
4. **Inhoud vervangen.** In `<article class="article-content">`:
   - `meta-cat`: `<categorie> · <leestijd> min lezen`. Leestijd berekenen op basis van woordental, 200 woorden per minuut, naar boven afgerond.
   - `<h1>`: artikeltitel.
   - Intro-alinea krijgt class `intro`.
   - Markdown `##` wordt `<h2 id="<kebab-slug>">`. Het `id` is nodig voor de sidebar-TOC.
   - Vetgedrukte labels blijven `<strong>`.
   - Citaten/voorbeelden uit het echte leven kunnen in een `<div class="callout">…</div>`.
   - Sluit af met het bestaande `article-cta`-blok (Calendly-knop).
5. **Sidebar bijwerken.** TOC: één `<li>` per `<h2>`-id. "Meer lezen": kies een ander artikel dat thematisch aansluit. Gratis-intake-blok ongewijzigd laten.
6. **Header-afbeelding.** Alleen als de markdown een afbeelding noemt en het bestand in de repo staat. Zo niet, beeldblok weglaten (zoals de huidige drie artikelen doen).
7. **Blog-index aanvullen.** Voeg een nieuwe `<a class="blog-row">…</a>` bovenaan de `.blog-list` in [blog/index.html](blog/index.html) toe — zelfde structuur als de bestaande rijen.
8. **Sitemap.** Voeg `<url>` toe aan [sitemap.xml](sitemap.xml) voor het nieuwe artikel.
9. **Stop en rapporteer.** Geen commit. Sluit af met: welke bestanden gewijzigd, welk handwerk er nog is (bijvoorbeeld afbeelding plaatsen, LinkedIn-versie posten).

### Stijl- en kwaliteitsregels

- Nederlands, je-vorm, B1-niveau. Korte alinea's, concrete getallen boven abstracte claims.
- Geen emoji's. Geen Amerikaanse verkooptaal, geen overdreven superlatieven, geen nep-urgentie.
- Titels in gewone zinsopbouw — geen hoofdletter per woord.
- Bestaande pagina's en teksten op de site niet aanraken, tenzij expliciet gevraagd.

### Wat je niet doet

- Geen frameworks, build-tools of dependencies introduceren.
- Geen Netlify Forms — die werken niet op GitHub Pages. Voor leadgeneratie alleen Web3Forms of Calendly.
- Geen huisstijl "verbeteren" of herontwerpen. Aansluiten op wat er is.
- Geen content verzinnen die niet in het markdown-bestand staat. Bij twijfel: stoppen en vragen.
- Geen `git commit` of `git push` zonder review.

---

## Per-artikel input

Verwacht in `/content-input/<slug>.md`:

```yaml
---
meta-titel: <titel-tag, max ~60 tekens>
meta-beschrijving: <max ~155 tekens>
categorie: <bijv. Controle & Grip / Reporting & Inzicht / AI in finance / Odoo>
header-afbeelding: <pad of leeg laten>
---

# <artikeltitel>

<intro-alinea>

## <eerste kop>

<inhoud>
```
