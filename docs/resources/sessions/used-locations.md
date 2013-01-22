# Sessions/used-locations

	GET https://api.9292.nl/0.1/sessions/:session_id/used-locations

## Abstract

Met de `sessions/used-locations`-resource kan een lijst van laatst gebruikte
locaties opgehaald worden.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **:session_id** | Bevat de sessie ID die is opgehaald bij het registreren of inloggen. |
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |
| **etag** | Bevat de laatste E-Tag, zodat alleen wijzigingen geretourneerd worden. (optioneel) |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **etag** | Bevat een nieuwe E-Tag. |
| **usedLocations** | Bevat een array van **usedLocation** objecten. |
| **locations** | Bevat een array van **location** objecten. |
