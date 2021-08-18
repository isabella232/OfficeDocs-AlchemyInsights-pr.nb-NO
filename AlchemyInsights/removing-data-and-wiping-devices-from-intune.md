---
title: Fjerne data og sletteenheter fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331050"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjerne data og sletteenheter fra Intune

Eksterne handlinger for fjerning av enheter og enhetsutsletting kan brukes til å fjerne firmadata som administreres av Intune, eller til å utføre tilbakestilling til fabrikkinnstillinger og returnere enheten til standardinnstillingene.

1. Logg på Microsoft 365 Device Management, og gå til **Enheter** > **Alle enheter**.
2. Velg enheten du vil fjerne.
3. Velg hvilken type ekstern sletting du vil utføre. Tilbaketrekking sletter bare organisasjonsinformasjon, mens total sletting gjenoppretter enheten til fabrikkinnstillingene.
4. Velg **Ja** for å bekrefte. Inntil slettingen er ferdig, vises Enhetens handlingsstatus som *Tilbaketrekking venter*.
    Når handlingen er fullført, ser du ikke lenger den mobile enheten i listen over administrerte enheter.

**Obs!** Firmadata kan ikke fjernes fra enheter SOM BLIR MED TIL Azure AD. 

Hvis du vil ha detaljert informasjon om effekten av handlingene Tilbaketrekking og Sletting, inkludert hva som beholdes og hva som slettes, kan du se følgende dokumentasjon:

- [Fjern enheter ved hjelp av sletting, fjerning eller manuell avregistrering av enheten](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Slik sletter du bare bedriftsdata fra Intune-administrerte apper](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Slett alle data fra en macOS-enhet](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).