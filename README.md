# 9292 API specificatie
Al sinds mei 2011 is 9292ov.nl bezig aan een API voor ontwikkelaars. Zou er het
najaar zijn. Kwam er niet. Nu zijn we twee jaar verder, en blijkt dat de API al
lang af is. Alleen nog niet gedocumenteerd.

De mobiele iPhone app van 9292ov.nl maakt er gebruik van. Het is daarom
eenvoudig te achterhalen welke URLs de app aanroept, ook al maakt deze gebruik
van https.

Voor het uitvogelen van de documentatie is geen reverse-engineering of hacken
vereist of toegepast. Alleen het uitgaande en inkomende internetverkeer is
bijgehouden en geanalyseerd.

## Uitleg over de structuur van de documentatie

1.  Algemene informatie vindt je in `docs/general.md`. Daar staat
	bijvoorbeeld beschreven naar welke host je moet verbinden, wat voor response
	je verwachten kunt, etc.
	
2.	In `docs/resources.md` vind je een lijst van de (tot nu toe bekende)
	resources, met een korte beschrijving van wat ze doen. De volledige
	informatie vind je daarna in `docs/resources/*.md`.

3.  In `docs/objects.md` vind je een lijst met de verschillende objecten die de
	API kan retourneren.

4.	In `docs/types.md` vind je een lijst met verschillende types (bv.
	station-types).

## Disclaimer

Hoewel het gaat om de officiële 9292 API, is dit niet de officiële API
documentatie, die is nog niet of nooit vrijgegeven. Ik ben dus ook niet
verantwoordelijk voor eventuele onvolkomenheden die in de documentatie zouden
kunnen staan.

Door het ontbreken van officiële API documentatie is ook onduidelijk welke
voorwaarden van toepassing zijn op het gebruik. Ga er daarom vanuit dat dit
een combinatie van de voorwaarden van de apps en site is (**vooral: commercieel
gebruik is niet toegestaan**).
