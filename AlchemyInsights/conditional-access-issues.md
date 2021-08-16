---
title: Problemer med betinget tilgang
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
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069973"
---
# <a name="conditional-access-issues"></a>Problemer med betinget tilgang

**Løse problemer med påloggingsdiagnose**

Du kan raskt finne ut hva som har skjedd eller diagnostisere problemer relatert til brukerlogging ved hjelp [av påloggingsdiagnose:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Start Påloggingsdiagnose.
1. Finn hendelsen du vil analysere, ved å skrive inn detaljene du har om brukeren, programmet, tidspunktet for pålogging, forespørsels-ID eller korrelasjons-ID.
1. Se gjennom diagnoseresultatene som viser detaljer om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer (hvis det er nødvendig).

**Fremgangsmåte for å feilsøke en pålogging** 

1. Gå til påloggingssiden for Azure AD.
1. Filtrer pålogginger etter bruker, tidsområde, program, status, klientapp og så videre.
1. Velg en påloggingshendelse, og vis betinget tilgang-fanen for å se hvilke policyer som ble evaluert.
1. Klikk raden for en policy for å vise policydetaljene og forstå hvorfor den brukes.

**Verktøy for å feilsøke en policy for betinget tilgang**

- Med rapportmodus kan du evaluere en policy uten å påvirke brukere.
- Hva-skjer-hvis-verktøyet lar deg simulere påloggingshendelser og se hvilke policyer som gjelder.
- Insights og rapporteringsarbeidsboken viser sanntidseffekten av hver policy.

**Policyer for opprinnelig beskyttelse**

Policyer for beskyttelse av opprinnelig plan er avskrevet. De håndheves ikke lenger, og vil snart bli fjernet fra Azure Portal. Vi anbefaler at du aktiverer [sikkerhetsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Hvis du vil ha mer informasjon om betinget tilgang, kan du se:

[Anbefalte fremgangsmåter for betinget tilgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontroller i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Plasseringer i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
