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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014887"
---
# <a name="conditional-access-issues"></a>Problemer med betinget tilgang

**Løse problemer med påloggings diagnose**

Du kan raskt finne ut hva som skjedde eller diagnostisere problemer som er relatert til bruker pålogging ved hjelp av [påloggings diagnosen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Start påloggings diagnosen.
1. Finn hendelsen for å analysere ved å angi i detaljene du har om brukeren, programmet, påloggings tidspunktet, forespørsels-ID-en eller korrelasjons-IDen.
1. Se gjennom diagnose resultatene som viser informasjon om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer (hvis det er nødvendig med endringer).

**Fremgangs måte for å feilsøke påloggings problemer** 

1. Gå til påloggings siden for Azure AD.
1. Filtrer pålogginger etter bruker, tids intervall, program, status, klient program og så videre.
1. Velg en påloggings hendelse, og Vis betinget tilgang-fanen for å se hvilke policyer som ble evaluert.
1. Klikk på raden i en policy for å vise policy detaljene og forstå hvorfor den er brukt.

**Verktøy for å feilsøke en policy for betinget tilgang**

- Bare rapport modus lar deg evaluere en policy uten å påvirke brukere.
- Hva-skjer-hvis-verktøyet lar deg simulere påloggings hendelser og se hvilke policyer som gjelder.
- Innsikt-og rapporterings arbeids bok viser sann tids innvirkning for hver policy.

**Policyer for grunn linje beskyttelse**

Policyer for grunn linje beskyttelse er avverget. De blir ikke lenger håndhevet og vil snart bli fjernet fra Azure-portalen. Vi anbefaler at du aktiverer [sikkerhets standarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Hvis du vil ha mer informasjon om betinget tilgang, kan du se:

[Anbefalte Fremgangs måter for betinget tilgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontroller i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Plasseringer i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
