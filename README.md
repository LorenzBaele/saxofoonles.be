# saxofoonles.be

Eénpagina-website in het Nederlands, met een Engelse versie op `/en/`. Gewone HTML en CSS, geen build nodig. Open `index.html` in je browser om de site lokaal te bekijken.

## Inhoud

- `index.html`: de Nederlandse pagina (het scriptje voor het formulier zit erin)
- `en/index.html`: dezelfde pagina in het Engels. Verander je tekst, prijzen of aanbod op de ene pagina, doe het dan ook op de andere. De twee pagina's verwijzen naar elkaar (`hreflang`), zodat Google Engelstaligen de Engelse toont. Bovenaan staat een knopje NL/EN om te wisselen.
- `style.css`: de opmaak van alle pagina's, in het Nederlands en het Engels. Een aanpassing aan het ontwerp doe je hier, één keer voor beide talen.
- `privacy/index.html` en `en/privacy/index.html`: de privacyverklaring in beide talen, gelinkt onder het formulier en in de footer. Verander je iets aan het formulier, je adres of de diensten die je gebruikt (zoals Web3Forms), pas het in beide aan.
- `images/`: de foto's als WebP (kleiner dan JPEG, max. 2000 px breed) en `favicon.png` (192 px). `banner-lorenz.jpg` blijft als JPEG staan, want die toont WhatsApp, Facebook en Google als voorbeeldfoto. Een nieuwe foto? Zet hem om naar WebP (kwaliteit rond 75-80).
- `fonts/`: de lettertypes Barlow, Barlow Semi Condensed en Caveat (alleen de Latijnse tekens). Ze staan op de site zelf in plaats van bij Google Fonts: dat laadt sneller en er gaat geen IP-adres van je bezoekers naar Google.
- `favicon.ico`: het icoontje in de browsertab en naast de site in Google. Google pikt een nieuw icoon pas na enkele dagen tot weken op.
- `robots.txt` en `sitemap.xml`: voor Google. Pas `lastmod` in de sitemap aan als de inhoud flink verandert.
- `CNAME`: zegt aan GitHub Pages dat de site op saxofoonles.be draait
- `.nojekyll`: zorgt dat GitHub de bestanden ongewijzigd toont

## Contactformulier

GitHub Pages kan zelf geen e-mail sturen. Het formulier gebruikt daarom [Web3Forms](https://web3forms.com) (gratis). Berichten komen toe op het e-mailadres dat aan de access key gekoppeld is.

- De access key staat in `index.html` en `en/index.html`, in het verborgen veld `access_key`. Die sleutel mag publiek zijn: hij kan alleen berichten naar jouw adres sturen.
- Het onderwerp van de mail pas je aan in het verborgen veld `subject`. Berichten van de Engelse pagina hebben als onderwerp "Nieuw bericht via saxofoonles.be (Engels)", zodat je weet dat je in het Engels antwoordt.
- Na het versturen toont de pagina zelf een bedankt- of foutmelding, zonder naar een andere pagina te gaan.
- Een verborgen `botcheck`-vakje houdt de meeste spam tegen.
- Een ander ontvangstadres nodig? Maak op web3forms.com een nieuwe access key aan en vervang de oude in beide pagina's.

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
- **Gestructureerde gegevens**: `index.html` bevat een JSON-LD-blok (LocalBusiness) met naam, e-mail, het adres van de studio (precies zoals op het Google Bedrijfsprofiel, ook in de footer), de link naar het profiel op Google Maps, talen (Nederlands en Engels), de saxofoons en stijlen, de tarieven (ook voor kinderen) en de verhuur. `en/index.html` heeft hetzelfde blok in het Engels (zelfde `@id`, zonder de lijst met gemeenten). Pas de prijzen in beide aan als ze op de pagina veranderen. Testen met de Rich Results Test van Google.
- **Veelgestelde vragen** (sectie `#vragen`): beantwoordt in gewone zinnen wat mensen aan Google en aan AI-chatbots zoals ChatGPT vragen: prijs, kinderen, proefles, waar, online, welke saxofoons, stijlen, huren en lessen in het Engels. AI-zoekmachines citeren alleen wat letterlijk op de pagina staat, dus verandert je aanbod (of je prijzen), pas het hier ook aan.
- **Trustpilot**: er bestaat een bedrijfsaccount, maar dat staat bewust niet op de website. Reviews gaan naar Google.
- **Vorige eigenaar van het domein**: tot ongeveer september 2024 stond op saxofoonles.be de Wix-site van een andere saxofoonleraar. Daarom staat in Search Console nog een oude sitemap `https://www.saxofoonles.be/sitemap.xml` (sinds 2023, verwijst door naar de nieuwe sitemap en doet geen kwaad) en kunnen oude Wix-adressen als 404 opduiken. Niets aan doen. Gecontroleerd in oktober 2026: alleen Lorenz is eigenaar in Search Console.
