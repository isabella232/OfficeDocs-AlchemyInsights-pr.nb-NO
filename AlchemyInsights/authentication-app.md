---
title: Godkjenningsapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405067"
---
# <a name="authentication-app"></a>Godkjenningsapp

Hvis du er global administrator, kan du raskt finne ut hva som skjedde eller diagnostisere problemer relatert til brukerlogging ved hjelp av [påloggingsdiagnose](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Start diagnostikken ved å klikke[startdiagnose-knappen.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Finn hendelsen du vil analysere, ved å skrive inn detaljene du har om brukeren, programmet, tidspunktet for pålogging, forespørsels-ID eller korrelasjons-ID.
1. Se gjennom diagnoseresultatene som viser detaljer om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer, hvis det er nødvendig med endringer.

**Kontroller scenarioet som gjelder:**

1. Hvis en bruker ikke får et push-varsel i Microsoft Authenticator-appen, må du kontrollere at de ikke vises under de MFA-blokkerte brukerne, som beskrevet i Blokkere og [oppheve blokkeringen av brukere.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Hvis brukeren ikke er blokkert for MFA, men ikke mottar en push-varsling, kan de åpne Microsoft Authenticator-appen, som vil trekke ventende godkjenningsforespørsler.
1. Som en alternativ påloggingsmetode kan brukeren også klikke på Logg på en annen måte og velge å bruke en bekreftelseskode fra mobilappen.
1. Microsoft Authenticator-appen er den eneste tilgjengelige metoden for mange brukere. [Finn ut mer om sikkerhetsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), se Vanlige spørsmål om [Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for vanlige spørsmål og hvordan du løser dem.
 
**Anbefalte videoer**

[Slik konfigurerer du Authenticator-appen på en ny telefon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
