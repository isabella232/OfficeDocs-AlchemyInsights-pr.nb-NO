---
title: Finne hendelser som utføres på innboksregler
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430011"
---
# <a name="find-events-performed-on-inbox-rules"></a>Finne hendelser som utføres på innboksregler

Når innboksregler opprettes, endres eller slettes, registreres hendelsene i overvåkingsloggen. Slik ser du gjennom dem:

1. Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Velg Søk > søk i overvåkingsloggen.

    > [!NOTE]
    > Hvis du ser en melding om at du må aktivere overvåking, går du videre og slår den på nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.
1. Velg Aktiviteter-feltet og finn aktiviteter for Exchange-postboksen, og velg deretter New-InboxRule Opprett innboksregel fra Outlook Web App. Når du er ferdig, klikker du utenfor ruten for å minimere Aktiviteter-ruten.
1. Angi datoområdet, og velg brukernavnet for brukeren du vil undersøke, i Brukere-feltet. Du kan velge mer enn én bruker om gangen.
1. Velg Søk. Aktivitetene vises under Resultater.
1. Hvis du vil vise detaljer, velger du en aktivitet og velger deretter Mer informasjon. Under Parametere-delen kan du se navnet på regelen, betingelsene som er angitt, og handlingene regelen vil utføre.

Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for Office 365 for å feilsøke vanlige scenarier.