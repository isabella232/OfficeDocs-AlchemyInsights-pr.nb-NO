---
title: Sitter fast i utboksen på grunn av store vedlegg
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241261"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Løse meldinger som sitter fast i utboksen

Vi anbefaler at du starter med å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [verktøyet Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)

Når en melding sitter fast i utboksen, er den mest sannsynlige årsaken et stort vedlegg eller alternativet "Send umiddelbart når den er tilkoblet" er ikke aktivert.

**Fjern det store tilbehøret**

1. I Outlook velger du **Send / motta** > **arbeid frakoblet**. 
2. Velg **Utboks**i navigasjonsruten. Herfra kan du: 
    - Slett meldingen (velg den, og velg deretter **Slett**).
    - Dra meldingen til Kladd-mappen, dobbeltklikk for å åpne den, og fjern vedlegget, velg den og velg deretter **Slett**).
3. Hvis du får en feilmelding som sier at Outlook prøver å overføre meldingen, lukker du Outlook. Det kan ta litt tid å avslutte. Hvis Outlook ikke lukkes, trykker du CTRL+ALT+Slett og velger **Start Oppgavebehandling**. I Oppgavebehandling velger du **kategorien Prosesser,** blar ned til outlook.exe, og velger **Avslutt prosess**.
4. Når Outlook lukkes, starter du den på nytt og gjentar trinn 2 og 3. 
5. Når du har fjernet vedlegget, klikker du **Send / motta** > **arbeid frakoblet** for å fortsette arbeidet på nettet. 

Meldinger blir også sittende fast i utboksen når du klikker **Send**, men du er ikke tilkoblet. Klikk **Send / motta** og se på Arbeid **frakoblet-knappen.** Hvis den er blå, kobles du fra. Klikk den for å koble til (knappen blir hvit) og klikk **Send alle**.
 
**Aktiver Send umiddelbart når du er tilkoblet**
 
1. Klikk **Alternativer**i kategorien Fil .

2. Klikk **Avansert**i dialogboksen Alternativer for Outlook .

3. Klikk for å aktivere Send **umiddelbart når du er tilkoblet,** i delen Send og motta . Klikk på **OK**.
 
Hvis du vil ha mer informasjon, kan du se:
- [Video: Sende eller slette en fast e-post](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-post forblir i utboksmappen til du manuelt starter en send/motta-operasjon i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
