# Messages/disturbances

	GET https://api.9292.nl/0.1/messages/disturbances

## Abstract

Met de `messages/disturbances`-resource kan een lijst van ongeplande storingen
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
| **calamity** | Bevat een `calamity` object (indien beschikbaar). |
| **total** | Bevat getal dat het totaal aantal ongeplande storingen weergeeft (waarbij `rows` dus buiten beschouwing wordt gelaten). |
| **disturbances** | Bevat een array van `disturbance` objecten. |

## Voorbeeld

### Request

	GET /0.1/messages/disturbances?lang=nl-NL&rows=10&start=0&q=
	Host: api.9292.nl

### Response

	{
	  "calamity": {
		"title": "Sneeuw hindert openbaar vervoer",
		"introduction": {
		  "title": "Houd rekening met vertraging",
		  "textHtml": "<p>Vanwege het winterweer&nbsp;rijdt het openbaar vervoer anders dan je gewend bent. In ieder reisadvies dat je opvraagt bij 9292 kun je zien of er vertraging is door op de halte of het station te klikken. Of bel voor de meest actuele reisinformatie met 0900 9292.</p>",
		  "imageUrl": "/gimmage/N2/Mobile/Calamiteiten/Bevroren%20tak.jpg",
		  "imageText": "Beeld van een bevroren tak met sneeuw"
		},
		"textHtml": "<h3>Trein</h3>\n<p>NS rijdt&nbsp;21 en 22 januari volgens een aangepaste dienstregeling. De OV-reisplanner is bijgewerkt. De overige spoorvervoerders rijden de normale dienstregeling.&nbsp;<br /><br />De Thalys tussen Amsterdam en Brussel/Parijs, vertrek 09:19 en 18:19,&nbsp;rijdt vandaag niet.&nbsp;</p>\n<h3>Bus, Tram en Metro</h3>\n<p>Op dit moment rijdt&nbsp;bijna al het openbaar vervoer weer. Er kunnen nog vertraging zijn&nbsp;van 5 &agrave; 15 minuten.</p>\n<p>De bijzonderheden in het openbaar vervoer op dit moment zijn;</p>\n<ul>\n<li>HTM<br />Tram 1 rijdt volgens een aangepaste route en de tramlijnen 6 en 16 rijden op dit moment niet.</li>\n</ul>\n<h3>Actuele vertrektijden</h3>\n<p>Op de stationspagina's van 9292&nbsp;kun je de actuele vertrektijden zien. Hieronder een aantal voorbeelden:</p>\n<ul class=\"link-list\">\n<li><a title=\"link naar stationspagina\" href=\"http://9292.nl/station-utrecht-centraal\">Utrecht Centraal</a></li>\n<li><a href=\"http://9292.nl/station-breda\">Breda</a></li>\n<li><a href=\"http://9292.nl/station-arnhem\">Arnhem</a></li>\n<li><a href=\"http://9292.nl/station-amersfoort\">Amersfoort</a></li>\n<li><a href=\"http://9292.nl/station-s-hertogenbosch\">Den Bosch</a></li>\n<li><a title=\"Link naar de station pagina van Zwolle\" href=\"http://9292.nl/station-zwolle\">Zwolle</a></li>\n</ul>\n<p><img src=\"/gimmage/N2/Mobile/Twitter.png\" alt=\"Twitter logo\" width=\"65\" height=\"55\" /></p>\n<p>Volg ons op <a title=\"Link naar het Twitter account van 9292\" href=\"https://twitter.com/9292\">Twitter</a> en blijf op de hoogte van ons laatste nieuws.</p>\n<p>Laatste update&nbsp;16.00 uur</p>"
	  },
	  "total": 6,
	  "disturbances": [
		{
		  "plannerDisturbanceId": "146146",
		  "title": "Veendam, Zuidbroek",
		  "datesString": "21-01-2013, 17:29 uur tot 21-01-2013, 18:00 uur",
		  "startDateTime": "2013-01-21T17:29",
		  "endDateTime": "2013-01-21T18:00",
		  "cause": "Wisselstoring",
		  "effect": "Vervoer ontregeld",
		  "measure": null,
		  "advice": null,
		  "operatorAdvice": "De beperkingen als gevolg van een wisselstoring tussen Zuidbroek en Veendam zijn voorbij.\nDe vertraging zal geleidelijk afnemen.",
		  "lines": [],
		  "clusters": [],
		  "clusterRanges": [
			{
			  "oneWay": false,
			  "start": {
				"location": null,
				"fallbackPointName": "Station Zuidbroek ",
				"fallbackPlaceName": "Zuidbroek"
			  },
			  "end": {
				"location": null,
				"fallbackPointName": "Station Veendam",
				"fallbackPlaceName": "Veendam"
			  }
			}
		  ],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146139",
		  "title": "Lelystad Centrum, Zwolle",
		  "datesString": "21-01-2013, 15:46 uur tot 21-01-2013, 18:30 uur",
		  "startDateTime": "2013-01-21T15:46",
		  "endDateTime": "2013-01-21T18:30",
		  "cause": "Wisselstoring",
		  "effect": "Minder vervoer",
		  "measure": null,
		  "advice": null,
		  "operatorAdvice": "Tussen Lelystad Centrum en Zwolle moeten reizigers rekening houden met een vertraging van 30 \ntot 60 minuten.\nDoor een wisselstoring rijden er tussen Lelystad Centrum en Zwolle minder treinen.",
		  "lines": [],
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
				"fallbackPointName": "Station Zwolle ",
				"fallbackPlaceName": "Zwolle"
			  }
			}
		  ],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146147",
		  "title": "Uitgeest, Zaandam",
		  "datesString": "21-01-2013, 17:50 uur tot 21-01-2013, 19:30 uur",
		  "startDateTime": "2013-01-21T17:50",
		  "endDateTime": "2013-01-21T19:30",
		  "cause": "Aanrijding met een persoon",
		  "effect": "Geen treinen",
		  "measure": null,
		  "advice": null,
		  "operatorAdvice": "Tussen Zaandam en Wormerveer moeten reizigers rekening houden met een vertraging van meer \ndan 60 minuten.\nDoor een aanrijding met een persoon rijden er tussen Zaandam en Wormerveer geen treinen.",
		  "lines": [],
		  "clusters": [],
		  "clusterRanges": [
			{
			  "oneWay": false,
			  "start": {
				"location": null,
				"fallbackPointName": "Station Zaandam ",
				"fallbackPlaceName": "Zaandam"
			  },
			  "end": {
				"location": null,
				"fallbackPointName": "Station Uitgeest ",
				"fallbackPlaceName": "Uitgeest"
			  }
			}
		  ],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146047",
		  "title": "Den Haag, Zoetermeer: HTM tram RR 3, RR 4",
		  "datesString": "18-01-2013, 15:50 uur tot 21-01-2013, 23:59 uur",
		  "startDateTime": "2013-01-18T15:50",
		  "endDateTime": "2013-01-21T23:59",
		  "cause": "Weersomstandigheden",
		  "effect": null,
		  "measure": "route aangepast",
		  "advice": "RR3 en RR4 rijden alleen rechtsom door de krakeling.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "RR 3",
			  "operatorName": "HTM",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"Zoetermeer Centrum West",
				"Loosduinen"
			  ]
			},
			{
			  "name": "RR 4",
			  "operatorName": "HTM",
			  "modeName": "Tram",
			  "modeType": "Tram",
			  "destinationNames": [
				"De Uithof",
				"Zoetermeer Javalaan"
			  ]
			}
		  ],
		  "clusters": [],
		  "clusterRanges": [],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146144",
		  "title": "Rotterdam: RET metro ABC",
		  "datesString": "21-01-2013, 17:20 uur tot 21-01-2013, 23:59 uur",
		  "startDateTime": "2013-01-21T17:20",
		  "endDateTime": "2013-01-21T23:59",
		  "cause": "Herstelwerkzaamheden",
		  "effect": null,
		  "measure": "Vervallen halte(n) Kralingsezoom",
		  "advice": "Door werkzaamheden Kralingse Zoom wordt op metrolijn A, B en C er niet gereden tussen metrostation Capelse Brug en Voorschoterlaan. Houd rekening met extra reistijd en overstap. Er worden bussen ingezet.",
		  "operatorAdvice": null,
		  "lines": [
			{
			  "name": "ABC",
			  "operatorName": "RET",
			  "modeName": "Metro",
			  "modeType": "Metro",
			  "destinationNames": [
				"C/D De Akkers",
				"A Binnenhof"
			  ]
			}
		  ],
		  "clusters": [],
		  "clusterRanges": [
			{
			  "oneWay": false,
			  "start": {
				"location": null,
				"fallbackPointName": "Capelsebrug",
				"fallbackPlaceName": "Rotterdam"
			  },
			  "end": {
				"location": null,
				"fallbackPointName": "Voorschoterlaan",
				"fallbackPlaceName": "Rotterdam"
			  }
			}
		  ],
		  "alternativeClusters": []
		},
		{
		  "plannerDisturbanceId": "146131",
		  "title": "Groningen, Leeuwarden",
		  "datesString": "21-01-2013, 14:07 uur tot 22-01-2013, 02:00 uur",
		  "startDateTime": "2013-01-21T14:07",
		  "endDateTime": "2013-01-22T02:00",
		  "cause": "Wisselstoring",
		  "effect": "Minder vervoer",
		  "measure": null,
		  "advice": null,
		  "operatorAdvice": "Tussen Leeuwarden en Groningen moeten reizigers rekening houden met een vertraging van 30 tot \n60 minuten.\nDoor een wisselstoring rijden er tussen Leeuwarden en Groningen minder treinen.",
		  "lines": [],
		  "clusters": [],
		  "clusterRanges": [
			{
			  "oneWay": false,
			  "start": {
				"location": null,
				"fallbackPointName": "Station Leeuwarden ",
				"fallbackPlaceName": "Leeuwarden"
			  },
			  "end": {
				"location": null,
				"fallbackPointName": "Station Groningen ",
				"fallbackPlaceName": "Groningen"
			  }
			}
		  ],
		  "alternativeClusters": []
		}
	  ]
	}
