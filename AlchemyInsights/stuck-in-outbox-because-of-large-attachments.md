---
title: Stakk i utboksen på grunn av store vedlegg
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441314"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Rette opp meldinger som sitter fast i utboksen

Vi anbefaler at du starter ved å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [Microsoft Kundestøtte og gjenoppretting Assistant](https://diagnostics.office.com/#/) verktøyet.

Når en melding blir værende i utboksen, er de mest sannsynlige årsakene:
- Store vedlegg.
- Alternativet **Send umiddelbart når tilkoblet** er ikke aktivert.

Slik fjerner du store vedlegg: 

1. Velg **Send/motta** > **arbeid frakoblet**i Outlook. 
2. Velg **Utboks**i navigasjonsruten. Herfra kan du gjøre følgende: 
    - Slett meldingen (Merk den, og velg deretter **Slett**).
    - Dra meldingen til Kladd-mappen, dobbeltklikk for å åpne den, og fjern vedlegget, Velg den, og velg deretter **Slett**).
3. Hvis du får en feilmelding som sier at Outlook prøver å overføre meldingen, lukker du Outlook. Det kan ta litt tid å avslutte. Hvis Outlook ikke lukkes, trykker du Ctrl + Alt + Delete og velger **Start Oppgavebehandling**. I Oppgavebehandling velger du kategorien **prosesser** , blar ned til Outlook. exe og velger **Avslutt prosess**.
4. Når Outlook lukkes, starter du det på nytt og gjentar trinn 2 og 3. 
5. Når du har fjernet vedlegget, klikker du **Send/motta** > **arbeid frakoblet** for å gjenoppta arbeidet online. 

Meldinger blir også værende i utboksen når du klikker **Send**, men du er ikke tilkoblet. Klikk **Send og motta** , og se på **arbeid frakoblet** -knappen. Hvis den er blå, er du frakoblet. Velg den for å koble til (knappen blir hvit) og klikk på **Send alle**.
 
Slik aktiverer du **sending umiddelbart når**du er tilkoblet:
 
- Velg **fil** > **Alternativer** >  **Avansert**.
I delen **Send og motta** velger du **Send umiddelbart når**du er tilkoblet, og deretter velger du **OK**.
 
For alle detaljer, se:
- [Video: sende eller slette en fastlåst e-post](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-post blir værende i Utboks-mappen til du manuelt starter en operasjon for sending/mottak i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
