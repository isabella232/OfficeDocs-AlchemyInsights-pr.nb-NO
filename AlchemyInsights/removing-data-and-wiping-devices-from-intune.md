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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922250"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Fjerne data og sletteenheter fra Intune

Eksterne handlinger for fjerning av enheter og enhetsutsletting kan brukes til å fjerne firmadata som administreres av Intune, eller til å utføre tilbakestilling til fabrikkinnstillinger og returnere enheten til standardinnstillingene.

1. Logg på Microsoft 365 Device Management, og gå til **Enheter** > **Alle enheter**.
2. Velg enheten du vil fjerne.
3. Velg hvilken type ekstern sletting du vil utføre. Tilbaketrekking sletter bare organisasjonsinformasjon, mens total sletting gjenoppretter enheten til fabrikkinnstillingene.
4. Velg **Ja** for å bekrefte. Inntil slettingen er ferdig, vises Enhetens handlingsstatus som *Tilbaketrekking venter*.
    Når handlingen er fullført, ser du ikke lenger den mobile enheten i listen over administrerte enheter.

> [!NOTE]
> Firmadata kan ikke fjernes fra enheter SOM ER KOBLET TIL Azure AD. 

Hvis du vil ha detaljert informasjon om effekten av handlingene Tilbaketrekking og Sletting, inkludert hva som beholdes og hva som slettes, kan du se følgende dokumentasjon:

- [Fjern enheter ved hjelp av sletting, fjerning eller manuell avregistrering av enheten](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Slik sletter du bare bedriftsdata fra Intune-administrerte apper](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Slett alle data fra en macOS-enhet](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).