# Locations/departure-times

	GET https://api.9292.nl/0.1/locations/:location_id/departure-times

## Abstract
Met de `locations/departure-times`-resource kun je de vertrektijden van treinen
en bussen vanaf de gespecificeerde locatie ophalen.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **:location_id** | Bevat het `id` van de `location` waar je de vertrektijden van wil ophalen. |
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **location** | Bevat een `location` object. |
| **tabs** | Bevat een array van `tab` objecten. |

## Voorbeeld

### Request

	GET /0.1/station-amsterdam-centraal/departure-times?lang=nl-NL
	Host: api.9292.nl

### Response

	{}
