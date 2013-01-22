# Messages/deviations

	GET https://api.9292.nl/0.1/messages/deviations

## Abstract

Met de `messages/deviations`-resource kan een lijst van geplande storingen
opgehaald worden.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |
| **rows** | Bevat het maximum aantal storingen dat opgehaald moet worden. |
| **start** | Bevat een getal waarvandaan gestart moet worden met het ophalen van storingen. |
| **q** | Bevat een zoekterm. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **total** | Bevat getal dat het totaal aantal geplande storingen weergeeft (waarbij `rows` dus buiten beschouwing wordt gelaten). |
| **disturbances** | Bevat een array van `disturbance` objecten. |

## Voorbeeld

### Request

	GET /0.1/messages/deviations?lang=nl-NL&rows=10&start=0&q=
	Host: api.9292.nl

### Response

	{
	  "total": 207,
	  "disturbances": [
		{
		  "plannerDisturbanceId": "145123",
		  "title": "Enschede: Connexxion bus 6",
		  "datesString": "30-11-2012, 00:00 uur tot 21-01-2013, 23:59 uur",
		  "startDateTime": "2012-11-30T00:00",
		  "endDateTime": "2013-01-21T23:59",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Vervangende haltes",
		  "advice": null,
		  "operatorAdvice": "In verband met de afsluiting van de Kanaalstraat rijdt de bus een andere route.",
		  "lines": [
			{
			  "name": "6",
			  "operatorName": "Connexxion",
			  "modeName": "Stadsbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Stokhorst",
				"Boekelo"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Lonnekerbrugstraat",
			  "fallbackPlaceName": "Enschede"
			},
			{
			  "location": null,
			  "fallbackPointName": "Orion",
			  "fallbackPlaceName": "Enschede"
			},
			{
			  "location": null,
			  "fallbackPointName": "Scansped",
			  "fallbackPlaceName": "Enschede"
			},
			{
			  "location": null,
			  "fallbackPointName": "Transportcentrum",
			  "fallbackPlaceName": "Enschede"
			},
			{
			  "location": null,
			  "fallbackPointName": "Kanaalstraat",
			  "fallbackPlaceName": "Enschede"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "145459",
		  "title": "Hoogerheide: Veolia bus 104, 105",
		  "datesString": "14-01-2013, 09:00 uur tot 22-01-2013, 18:00 uur",
		  "startDateTime": "2013-01-14T09:00",
		  "endDateTime": "2013-01-22T18:00",
		  "cause": "Cyclecross",
		  "effect": "Vervallen haltes",
		  "measure": "Route aangepast",
		  "advice": "In-/uitstappen: huijbergseweg.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "104",
			  "operatorName": "Veolia",
			  "modeName": "Bus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Roosendaal",
				"Bergen op Zoom"
			  ]
			},
			{
			  "name": "105",
			  "operatorName": "Veolia",
			  "modeName": "Bus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Putte (B)",
				"Bergen op Zoom"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Raadhuisstraat",
			  "fallbackPlaceName": "Hoogerheide"
			},
			{
			  "location": null,
			  "fallbackPointName": "Dr de Bruijnlaan",
			  "fallbackPlaceName": "Hoogerheide"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146123",
		  "title": "Lelystad Centrum, Vlissingen: NS trein",
		  "datesString": "21-01-2013, 08:00 uur tot 22-01-2013, 23:59 uur",
		  "startDateTime": "2013-01-21T08:00",
		  "endDateTime": "2013-01-22T23:59",
		  "cause": "Aanpassing dienstregeling door winterweer",
		  "effect": "Overstap in roosendaal",
		  "measure": null,
		  "advice": "door de aanpassing gaat deze trein niet rechtstreeks maar dient er extra in roosendaal te worden overgestapt.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "26",
			  "operatorName": "NS",
			  "modeName": "Sneltrein",
			  "modeType": "Trein",
			  "destinationNames": [
				"Den Haag Centraal",
				"Vlissingen"
			  ]
			}
		  ],
		  "clusters": [],
		  "clusterRanges": [
			{
			  "oneWay": false,
			  "start": {
				"location": null,
				"fallbackPointName": "Station Lelystad Centrum ",
				"fallbackPlaceName": "Lelystad"
			  },
			  "end": {
				"location": null,
				"fallbackPointName": "Station Vlissingen ",
				"fallbackPlaceName": "Vlissingen"
			  }
			}
		  ],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "144637",
		  "title": "Amsterdam: GVB tram 1, 2, 5, 13, 14, 17",
		  "datesString": "20-01-2013, 20:00 uur tot 25-01-2013, 03:59 uur",
		  "startDateTime": "2013-01-20T20:00",
		  "endDateTime": "2013-01-25T03:59",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Route aangepast",
		  "advice": "In-/uitstappen: bij tijdelijke halte in de raadhuisstraat, tussen de spuistraat en de nieuwezijds voorburgwal.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "1",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Centraal Station",
				"Osdorp de Aker"
			  ]
			},
			{
			  "name": "2",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Centraal Station",
				"Nieuw Sloten"
			  ]
			},
			{
			  "name": "5",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Amstelveen Binnenhof",
				"Centraal Station"
			  ]
			},
			{
			  "name": "13",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Centraal Station",
				"Geuzenveld"
			  ]
			},
			{
			  "name": "14",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Flevopark",
				"Slotermeer"
			  ]
			},
			{
			  "name": "17",
			  "operatorName": "GVB",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Centraal Station",
				"Osdorp Dijkgraafplein"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Martelaarsgracht",
			  "fallbackPlaceName": "Amsterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Dam/Raadhuisstraat",
			  "fallbackPlaceName": "Amsterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Dam/Paleisstraat",
			  "fallbackPlaceName": "Amsterdam"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "144644",
		  "title": "Amsterdam: GVB bus 352, 354, 358",
		  "datesString": "20-01-2013, 20:00 uur tot 25-01-2013, 03:59 uur",
		  "startDateTime": "2013-01-20T20:00",
		  "endDateTime": "2013-01-25T03:59",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Route aangepast",
		  "advice": "In-/uitstappen: ter hoogte van de bestaande halten nieuwezijds kolk en dam, lang het trottoir.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "352",
			  "operatorName": "GVB",
			  "modeName": "Nachtbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Centraal Station",
				"Geuzenveld"
			  ]
			},
			{
			  "name": "354",
			  "operatorName": "GVB",
			  "modeName": "Nachtbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Amstelveen Waardhuizen",
				"Centraal Station"
			  ]
			},
			{
			  "name": "358",
			  "operatorName": "GVB",
			  "modeName": "Nachtbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Centraal Station",
				"Badhoevedorp"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Dam/Raadhuisstraat",
			  "fallbackPlaceName": "Amsterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Westermarkt",
			  "fallbackPlaceName": "Amsterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Marnixstraat/Rozengracht",
			  "fallbackPlaceName": "Amsterdam"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "145810",
		  "title": "Utrecht: Connexxion bus 3",
		  "datesString": "20-01-2013, 23:00 uur tot 25-01-2013, 06:00 uur",
		  "startDateTime": "2013-01-20T23:00",
		  "endDateTime": "2013-01-25T06:00",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Vervangende haltes",
		  "advice": null,
		  "operatorAdvice": "Lijn 3 rijdt in deze periode via de Biltstraat",
		  "lines": [
			{
			  "name": "3",
			  "operatorName": "Connexxion",
			  "modeName": "Stadsbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Burg Fockema Andreaelaan",
				"Zuilen Noord"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Stadsschouwburg",
			  "fallbackPlaceName": "Utrecht"
			},
			{
			  "location": null,
			  "fallbackPointName": "Station Maliebaan Utrecht",
			  "fallbackPlaceName": "Utrecht"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "145308",
		  "title": "Rotterdam: RET bus 35, B10",
		  "datesString": "14-01-2013, 04:00 uur tot 25-01-2013, 18:00 uur",
		  "startDateTime": "2013-01-14T04:00",
		  "endDateTime": "2013-01-25T18:00",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Route aangepast",
		  "advice": "In-/uitstappen: bij tijdelijke halten aan de meidoornsingel",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "35",
			  "operatorName": "RET",
			  "modeName": "Stadsbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Rotterdam Noord",
				"Rotterdam Station Alexander"
			  ]
			},
			{
			  "name": "B10",
			  "operatorName": "RET",
			  "modeName": "Bobbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Rotterdam Centraal"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Kastanjeplein",
			  "fallbackPlaceName": "Rotterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Peppelweg",
			  "fallbackPlaceName": "Rotterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Hazelaarweg",
			  "fallbackPlaceName": "Rotterdam"
			},
			{
			  "location": null,
			  "fallbackPointName": "Adrianalaan",
			  "fallbackPlaceName": "Rotterdam"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "145171",
		  "title": "Nederweert: Veolia bus 61",
		  "datesString": "28-12-2012, 11:40 uur tot 25-01-2013, 23:59 uur",
		  "startDateTime": "2012-12-28T11:40",
		  "endDateTime": "2013-01-25T23:59",
		  "cause": "Nieuwe route nog niet gereed",
		  "effect": "Vervallen haltes",
		  "measure": "Route aangepast",
		  "advice": null,
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "61",
			  "operatorName": "Veolia",
			  "modeName": "Bus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Venlo",
				"Weert"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Schoolstraat",
			  "fallbackPlaceName": "Nederweert"
			},
			{
			  "location": null,
			  "fallbackPointName": "Loverstraat",
			  "fallbackPlaceName": "Nederweert"
			},
			{
			  "location": null,
			  "fallbackPointName": "Gemeentehuis",
			  "fallbackPlaceName": "Nederweert"
			},
			{
			  "location": null,
			  "fallbackPointName": "De Pinnenhof",
			  "fallbackPlaceName": "Nederweert"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "144232",
		  "title": "Dedemsvaart: Syntus bus 83S",
		  "datesString": "22-10-2012, 05:00 uur tot 26-01-2013, 03:59 uur",
		  "startDateTime": "2012-10-22T05:00",
		  "endDateTime": "2013-01-26T03:59",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Er wordt via een andere route gereden",
		  "advice": "In-/uitstappen: Mien Ruyslaan",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "83S",
			  "operatorName": "Syntus",
			  "modeName": "Bus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Dedemsvaart",
				"Zwolle",
				"Hardenberg"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Krikkenstraat",
			  "fallbackPlaceName": "Dedemsvaart"
			},
			{
			  "location": null,
			  "fallbackPointName": "Haitjema",
			  "fallbackPlaceName": "Dedemsvaart"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "145205",
		  "title": "Apeldoorn: Syntus bus 6",
		  "datesString": "09-12-2012, 05:00 uur tot 26-01-2013, 03:59 uur",
		  "startDateTime": "2012-12-09T05:00",
		  "endDateTime": "2013-01-26T03:59",
		  "cause": "Werkzaamheden",
		  "effect": "Vervallen haltes",
		  "measure": "Er wordt via een andere route gereden",
		  "advice": "In-/uitstappen: De volgende haltes zijn vervallen: Ritbroekstraat, Prins Willem Alexanderlaan, Asselsestraat, driehuizerweg, H. Dunantlaan, Blekersweg en Prinses Beatrixlaan.\nEr is geen vervangende halte.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "6",
			  "operatorName": "Syntus",
			  "modeName": "Stadsbus",
			  "modeType": "Bus",
			  "destinationNames": [
				"Orden/Rijkskantoren"
			  ]
			}
		  ],
		  "clusters": [
			{
			  "location": null,
			  "fallbackPointName": "Blekersweg",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Ritbroekstraat",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Prins Willem Alexanderlaan",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Asselsestraat",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Driehuizerweg",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Prinses Beatrixlaan",
			  "fallbackPlaceName": "Apeldoorn"
			},
			{
			  "location": null,
			  "fallbackPointName": "Henri Dunantlaan",
			  "fallbackPlaceName": "Apeldoorn"
			}
		  ],
		  "clusterRanges": [],
		  "alternativeClusters": []
		}
	  ]
	}
