# The Client - Website

## Typografie & leesbaarheid

Hoe zorg je ervoor dat de teksten op je website goed leesbaar zijn?

### Goed leesbare teksten

Voor goed leesbare teksten gelden een aantal basis regels die je kan toepassen op je ontwerp: tekst is minimaal 16px groot, de regelafstand van langere teksten is 1,4 (140%) en de optimale lengte van de regels zijn 10-12 woorden.


### Font styling

Het is gebruikelijk om aan de `<html>` de basis font styling te definieren, zoals:  
- font-family
- font-size
- color

De `font-family` die je in de `html` zet, zal ook gelden voor de elementen die daarbinnen vallen (genest zijn), dat heet *inheritance*. Je hoeft daarom maar op 1 plek de `font-family` te zetten. De `font-size` wordt niet doorgegeven aan de elementen die genest zijn. Als je een andere font size nodig hebt voor een heading of paragraaf moet je per element de font size bepalen. 

#### Aanpak
Analyseer de font waardes uit het design dat je hebt gekregen in Figma, zoals `font-family`, `font-size` en kleuren. Zet de basis font styling op in het `html` element. Pas daarna voor de belangrijkste tekst, de belangrijke details en achtergrondinformatie de font styling aan zoals het in het aangeleverde ontwerp staat, zoals de `<h1>`, `<h2>`, `<h3>`,  `<p>`, `<a>` en/of `<button>`. Controleer in de browser met de *inspector* de font styling van alle tekst elementen.

Als je nog niet bekend bent met (basis) font styling in CSS lees dan het artikel [Fundamental text and font styling](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals), bekijk de voorbeelden en probeer het uit in je opdracht.

### Regellengte en regelafstand

> A column is easy to read if it's wide enough to accommodate an average of 10 words per line. - Josef Müller-Brockmann

De beroemde grafisch ontwerper Josef Müller-Brockman (1914–1996) heeft uitgangspunten voor goede typografie beschreven. Deze uitgangspunten gelden voor print, maar gelden ook voor het web. Ook Robert Bringhurst komt tot dezelfde uitgangspunten: een goede regellengte heeft 66 karakters, oftwel 10–12 woorden.

> Anything from 45 to 75 characters is widely regarded as a satisfactory line length for a single-column page set in a serifed text face in a text size. The 66-character line (counting both letters and spaces) is widely regarded as ideal. For multiple column work, a better average is 40 to 50 characters. - Robert Bringhurst 

#### Max-width
De regellengte kan je op verschillende manieren bepalen door een element een breedte te geven. Omdat een website het goed moet doen op allerlei schermen is het aan te bevelen de regellengte geen vaste waarde te geven, dan kan het zomaar gebeuren dat de teksten niet in een scherm passen. Een veel gebruikte manier is de kaders met teksten een maximale breedte geven. Met `max-width` zorg je ervoor dat de teksten op een smal scherm passen, maar niet te lang worden op brede schermen, zodat de teksten goed leesbaar blijven. 

#### Aanpak
Geef een paragraaf met tekst een maximale breedte met `max-width`. Gebruik pixels om niet meer dan 10–12 woorden op een regel te tonen. Test de code door de browser smaller en breder te maken. Hoeveel pixels mag een paragraaf worden voor een goede regellengte? Probeer hetzelfde eens met `min-width`, wat gebeurt er nu als je je code in de browser test?

Je kan de breedte van een tekst ook met `em` of bijvoorbeeld met `ch` _units_ bepalen. Probeer uit welke waardes je kan gebruiken om een goede regellengte te krijgen. Bv `max-width: 60ch` of `max-width: 20em`. Tel hoeveel woorden er maximaal op een regel staan. Experimenteer met hoeveel `em` en hoeveel `ch` je nodig hebt voor een goede regellengte.

### Bronnen

[Web Design is 95% Typography](https://web.archive.org/web/20191218153545/https://ia.net/topics/the-web-is-all-about-typography-period)

[How We Read](https://alistapart.com/article/how-we-read)

[The 100% Easy-2-Read Standard](https://web.archive.org/web/20200114014936/https://ia.net/topics/100e2r)

[Fundamental text and font styling @ MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

[Text and typography @ web.dev](https://web.dev/learn/css/typography)

[Typography for Developers @ CSS Tricks](https://css-tricks.com/typography-for-developers/)

[font-size @ MDN, met uitleg over EM](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
