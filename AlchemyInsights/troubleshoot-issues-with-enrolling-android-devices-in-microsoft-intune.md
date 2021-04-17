---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830951"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Android-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.
  
Noen vanlige problemer og løsningstrinn:
  
 **Enhetsfeil ikke kryptert i firmaportalen:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et oppstartspassord for å sikre at enheten er fullstendig kryptert. Vanlige løsninger er å aktivere en oppstartsstift eller kryptere enheten fullstendig. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.
  
 **Enheter kan ikke sjekke inn med Intune-tjenesten eller vise den som «Usunn» i Administrasjonskonsollen for Intune:** Enkelte Samsung 4.4- og 5.5-enheter sjekker kanskje ikke inn tjenesten. Det finnes tre mulige løsninger på dette problemet:
  
1. Åpne Intune Company Portal-appen manuelt, som automatisk starter en enhetssynkronisering.

2. Oppdater enheten til Android 6.0 eller nyere.

3. Deaktiver Samsung Smart Manager fra å administrere Intune Company Portal. Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.

 **Feil med brukerlisenstypen Ugyldig** eller Brukernavn gjenkjennes **ikke:** Brukeren må tilordnes en Intune- eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens gjennom: Administrasjonssenter for Office eller Azure-portalen.
  
Flere ressurser for å løse problemet:
  
1. Bruk [Feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

2. Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som hindrer registrering og løsninger for hver av dem.

3. [Finn ut hvordan du kan registrere Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
