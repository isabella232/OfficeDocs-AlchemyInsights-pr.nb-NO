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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="b09af-102">Feilsøke feilkoder for Azure AD-godkjenning og autorisasjon (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="b09af-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="b09af-103">Hvis du vil løse AAD-godkjenning og autorisasjonsfeilkoder (AADSTS), utfører du følgende anbefalte trinn:</span><span class="sxs-lookup"><span data-stu-id="b09af-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="b09af-104">**Håndtere feilkoder i programmet**</span><span class="sxs-lookup"><span data-stu-id="b09af-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="b09af-105">**OAuth2.0-spesifikasjonen**, gir veiledning om hvordan du håndterer feil under godkjenning ved hjelp av feildelen https://tools.ietf.org/html/rfc6749#section-5.2 av feilsvaret.</span><span class="sxs-lookup"><span data-stu-id="b09af-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="b09af-106">**feil**: En feilkodestreng som kan brukes til å klassifisere feiltyper som oppstår, og som skal brukes til å reagere på feil.</span><span class="sxs-lookup"><span data-stu-id="b09af-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="b09af-107">**Feilfeltet** har flere mulige verdier – se gjennom koblingene for protokolldokumentasjonen og OAuth 2.0-spesifikasjoner for mer informasjon om bestemte feil og hvordan du reagerer på dem.</span><span class="sxs-lookup"><span data-stu-id="b09af-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="b09af-108">Her er et eksempel på et feilsvar:</span><span class="sxs-lookup"><span data-stu-id="b09af-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="b09af-109">**Oppslagsinformasjon om gjeldende feilkode**</span><span class="sxs-lookup"><span data-stu-id="b09af-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="b09af-110">Feilkoder og meldinger kan endres.</span><span class="sxs-lookup"><span data-stu-id="b09af-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="b09af-111">Hvis du vil ha den nyeste informasjonen, kan du se siden for å finne https://login.microsoftonline.com/error AADSTS-feilbeskrivelser, løsninger og noen foreslåtte midlertidige løsninger.</span><span class="sxs-lookup"><span data-stu-id="b09af-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="b09af-112">Du kan også søke etter og feilsøke [AADSTS-feilkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) som er oppført i artikkelen [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="b09af-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="b09af-113">**Få hjelp**</span><span class="sxs-lookup"><span data-stu-id="b09af-113">**Get Help**</span></span>

- <span data-ttu-id="b09af-114">[Støtte- og hjelpealternativer for](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) utviklere – Hvis du trenger svar på et spørsmål eller hjelp til å løse et problem som ikke dekkes i dokumentasjonen vår, kan det være på tide å ta kontakt med eksperter for å få hjelp.</span><span class="sxs-lookup"><span data-stu-id="b09af-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="b09af-115">Denne artikkelen inneholder flere forslag for å få svar på spørsmålene dine etter hvert som du utvikler apper som integreres med Microsofts identitetsplattform.</span><span class="sxs-lookup"><span data-stu-id="b09af-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








