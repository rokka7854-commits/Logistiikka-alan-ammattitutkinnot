# Logistiikka-alan ammattitutkinnot

Näytön arviointityökalu LogPT-sovelluksen käyttöliittymällä. Sisältää Word-rajauksen mukaiset 26 tutkinnon osaa neljässä osaamisalassa: varastologistiikka, kuljetusalan työnjohto, tavarakuljetukset ja henkilökuljetukset.

Arviointikohdat merkitään hyväksytyiksi tai hylätyiksi tai jätetään tyhjiksi. Hyväksyttyjen prosenttiosuus lasketaan kaikista tutkinnon osan arviointikohdista. Tyhjät kohdat vaativat yhteisen kirjallisen täydennyksen tutkinnon osalle, hylätyt kohdat oman perustelunsa. Tutkinnon osan loppuarvion antaa arvioija erikseen. Tyhjä loppuarvio näkyy PDF:ssä keskeneräisenä arviointina. Pelkkä perustelu ei muuta hylättyä kohtaa hyväksytyksi.

Sovellus tallentaa tiedot tämän laitteen selaimeen automaattisesti. Muutokset arvioihin, perusteluihin tai näytön tietoihin tyhjentävät allekirjoitukset. Arviointimerkinnän tai täydennyksen muuttaminen tyhjentää myös kyseisen osan loppuarvion. Sovelluksen linkin jakaminen jakaa vain sovelluksen osoitteen. Arviointitiedot jaetaan PDF-raporttina. PDF-jako käyttää laitteen jakotoimintoa; jos se ei tue tiedostoja, PDF ladataan ja jaetaan laitteen tiedostoista.

PWA voidaan asentaa puhelimelle. Ensimmäisen verkkokäynnin jälkeen sovellus toimii myös ilman verkkoyhteyttä. Selaintietojen poistaminen poistaa myös paikalliset arviot.

## Käyttö

1. Avaa sovellus, kirjaa näytön perustiedot ja valitse osaamisala.
2. Valitse tämän näytön tutkinnon osat.
3. Merkitse arviot ja lisää huomiot sekä tarvittavat hylkäysperustelut.
4. Siirry yhteenvetoon. Täytä puuttuvat arviot tai kirjoita yhteinen täydennys kullekin tutkinnon osalle.
5. Valitse loppuarviot, allekirjoita ja tallenna tai jaa PDF.
6. Tallenna raportti ennen kuin päätät näytön ja tyhjennät tiedot.

Älä kirjaa sovellukseen näytön suorittajan nimeä, henkilötunnusta, terveystietoja tai muita arkaluontoisia tietoja. Käytä näytön tunnistetta.

## Aineisto

- Palvelulogistiikan ammattitutkinto, OPH-1135-2025, voimaantulo 1.8.2025.
- Kuljetusalan ammattitutkinto, OPH-5799-2025, voimaantulo 1.1.2026.
- Käyttäjän toimittama Tutkinnot ja tutkinnon osat.docx rajaa osaamisalat ja osat.

24 tutkinnon osassa arviointikohdat on poimittu toimitettujen perusteiden hyväksytyn suorituksen kriteereistä. Ammattipätevyys ja ammattipätevyyden laajennus näytetään suorituksen toteamisena. Työkalu ei korvaa niiden erillistä koulutus- ja koemenettelyä. data.js säilyttää kriteerien lähdesivut ja ryhmäotsikot. Perusteiden mahdolliset toistuvat kriteerit on säilytetty.

## Julkaiseminen

Staattinen sovellus ilman palvelinta tai rakennusvaihetta. GitHub Pages: Settings → Pages → Deploy from a branch → main / root. Sovellus avautuu index.html-tiedostosta.

Paikallinen testaus: `python -m http.server 8000` tässä kansiossa, sitten `http://localhost:8000`. PWA tarvitsee HTTPS-yhteyden tai localhostin.

PDF-kirjasto: jsPDF 2.5.1, MIT-lisenssi (lisenssiteksti kirjastotiedostossa).
