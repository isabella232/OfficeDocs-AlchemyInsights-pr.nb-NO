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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232639"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Løse meldinger som sitter fast i utboksen

Vi anbefaler at du starter med å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [verktøyet Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) på den berørte maskinen.

Når en melding sitter fast i utboksen, er den mest sannsynlige årsaken et stort vedlegg eller alternativet "Send umiddelbart når den er tilkoblet" er ikke aktivert.

**Fjern det store tilbehøret**

1. Klikk **Send / motta** > **arbeid frakoblet**. 
2. Klikk **Utboks**i navigasjonsruten. Herfra kan du: 
    - Slett meldingen. Bare velg det og klikk **Slett**.
    - Dra meldingen til **kladdemappen,** dobbeltklikk for å åpne meldingen, og slett vedlegget (klikk det og klikk **Slett**).
3. Hvis det oppstår en feil i Outlook som prøver å overføre meldingen, lukker du Outlook. Det kan ta litt tid å avslutte. Hvis Outlook ikke lukkes, trykker du **CTRL+ALT+Slett** og klikker **Start Oppgavebehandling**. I Oppgavebehandling velger du **kategorien Prosesser,** blar ned til outlook.exe, og klikker **Avslutt prosess**.
4. Når Outlook lukkes, starter du Outlook på nytt og gjentar trinn 2-3. 
5. Når du har fjernet vedlegget, klikker du **Send / motta** > **arbeid frakoblet** for å fjerne merket for knappen og for å fortsette å jobbe på nettet. 

Meldinger blir også sittende fast i utboksen når du klikker **Send**, men du er ikke tilkoblet. Klikk **Send / motta** og se på Arbeid **frakoblet-knappen.** Hvis den er blå, kobles du fra. Klikk den for å koble til (knappen blir hvit) og klikk **Send alle**.
 
**Aktiver Send umiddelbart når du er tilkoblet**
 
1. Klikk **Alternativer**i kategorien Fil .

2. Klikk **Avansert**i dialogboksen Alternativer for Outlook .

3. Klikk for å aktivere Send **umiddelbart når du er tilkoblet,** i delen Send og motta . Klikk på **OK**.
 
Hvis du vil ha mer informasjon, kan du se:
- [Video: Sende eller slette en fast e-post](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-post forblir i utboksmappen til du manuelt starter en send/motta-operasjon i Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
