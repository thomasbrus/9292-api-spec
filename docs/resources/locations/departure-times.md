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

    GET /0.1/locations/station-amsterdam-centraal/departure-times?lang=nl-NL
    Host: api.9292.nl

### Response

    {
      "location": {
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
      "tabs": [
        {
          "id": "trein",
          "name": "Trein",
          "locations": [
            {
              "id": "station-amsterdam-centraal",
              "type": "stop",
              "stopType": "Station",
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
            }
          ],
          "departures": [
            {
              "time": "02:18",
              "destinationName": "Utrecht Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "late",
              "realtimeText": "+8 min."
            },
            {
              "time": "02:45",
              "destinationName": "Rotterdam Centraal",
              "viaNames": "Schiphol, Leiden C., Den Haag HS",
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:17",
              "destinationName": "Utrecht Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:45",
              "destinationName": "Rotterdam Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:17",
              "destinationName": "Utrecht Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:45",
              "destinationName": "Rotterdam Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:14",
              "destinationName": "Den Haag Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "11a",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:17",
              "destinationName": "Alkmaar",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "7a",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:17",
              "destinationName": "Utrecht Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "8b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:25",
              "destinationName": "Amsterdam Bijlmer ArenA",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "5b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:27",
              "destinationName": "Den Haag Centraal",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "2a",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:29",
              "destinationName": "Vlissingen",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Intercity"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "13a",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:40",
              "destinationName": "Zwolle",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "5b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:44",
              "destinationName": "Hoofddorp",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "13b",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:47",
              "destinationName": "Alkmaar",
              "viaNames": null,
              "mode": {
                "type": "train",
                "name": "Sprinter"
              },
              "operatorName": "NS",
              "service": null,
              "platform": "7a",
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            }
          ]
        },
        {
          "id": "bus",
          "name": "Bus",
          "locations": [
            {
              "id": "amsterdam/bushalte-cs-ijsei",
              "type": "stop",
              "stopType": "Bushalte",
              "name": "CS IJzijde",
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
                "lat": 52.38016,
                "long": 4.899871
              },
              "urls": {
                "nl-NL": "/amsterdam/bushalte-cs-ijsei",
                "en-GB": "/en/amsterdam/bushalte-cs-ijsei"
              }
            },
            {
              "id": "amsterdam/bushalte-cs-centrum-pr-hendrikkade",
              "type": "stop",
              "stopType": "Bushalte",
              "name": "CS Prins Hendrikplantsoen",
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
                "lat": 52.377688,
                "long": 4.897725
              },
              "urls": {
                "nl-NL": "/amsterdam/bushalte-cs-centrum-pr-hendrikkade",
                "en-GB": "/en/amsterdam/bushalte-cs-centrum-pr-hendrikkade"
              }
            },
            {
              "id": "amsterdam/bushalte-cs-bus-oost",
              "type": "stop",
              "stopType": "Bushalte",
              "name": "CS Bus Oost",
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
                "lat": 52.377524,
                "long": 4.901589
              },
              "urls": {
                "nl-NL": "/amsterdam/bushalte-cs-bus-oost",
                "en-GB": "/en/amsterdam/bushalte-cs-bus-oost"
              }
            },
            {
              "id": "amsterdam/bushalte-cs-kamperbrug",
              "type": "stop",
              "stopType": "Bushalte",
              "name": "CS Kamperbrug",
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
                "lat": 52.377113,
                "long": 4.902019
              },
              "urls": {
                "nl-NL": "/amsterdam/bushalte-cs-kamperbrug",
                "en-GB": "/en/amsterdam/bushalte-cs-kamperbrug"
              }
            },
            {
              "id": "amsterdam/bushalte-cs-nicolaaskerk",
              "type": "stop",
              "stopType": "Bushalte",
              "name": "CS/Nicolaaskerk",
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
                "lat": 52.376810999999996,
                "long": 4.900818
              },
              "urls": {
                "nl-NL": "/amsterdam/bushalte-cs-nicolaaskerk",
                "en-GB": "/en/amsterdam/bushalte-cs-nicolaaskerk"
              }
            }
          ],
          "departures": [
            {
              "time": "02:10",
              "destinationName": "Geuzenveld",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "352",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:11",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "355",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:12",
              "destinationName": "Purmerend",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "EBS",
              "service": "N01",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:12",
              "destinationName": "Hoorn NH",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "EBS",
              "service": "N14",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:20",
              "destinationName": "A'veen Waardhuizen",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "354",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:24",
              "destinationName": "Molenwijk",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "363",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:35",
              "destinationName": "Badhoevedorp",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "358",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:41",
              "destinationName": "Bijlmermeer",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "357",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:47",
              "destinationName": "IJburg",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "359",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:49",
              "destinationName": "Osdorp De Aker",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "353",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:54",
              "destinationName": "Banne Buiksloot",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "361",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:58",
              "destinationName": "Stat.Sloterdijk",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "348",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:10",
              "destinationName": "Geuzenveld",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "352",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:11",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "GVB",
              "service": "355",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:12",
              "destinationName": "Purmerend",
              "viaNames": null,
              "mode": {
                "type": "bus",
                "name": "Nachtbus"
              },
              "operatorName": "EBS",
              "service": "N01",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            }
          ]
        },
        {
          "id": "tram",
          "name": "Tram",
          "locations": [
            {
              "id": "amsterdam/bus-tramhalte-cs-tram-westzijde",
              "type": "stop",
              "stopType": "Tramhalte",
              "name": "CS Tram Westzijde",
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
                "lat": 52.378179,
                "long": 4.89907
              },
              "urls": {
                "nl-NL": "/amsterdam/bus-tramhalte-cs-tram-westzijde",
                "en-GB": "/en/amsterdam/bus-tramhalte-cs-tram-westzijde"
              }
            },
            {
              "id": "amsterdam/tramhalte-cs-tram-oostzijde",
              "type": "stop",
              "stopType": "Tramhalte",
              "name": "CS Tram Oostzijde",
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
                "lat": 52.377783,
                "long": 4.901131
              },
              "urls": {
                "nl-NL": "/amsterdam/tramhalte-cs-tram-oostzijde",
                "en-GB": "/en/amsterdam/tramhalte-cs-tram-oostzijde"
              }
            }
          ],
          "departures": [
            {
              "time": "05:54",
              "destinationName": "VU medisch centrum",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "24",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:56",
              "destinationName": "Osdorp Dijkgraafplein",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "17",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:57",
              "destinationName": "A'veen Binnenhof",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "5",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "05:58",
              "destinationName": "Osdorp De Aker",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "1",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:00",
              "destinationName": "IJburg",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "26",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:02",
              "destinationName": "VU medisch centrum",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "16",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:06",
              "destinationName": "Osdorp Dijkgraafplein",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "17",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:08",
              "destinationName": "Osdorp De Aker",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "1",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:09",
              "destinationName": "VU medisch centrum",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "24",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:10",
              "destinationName": "IJburg",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "26",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:12",
              "destinationName": "A'veen Binnenhof",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "5",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:13",
              "destinationName": "Geuzenveld",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "13",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:16",
              "destinationName": "Osdorp Dijkgraafplein",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "17",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:17",
              "destinationName": "VU medisch centrum",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "16",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:18",
              "destinationName": "Osdorp De Aker",
              "viaNames": null,
              "mode": {
                "type": "tram",
                "name": "Tram"
              },
              "operatorName": "GVB",
              "service": "1",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            }
          ]
        },
        {
          "id": "metro",
          "name": "Metro",
          "locations": [
            {
              "id": "amsterdam/metrostation-centraal-station",
              "type": "stop",
              "stopType": "Metrostation",
              "name": "Centraal Station",
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
                "lat": 52.378291,
                "long": 4.900127
              },
              "urls": {
                "nl-NL": "/amsterdam/metrostation-centraal-station",
                "en-GB": "/en/amsterdam/metrostation-centraal-station"
              }
            }
          ],
          "departures": [
            {
              "time": "06:14",
              "destinationName": "Westwijk",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "51",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:15",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:22",
              "destinationName": "Gaasperplas",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "53",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:25",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:29",
              "destinationName": "Westwijk",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "51",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:32",
              "destinationName": "Gaasperplas",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "53",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:36",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:39",
              "destinationName": "Westwijk",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "51",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:43",
              "destinationName": "Gaasperplas",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "53",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:45",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:48",
              "destinationName": "Westwijk",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "51",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:51",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:52",
              "destinationName": "Gaasperplas",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "53",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:56",
              "destinationName": "Westwijk",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "51",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "06:58",
              "destinationName": "Gein",
              "viaNames": null,
              "mode": {
                "type": "subway",
                "name": "Metro"
              },
              "operatorName": "GVB",
              "service": "54",
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            }
          ]
        },
        {
          "id": "veerboot",
          "name": "Veerboot",
          "locations": [
            {
              "id": "amsterdam/halte-veer-de-ruyterkade",
              "type": "stop",
              "stopType": "Halte",
              "name": "Veer Centraal Station",
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
                "lat": 52.380697,
                "long": 4.89941
              },
              "urls": {
                "nl-NL": "/amsterdam/halte-veer-de-ruyterkade",
                "en-GB": "/en/amsterdam/halte-veer-de-ruyterkade"
              }
            }
          ],
          "departures": [
            {
              "time": "02:06",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:18",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:30",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:42",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "02:54",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:06",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:18",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:30",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:42",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "03:54",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:06",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:18",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:30",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:42",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            },
            {
              "time": "04:54",
              "destinationName": "Buiksloterwegveer",
              "viaNames": null,
              "mode": {
                "type": "ferry",
                "name": "Veerdienst"
              },
              "operatorName": "GVB",
              "service": null,
              "platform": null,
              "platformChanged": false,
              "remark": null,
              "realtimeState": "ontime",
              "realtimeText": null
            }
          ]
        }
      ]
    }

