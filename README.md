# saxofoonles.be

Eénpagina-website, alleen in het Nederlands. Gewone HTML, geen build nodig.

## Inhoud

- `index.html`: de hele pagina (stijl zit erin)
- `images/`: de vier foto's
- `CNAME`: zegt aan GitHub Pages dat de site op saxofoonles.be draait
- `.nojekyll`: zorgt dat GitHub de bestanden ongewijzigd toont

## 1. Contactformulier laten mailen

GitHub Pages kan zelf geen e-mail sturen. Het formulier gebruikt daarom Formspree (gratis tot 50 berichten per maand).

1. Maak een account op formspree.io en maak een nieuw formulier aan met jouw e-mailadres.
2. Kopieer de formulier-ID (iets als `xqkrwpab`).
3. Open `index.html` en zoek `VERVANG_DIT_DOOR_JE_FORMULIER_ID`. Vervang dat door jouw ID.
4. Bij het eerste bericht stuurt Formspree een bevestigingsmail. Bevestig die één keer.

## 2. Online zetten met GitHub Pages

1. Maak op GitHub een nieuwe repository, bijvoorbeeld `saxofoonles`.
2. Upload alle bestanden uit deze map (ook `images/`, `CNAME` en `.nojekyll`).
3. Ga naar Settings, Pages. Kies bij Source "Deploy from a branch", branch `main`, map `/ (root)`.
4. Na een minuut staat de site op `jouwnaam.github.io/saxofoonles`.

## 3. Het domein saxofoonles.be koppelen

Stel bij je domeinregistrar deze DNS-records in:

- vier A-records voor `@` naar: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- een CNAME-record voor `www` naar `jouwnaam.github.io`

Vul daarna bij Settings, Pages, "Custom domain" `saxofoonles.be` in en zet "Enforce HTTPS" aan. Het kan enkele uren duren voor dit werkt.

## Dingen die je later zelf aanpast

- Tekst en prijzen: gewoon in `index.html` zoeken en aanpassen.
- Verhuizing naar Sint-Lievens-Houtem: zoek op "Gent" (staat in de lessenkaart, in "Over mij" en in de contacttabel).
- De korte video voor in de lessen is nog niet toegevoegd.
