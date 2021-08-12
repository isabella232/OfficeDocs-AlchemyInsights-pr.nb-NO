---
title: API-tillatelser og samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932106"
---
# <a name="api-permissions-and-consent"></a>API-tillatelser og samtykke

Programmer som integreres med Microsofts identitetsplattform, følger en autorisasjonsmodell som gir brukere og administratorer kontroll over hvordan data kan nås. Implementeringen av autorisasjonsmodellen er oppdatert på Microsofts identitetsplattform endepunktet. Den endrer hvordan en app må samhandle med Microsofts identitetsplattform. [Tillatelser og samtykke i](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Microsofts identitetsplattform endepunktet dekker de grunnleggende konseptene i denne godkjenningsmodellen, inkludert omfang, tillatelser og samtykke.

Det [Azure Active Directory samtykkerammeverket (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gjør det enkelt å utvikle nettbaserte og opprinnelige klientprogrammer for flere leiere. Disse programmene tillater pålogging av brukerkontoer fra en Azure AD-leier som er forskjellig fra den der programmet er registrert. De må kanskje også få tilgang til nett-API-er, for eksempel Microsoft Graph API (for å få tilgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft-tjenester API-er, i tillegg til dine egne api-er på nettet.

