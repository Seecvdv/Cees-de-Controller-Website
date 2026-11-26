# Cees de Controller: website v2 (2027)

Nieuwe versie van de site, naast de huidige. De live site in de hoofdmap is niet aangepast.

## Wat is er anders

- Licht palet (gebroken wit, donkergroen, oker) in plaats van dark mode.
- Koppen in Fraunces (serif), lopende tekst in Inter. JetBrains Mono is eruit.
- Geen labels met streepje, pillen, bolletjes, pijltjes of kaarten meer.
- Eén gedeelde stylesheet: `assets/site.css`. Geen `<style>`-blok per pagina meer.
- Teksten van home, diensten, over, odoo en contact zijn herschreven. Blogs en de vergelijking zijn overgezet met dezelfde tekst, zonder gedachtestreepjes.
- Formulieren (checklist, contact, AI-zelfcheck) gebruiken één gedeeld script via `data-web3`.

## Bekijken

Open `index.html` in deze map met een dubbelklik. Alle links zijn relatief, dus het werkt lokaal en onder `/v2/`.
Alleen `404.html` gebruikt absolute paden (`/assets/...`). Die ziet er pas goed uit als hij in de hoofdmap staat.

## Livegang (checklist)

1. In alle `.html`-bestanden de regel `<meta name="robots" content="noindex, nofollow" />` en het commentaar erboven weghalen.
2. Inhoud van `v2/` naar de hoofdmap verplaatsen en de oude bestanden overschrijven.
3. Bestanden in de hoofdmap die niet in v2 zitten, laten staan: `CNAME`, `robots.txt`, `sitemap.xml`, `site.webmanifest`, de doorverwijzingen (`contact/`, `gratis-intake/`, `cookiebeleid-eu/`, `privacy-statement-privacyverklaring/`, `blog/controller-vs-boekhouder-vs-accountant.html`) en `lead-magnet/`.
4. `site.webmanifest`: `background_color` en `theme_color` op `#f3efe6` zetten.
5. Links naar `index.html` en `blog/index.html` werken ook op Netlify. Wil je mooie URL's (`/` en `/blog/`), vervang ze dan na de verhuizing.
6. `og-image.png` is nog de donkere versie. Maak een nieuwe in de lichte stijl.
7. `proef-homepage.html` in de hoofdmap kan weg.

## Nog te checken of aan te vullen

- Twee keuzes: een financiële opdracht of de Grip-scan. Maandelijkse inzet kan binnen een opdracht worden afgesproken.
- Grip-scan: € 499 excl. btw, 90 minuten op locatie, één A4 en 30 minuten nabespreking. Komt er uit de scan een project dat ik voor je uitvoer? Dan trek ik de volledige € 499 af van de projectfactuur. Intern tijdsbudget: streef naar vier uur inclusief reistijd, maximaal vijf uur.
- **Naam quickscan.** De werktitel is "Grip-scan". Andere naam? Zoek in de hele v2-map op `Grip-scan` en vervang overal (ook in title, meta, JSON-LD en de footer van alle pagina's). De bestandsnaam `quickscan.html` en de link `contact.html?onderwerp=quickscan` blijven hetzelfde.
- **PDF van de checklist** (`assets/checklist-7-signalen.pdf`) is nog de oude tekst. Maak hem opnieuw vanuit `lead-magnet/checklist.html`.
- **Odoo Accounting Partner** staat op home, odoo en over. Klopt dat nog?
- **"Ik reageer binnen één werkdag"** staat op de contactpagina. Haal het weg als je dat niet wilt beloven.
- **Voorbeelden in blogs** (zoals €40.000, €75 naar €95 per uur, €100.000 omzet in "Drie signalen"). Zijn dit echte klantsituaties? Zo niet, weghalen of vervangen.
- **Tijdlijn op Over**: de volgorde (webshop, VU, PwC, KPMG, controller, nu) en de omschrijvingen per stap.
- **Testimonials en een klantcase** ontbreken nog. Die helpen het meest om de site menselijk te maken.
- **Foto's**: er zijn er nu drie, allemaal in zwart-wit via CSS. Nieuwe foto's (aan het werk, bij een klant, Utrecht) maken het sterker.
