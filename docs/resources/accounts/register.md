# Accounts/register

	POST https://api.9292.nl/0.1/accounts/register

## Abstract
De `accounts/register`-resource wordt aangeroepen wanneer een gebruiker een
nieuw 9292 account aanmaakt.

## Parameters

| Naam | Omschrijving |
|-----:|:-------------|
| **lang** | Bevat "nl-NL" in alle gevallen. Zelfs als de telefoon eigenlijk op Engels is ingesteld. |

## Body

De body van dit request is versleuteld in JSON (alhoewel de `"Content-Type"`-
header wel is ingesteld op `"application/x-www-form-urlencoded"`).

| Naam | Omschrijving |
|-----:|:-------------|
| **password** | Bevat het wachtwoord van de nieuwe gebruiker (moet uit minstens 8 karakters bestaan). |
| **email** | Bevat het e-mail adres van de nieuwe gebruiker. |

## Response

| Naam | Omschrijving |
|-----:|:-------------|
| **sessionId** | Bevat een unieke `accountID` (zie `types.md`). |

## Voorbeeld

### Request

	POST /0.1/accounts/register?lang=nl-NL HTTP/1.1
	Host: api.9292.nl
	Content-Type: application/x-www-form-urlencoded
	Content-Length: 47
	
	{"password":"abcdefgh","email":"Tim@apple.com"}

### Response

	{
	  "sessionId": "****2986-****-471e-****-****4e2d****"
	}
