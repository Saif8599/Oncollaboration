# The Client - Website

Ontwerp en maak een website voor een opdrachtgever en bespreek het resultaat tijdens de Sprint Review.

De instructie van deze leertaak staan in de [INSTRUCTIONS](https://github.com/fdnd-task/the-client-website/blob/main/docs/INSTRUCTIONS.md)



## Inhoudsopgave Readme

  * [Beschrijving](#beschrijving)
  * [Functionaliteiten](#functionaliteiten)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
Voor deze opdracht hebben wij de taak gekregen om een website te bouwen die de samenwerking tussen dokters uit Nederland en Indonesië te versterken. Het platform richt zich specifiek op radiotherapeuten en biedt hen de mogelijkheid om digitale webinars en CT-scans te uploaden en te delen, waarbij er vragen gesteld kunnen worden en gezamenlijk kan worden gewerkt aan de ontwikkeling van bestralingsplannen.

De website bestaat uit een homepagina, webinarspagina, contouringspagina, en profielpagina, elk met een specifieke functie voor de gebruikers:

- **Homepagina:** Een overzicht van het platform en de laatste nieuwsberichten en updates.
- **Webinarspagina:** Een overzicht van beschikbare webinars met zoek- en filteropties. Gebruikers kunnen webinars uploaden en deelnemen aan live of opgenomen sessies.
- **Contouringspagina:** Gebruikers kunnen hier CT-scans uploaden en samenwerken om bestralingsgebieden te bepalen.
- **Profielpagina:** Gebruikers kunnen hun persoonlijke informatie beheren en hun professionele achtergrond bijwerken.

![image](https://github.com/user-attachments/assets/b5281fe5-2271-43ec-9f49-2a21767fafa4)

![image](https://github.com/user-attachments/assets/997c14ef-7c9c-4efd-a1f9-8efcb2db2dbc)

Webinar pagina : https://saif8599.github.io/Oncollaboration/pages/all-webinars.html

## Functionaliteiten:
- **Webinar- en artikelbeheer:** Gebruikers kunnen webinars en artikelen uploaden en organiseren. Het platform bevat een zoekfunctie en filters om de juiste content snel te vinden.
- **Chatfunctie:** Voor directe communicatie tussen teams is er een ingebouwde chatfunctie, waar vragen en antwoorden kunnen worden gedeeld.
- **Veilige CT-scan upload:** Scans kunnen veilig worden geüpload en gezamenlijk worden geanalyseerd.
- **Naslagwerk:** Een naslagwerk dat is georganiseerd op specifieke onderwerpen, zodat gebruikers snel toegang hebben tot relevante informatie.
- **Q&A-sectie:** Gebruikers kunnen vragen stellen aan experts in een Q&A-sectie, wat de samenwerking en kennisuitwisseling versterkt.
- **Transcript functie:** Het platform biedt een transcriptie van webinars, zodat gebruikers de inhoud later gemakkelijk kunnen teruglezen.

## Kenmerken

Voor het ontwikkelen van de website zijn de volgende technieken gebruikt:


**HTML5:** Gebruikt voor het structureren van de content en opbouw van de pagina's.

Voorbeelden van semantische elementen:

`<header>` voor de bovenkant van de pagina of sectie.

`<nav>` voor navigatie-elementen.

`<section>` voor secties van content zoals webinars of profielinformatie.

`<article>` voor afzonderlijke items zoals een webinar of artikel.

`<footer>` voor de voettekst van een pagina.

Deze aanpak maakt de website beter leesbaar voor zowel mensen als zoekmachines.


**CSS:** Voor de opmaak en styling van de website. Er is gebruikgemaakt van moderne CSS technieken zoals flexbox en grid voor lay-outbeheer.

**Responsive design:** Door gebruik van media queries is de website geoptimaliseerd voor verschillende schermformaten, zoals mobiele apparaten en desktop.
```css
nav a:first-child {
  display: none;

  @media (min-width: 600px) {
    display: inline; /*De eerste a element in nav word weergegeven (logo) vanaf 600px*/
  }
}
```


**Flexbox en Grid:** Flexbox wordt gebruikt voor het uitlijnen van elementen, en CSS Grid voor het maken van een overzichtelijke indeling van de webinars.
```css
.webinar-grid {
  display: grid;
  grid-template-columns: repeat(
    2,
    1fr
  ); /* Hierbij word er 2 kolommen gemaakt van 2 1fr's */
  gap: 15px;
  margin-bottom: 80px;
  @media (min-width: 600px) {
    grid-template-columns: repeat(
      4,
      1fr
    ); /* En vanaf 600px word er 4 kolommen gemaakt van 4 1fr's */
    gap: 20px;
    margin-bottom: 0px;
  }
}
```


Vaste en flexibele navigatiebalk: De navigatiebalk is vastgezet (sticky) en verandert dynamisch afhankelijk van het schermformaat.

```css
nav {
  position: fixed; /* Fixed zorgt ervoor dat de nav vastgezet word */
  width: 100%;
  background-color: #ffffff;
  bottom: 0;
  left: 0;

  @media (min-width: 600px) {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #6a0025;
    padding: 10px;
    position: fixed;
    top: 0;
    height: 40px;
  }
}
```


## Bronnen

- MDN Web Docs - Media Queries : 
https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries

- CSS-Tricks - A Complete Guide to Flexbox : 
https://css-tricks.com/snippets/css/a-guide-to-flexbox/

- W3Schools - CSS Layout - Fixed Position : 
https://www.w3schools.com/css/css_positioning.asp#:~:text=An%20element%20with%20position%3A%20fixed,would%20normally%20have%20been%20located.







## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
