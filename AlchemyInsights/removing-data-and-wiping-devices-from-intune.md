---
title: Fjerne data og tørke enheter fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440460"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjerne data og tørke enheter fra Intune

Eksterne handlinger for enhetssletting og enhetssletting kan brukes til å fjerne firmadata som administreres av Intune, eller til å utføre en tilbakestilling til fabrikkinnstillingene og returnere enheten til standardinnstillingene.

1. Logg på Microsoft 365 Device Management, og gå til **Enheter**  >  **alle enheter**.
2. Velg enheten du vil tørke av.
3. Velg typen ekstern sletting du vil gjøre. Avslutt sletter bare organisasjonsinformasjon, mens fullstendige slettinger gjenoppretter enheten til fabrikkinnstillingene.
4. Velg **Ja** for å bekrefte. Til slettingen er ferdig, vises handlingsstatusen Enhet som Pensjonere venter.</br>
    Når handlingen er fullført, ser du ikke lenger mobilenheten i listen over administrerte enheter.

**Merk at** Firmadata kan ikke fjernes fra enheter som er KOBLET til Azure AD.

Hvis du vil ha mer informasjon om effekten av handlingene Trekk tilbake og tørk, inkludert hva som beholdes og hva som slettes, kan du se [Fjerne enheter ved hjelp av tørk, trekk ut eller rulle ut enheten manuelt](https://docs.microsoft.com/intune/devices-wipe).

Hvis du vil slette alle data fra en macOS-enhet, kan du se [Slette alle data fra en macOS-enhet](https://docs.microsoft.com/intune/device-erase).