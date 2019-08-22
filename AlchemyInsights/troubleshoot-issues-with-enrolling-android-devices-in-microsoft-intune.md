---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500080"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Android-enheter i Microsoft Intune

Se gjennom ressursene som vises nedenfor for å løse problemet nå.
  
Noen vanlige problemer og Løsningstrinn:
  
 **Enhet ikke kryptert feil i Company Portal:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et passord for oppstart å forsikre deg om at enheten er fullstendig kryptert. Vanlige løsninger er å aktivere en PIN-kode for oppstart eller kryptere fullstendig enheten. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.
  
 **Enheter kan ikke være på tjenesten Intune eller vise som "Unhealthy" i admin-konsollen Intune:** Noen Samsung 4.4 og 5.5 enheter kan ikke sjekke inn i tjenesten. Det er 3 mulige løsninger på dette problemet:
  
1. Åpne Intune Company Portal-app, som automatisk starter en enhetssynkronisering manuelt.

2. Oppdatere enheten til Android 6.0 eller høyere.

3. Deaktiver Samsung Smart Manager fra å behandle Intune Company Portal. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for ytterligere informasjon om disse problemer og løsninger.

 **Brukeren lisens Type ugyldig** eller **bruker navnet ikke gjenkjennes feil:** brukeren må tilordnes en Intune eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: Office Admin Center eller Azure portal.
  
Ytterligere ressurser til å løse problemet:
  
1. Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.

2. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som hindrer registrering og løsninger for hver.

3. [Lær hvordan du kan registrere Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
