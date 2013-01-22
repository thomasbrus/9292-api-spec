# Sessions/saved-locations

	GET https://api.9292.nl/0.1/sessions/:session_id/saved-locations
	POST https://api.9292.nl/0.1/sessions/:session_id/saved-locations

## Abstract

Met de `sessions/saved-locations`-resource kan een lijst van opgeslagen locaties
opgehaald worden.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **:session_id** | Bevat de sessie ID die is opgehaald bij het registreren of inloggen. |
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |
| **etag** | Bevat de laatste E-Tag, zodat alleen wijzigingen geretourneerd worden. (optioneel) |

## Body

Eventueel kan er een POST request aangeroepen worden, zodat er nieuwe locaties
opgeslagen kunnen worden.  
De body van dit request is versleuteld in JSON (alhoewel de `"Content-Type"`-
header wel is ingesteld op `"application/x-www-form-urlencoded"`).

| Naam | Omschrijving |
|-----:|:-------------|
| **etag** | Bevat een nieuwe E-Tag. |
| **savedLocationMutations** | Bevat een array van `savedLocationMutation` objecten. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **etag** | Bevat een nieuwe E-Tag. |
| **savedLocations** | Bevat een array van `savedLocation` objecten. |
