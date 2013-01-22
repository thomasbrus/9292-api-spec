# Locations

	GET https://api.9292.nl/0.1/locations

## Abstract
De `locations`-resource wordt opgehaald wanneer er een zoekopdracht wordt
aangeroepen. Het retourneert een lijst van locaties (stations, plaatsen, etc.)
die overeenkomen met de zoekopdracht (`q`).

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |
| **q** | Bevat de zoekopdracht. Bv. `"amsterd"`. (optioneel) |
| **latlong** | Bevat een combinatie van de latitude en longitude coördinaten (`52.*, 5.*`). (optioneel) |
| **includeStation** | Onbekend. Standaard = `false`. |
| **type** | Bevat een combinatie van `location type`s (`station,stop,poi`). Zie `types.md`. (optioneel) |
| **range** | Niet precies bekend, waarschijnlijk het bereik van de `latlong` parameter. (optioneel) |
| **rows** | Maximum aantal locations dat geretourneerd moet worden. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **locations** | Bevat een array van `location` objecten. |

## Voorbeeld

### Request

	GET /0.1/locations?lang=nl-NL&q=amsterdam HTTP/1.1
	Host: api.9292.nl

### Response

	{
	  "locations": [
		{
		  "id": "station-amsterdam-centraal",
		  "type": "station",
		  "stationId": "asd",
		  "stationType": "Station",
		  "name": "Amsterdam Centraal",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.378706,
			"long": 4.900489
		  },
		  "urls": {
			"nl-NL": "/station-amsterdam-centraal",
			"en-GB": "/en/station-amsterdam-centraal"
		  }
		},
		{
		  "id": "station-amsterdam-bijlmer-arena",
		  "type": "station",
		  "stationId": "asb",
		  "stationType": "Station",
		  "name": "Amsterdam Bijlmer ArenA",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.312011,
			"long": 4.947046
		  },
		  "urls": {
			"nl-NL": "/station-amsterdam-bijlmer-arena",
			"en-GB": "/en/station-amsterdam-bijlmer-arena"
		  }
		},
		{
		  "id": "station-amsterdam-sloterdijk",
		  "type": "station",
		  "stationId": "ass",
		  "stationType": "Station",
		  "name": "Amsterdam Sloterdijk",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.389133,
			"long": 4.837017
		  },
		  "urls": {
			"nl-NL": "/station-amsterdam-sloterdijk",
			"en-GB": "/en/station-amsterdam-sloterdijk"
		  }
		},
		{
		  "id": "station-amsterdam-amstel",
		  "type": "station",
		  "stationId": "asa",
		  "stationType": "Station",
		  "name": "Amsterdam Amstel",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.346689,
			"long": 4.917453
		  },
		  "urls": {
			"nl-NL": "/station-amsterdam-amstel",
			"en-GB": "/en/station-amsterdam-amstel"
		  }
		},
		{
		  "id": "station-amsterdam-lelylaan",
		  "type": "station",
		  "stationId": "asdl",
		  "stationType": "Station",
		  "name": "Amsterdam Lelylaan",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.358641,
			"long": 4.833901
		  },
		  "urls": {
			"nl-NL": "/station-amsterdam-lelylaan",
			"en-GB": "/en/station-amsterdam-lelylaan"
		  }
		},
		{
		  "id": "amsterdam",
		  "type": "place",
		  "name": "Amsterdam",
		  "regionCode": "NH",
		  "regionName": "Noord-Holland",
		  "showRegion": false,
		  "countryCode": "NL",
		  "countryName": "Nederland",
		  "showCountry": false,
		  "latLong": {
			"lat": 52.378706,
			"long": 4.900489
		  }
		},
		{
		  "id": "nieuw-amsterdam",
		  "type": "place",
		  "name": "Nieuw Amsterdam",
		  "regionCode": "DR",
		  "regionName": "Drenthe",
		  "showRegion": false,
		  "countryCode": "NL",
		  "countryName": "Nederland",
		  "showCountry": false,
		  "latLong": {
			"lat": 52.718426,
			"long": 6.84893
		  }
		},
		{
		  "id": "amsterdam/gemeentearchief-amsterdam",
		  "type": "poi",
		  "poiType": "Overig",
		  "name": "Gemeentearchief Amsterdam",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.364606,
			"long": 4.892158
		  }
		},
		{
		  "id": "amsterdam/amsterdams-historisch",
		  "type": "poi",
		  "poiType": "Museum",
		  "name": "Amsterdam Museum",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.369982,
			"long": 4.890233
		  }
		},
		{
		  "id": "amsterdam/rijksmuseum-amsterdam",
		  "type": "poi",
		  "poiType": "Museum",
		  "name": "Rijksmuseum Amsterdam",
		  "place": {
			"name": "Amsterdam",
			"regionCode": "NH",
			"regionName": "Noord-Holland",
			"showRegion": false,
			"countryCode": "NL",
			"countryName": "Nederland",
			"showCountry": false
		  },
		  "latLong": {
			"lat": 52.360103,
			"long": 4.883679
		  }
		}
	  ]
	}
