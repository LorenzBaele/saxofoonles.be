# saxofoonles.be

Eénpagina-website, alleen in het Nederlands. Gewone HTML, geen build nodig. Open `index.html` in je browser om de site lokaal te bekijken.

## Inhoud

- `index.html`: de hele pagina (stijl en het scriptje voor het formulier zitten erin)
- `images/`: de vier foto's
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

DNS bij de domeinregistrar:

- vier A-records voor `@` naar: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- een CNAME-record voor `www` naar `lorenzbaele.github.io`

## Google setup (October 2026)

### Google Business Profile
- Owner account: lorenzbaele.booking@gmail.com (verified ✔).
- Website: https://saxofoonles.be/
- Address: studio in Gent, shown publicly. When the studio moves, update it on Google as well as on the site.
- Services (custom): Saxofoonles 30 min (€30), Saxofoonles 60 min (€55), Saxofoonles voor kinderen 30min (€30), Saxofoonles voor kinderen 60min (€55). When the prices on the site change, change them here too.
- Saxophone rental is intentionally only on the website, not on Google.

### Google Search Console
- Domain property saxofoonles.be, owned by lorenzbaele.booking@gmail.com.
- Verified via a DNS TXT record (google-site-verification=...) in the Hoasted Zone Editor. Never delete this record.
- Indexing of https://saxofoonles.be requested on 8 October 2026. Check with: site:saxofoonles.be

### Trustpilot
- A business account exists but is not linked from the website on purpose. Reviews go to Google.

## Dingen die je later zelf aanpast

- Tekst en prijzen: gewoon in `index.html` zoeken en aanpassen.
- Verhuizing naar Sint-Lievens-Houtem: zoek op "Gent" (staat in de lessenkaart, in "Over mij" en in de contacttabel).
- De korte video voor in de lessen is nog niet toegevoegd.
