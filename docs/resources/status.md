# Status

	GET https://api.9292.nl/0.1/status

## Abstract
De `status`-resource wordt elke keer dat de mobiele app opstart, aangeroepen.
Met het antwoord kan bepaald worden in welke range aan data (bv. max 1 maand
van tevoren) een reis gepland kan worden. Ook retourneert dit commando de
laatste versie van de mobiele app, waarschijnlijk om de gebruiker er op te
attenderen dat er een update beschikbaar is.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **dateRange** | Bevat een `dateRange` object. |
| **version** | Bevat het versie nummer van de laatste app-uitgave. |

## Voorbeeld

### Request

	GET /0.1/status?lang=nl-NL HTTP/1.1
	Host: api.9292.nl

### Response

	{
		"dateRange": {
			"from": "2013-01-14",
			"to": "2013-02-24"
		},
		"version": "0.1.15.0"
	}
