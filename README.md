# saxofoonles.be

Eénpagina-website, alleen in het Nederlands. Gewone HTML, geen build nodig. Open `index.html` in je browser om de site lokaal te bekijken.

## Inhoud

- `index.html`: de hele pagina (stijl en het scriptje voor het formulier zitten erin)
- `images/`: de foto's (gecomprimeerd, max. 2000 px breed) en `favicon.png` (192 px)
- `favicon.ico`: het icoontje in de browsertab en naast de site in Google. Google pikt een nieuw icoon pas na enkele dagen tot weken op.
- `robots.txt` en `sitemap.xml`: voor Google. Pas `lastmod` in de sitemap aan als de inhoud flink verandert.
- `CNAME`: zegt aan GitHub Pages dat de site op saxofoonles.be draait
- `.nojekyll`: zorgt dat GitHub de bestanden ongewijzigd toont

## Contactformulier

GitHub Pages kan zelf geen e-mail sturen. Het formulier gebruikt daarom [Web3Forms](https://web3forms.com) (gratis). Berichten komen toe op het e-mailadres dat aan de access key gekoppeld is.

- De access key staat in `index.html`, in het verborgen veld `access_key`. Die sleutel mag publiek zijn: hij kan alleen berichten naar jouw adres sturen.
- Het onderwerp van de mail pas je aan in het verborgen veld `subject`.
- Na het versturen toont de pagina zelf een bedankt- of foutmelding, zonder naar een andere pagina te gaan.
- Een verborgen `botcheck`-vakje houdt de meeste spam tegen.
- Een ander ontvangstadres nodig? Maak op web3forms.com een nieuwe access key aan en vervang de oude in `index.html`.

## Online zetten

De site draait via GitHub Pages vanuit de repository [LorenzBaele/saxofoonles.be](https://github.com/LorenzBaele/saxofoonles.be), branch `main`, map `/ (root)`. Alles wat naar `main` gepusht wordt, staat na een minuutje live op saxofoonles.be.

Instellingen (Settings, Pages): Source "Deploy from a branch", custom domain `saxofoonles.be`, "Enforce HTTPS" aan.

DNS bij de domeinregistrar (Hoasted, Zone Editor):

- vier A-records voor `@` naar: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- een CNAME-record voor `www` naar `lorenzbaele.github.io`
- een TXT-record `google-site-verification=...` voor Google Search Console. Nooit verwijderen.

## Google (ingesteld in oktober 2026)

Alles staat op het account lorenzbaele.booking@gmail.com.

- **Google Bedrijfsprofiel** (geverifieerd): website https://saxofoonles.be/, adres van de studio in Gent (publiek zichtbaar). Diensten: Saxofoonles 30 min (€30), Saxofoonles 60 min (€55), Saxofoonles voor kinderen 30 min (€30) en Saxofoonles voor kinderen 60 min (€55). Saxofoonverhuur staat bewust alleen op de website, niet op Google.
- **Google Search Console**: domeineigendom saxofoonles.be, geverifieerd via het TXT-record hierboven. De homepage is geïndexeerd sinds oktober 2026. Sitemap: https://saxofoonles.be/sitemap.xml.
- **Gestructureerde gegevens**: `index.html` bevat een JSON-LD-blok (LocalBusiness) met naam, e-mail, Gent en de tarieven. Pas de prijzen daar ook aan als ze op de pagina veranderen. Testen met de Rich Results Test van Google.
- **Trustpilot**: er bestaat een bedrijfsaccount, maar dat staat bewust niet op de website. Reviews gaan naar Google.
- **Vorige eigenaar van het domein**: tot ongeveer september 2024 stond op saxofoonles.be de Wix-site van een andere saxofoonleraar. Daarom staat in Search Console nog een oude sitemap `https://www.saxofoonles.be/sitemap.xml` (sinds 2023, verwijst door naar de nieuwe sitemap en doet geen kwaad) en kunnen oude Wix-adressen als 404 opduiken. Niets aan doen. Gecontroleerd in oktober 2026: alleen Lorenz is eigenaar in Search Console.
