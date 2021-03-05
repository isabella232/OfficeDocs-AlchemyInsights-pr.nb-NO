---
title: Finne ut hvem som konfigurerte videresending for en postboks, og hvordan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482303"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Finne ut hvem som konfigurerte videresending for en postboks, og hvordan

Hvis ekstern videresending ble satt på en postboks, overvåkes aktiviteten som en del Set-Mailbox cmdlet. Slik finner du aktiviteten i overvåkingsloggen:

1. Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Velg **søk i** >  **overvåkingsloggen** for søk.
    > [!NOTE]
    > Hvis du ser en melding om at du må aktivere overvåking, går du videre og slår den på nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.
1. Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter** (standard). Angi datoområdet. Du trenger ikke å angi et brukernavn.
1. Velg **Søk.** Aktivitetene vises under **Resultater.**
1. Velg **Filterresultater,** og angi **deretter Set-mailbox** i **Aktivitetsfilter-feltet.** Dette returnerer alle **Set-Mailbox-aktiviteter.**
1. Hvis du vil vise detaljene, velger du en aktivitet og velger **deretter Mer informasjon.** Under **Parametere** kan du se e-postadressen for videresending som ble angitt for postboksen. **Bruker-ID-en** representerer brukeren som konfigurerte ekstern videresending for postboksen.
Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for [Office 365 for å feilsøke vanlige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)