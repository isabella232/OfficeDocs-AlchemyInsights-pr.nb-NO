---
title: Feilsøke feilkoder for Azure AD-godkjenning og autorisasjon (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036511"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Feilsøke feilkoder for Azure AD-godkjenning og autorisasjon (AADSTS)

Hvis du vil løse AAD-godkjenning og autorisasjonsfeilkoder (AADSTS), utfører du følgende anbefalte trinn:

1. **Håndtere feilkoder i programmet**

- **OAuth2.0-spesifikasjonen**, gir veiledning om hvordan du håndterer feil under godkjenning ved hjelp av feildelen https://tools.ietf.org/html/rfc6749#section-5.2 av feilsvaret.

    - **feil**: En feilkodestreng som kan brukes til å klassifisere feiltyper som oppstår, og som skal brukes til å reagere på feil.
    - **Feilfeltet** har flere mulige verdier – se gjennom koblingene for protokolldokumentasjonen og OAuth 2.0-spesifikasjoner for mer informasjon om bestemte feil og hvordan du reagerer på dem.

- Her er et eksempel på et feilsvar:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Oppslagsinformasjon om gjeldende feilkode**

- Feilkoder og meldinger kan endres. Hvis du vil ha den nyeste informasjonen, kan du se siden for å finne https://login.microsoftonline.com/error AADSTS-feilbeskrivelser, løsninger og noen foreslåtte midlertidige løsninger.
- Du kan også søke etter og feilsøke [AADSTS-feilkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) som er oppført i artikkelen [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Få hjelp**

- [Støtte- og hjelpealternativer for](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) utviklere – Hvis du trenger svar på et spørsmål eller hjelp til å løse et problem som ikke dekkes i dokumentasjonen vår, kan det være på tide å ta kontakt med eksperter for å få hjelp. Denne artikkelen inneholder flere forslag for å få svar på spørsmålene dine etter hvert som du utvikler apper som integreres med Microsofts identitetsplattform.








