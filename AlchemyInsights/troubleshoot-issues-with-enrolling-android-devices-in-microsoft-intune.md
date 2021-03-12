---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709007"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Android-enheter i Microsoft Intune

Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.
  
Noen vanlige problemer og løsningstrinn:
  
 **Enheten er ikke kryptert i firmaportalen:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et oppstartspassord for å sikre at enheten er fullstendig kryptert. Vanlige løsninger er å aktivere en oppstarts-PIN-kode eller fullstendig kryptere enheten. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.
  
 Enheter kan ikke sjekke inn med Intune-tjenesten eller vises som «Ugyldige» i **Intune-administrasjonskonsollen:** Enkelte Samsung 4.4- og 5.5-enheter sjekker kanskje ikke inn tjenesten. Det finnes tre mulige løsninger på dette problemet:
  
1. Åpne Firmaportal-appen for Intune manuelt, som automatisk starter en enhetssynkronisering.

2. Oppdater enheten til Android 6.0 eller nyere.

3. Deaktiver Smart Manager for Samsung fra å administrere firmaportalen for Intune. Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.

 **Feilmelding om ugyldig brukerlisenstype** **eller brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune- eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via administrasjonssenteret for Office eller Azure Portal.
  
Flere ressurser som kan hjelpe deg med å løse problemet:
  
1. Bruk [feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil. Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

2. Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som forhindrer registrering og løsninger for hver av dem.

3. [Lær hvordan du registrere Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
