---
title: Finne hendelser som er utført på innboksregler
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058659"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finne hendelser som er utført på innboksregler

Når innboksregler opprettes, endres eller slettes, registreres hendelsene i overvåkingsloggen. Slik ser du gjennom dem:

1. Gå til [Office 365 Sikkerhets- & Samsvarssenter](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Velg Søk > søk i overvåkingsloggen.

    > [!NOTE]
    > Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere den nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.
1. Velg Aktiviteter-feltet, finn Exchange postboksaktiviteter, og velg deretter New-InboxRule Opprett innboksregel fra Outlook Web App. Når du er ferdig, klikker du utenfor ruten for å minimere Aktiviteter-ruten.
1. Angi datointervallet, og velg brukernavnet for brukeren du vil undersøke, i Brukere-feltet. Du kan velge mer enn én bruker om gangen.
1. Velg Søk. Aktivitetene vises under Resultater.
1. Hvis du vil vise detaljer, velger du en aktivitet og velger deretter Mer informasjon. Under Parametere-delen kan du se navnet på regelen, betingelsene som er angitt, og handlingene som regelen skal utføre.

Hvis du vil ha mer informasjon, kan du se Søke Office 365 overvåkingsloggen for å feilsøke vanlige scenarier.