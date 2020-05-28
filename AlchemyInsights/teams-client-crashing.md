---
title: Krasjer Teams-klienten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354061"
---
# <a name="teams-client-crashing"></a>Krasjer Teams-klienten?

Hvis Teams-klienten krasjer, kan du prøve følgende:

- Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontroller at alle [Microsoft 365 URL-adresser og adresseområder er tilgjengelige.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Logg inn med leieradministratorkontoen din, og sjekk instrumentbordet for [tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for å bekrefte at det ikke finnes noe nedetid eller tjenesteforringelse.

- Avinstallere og installere Teams-programmet på nytt (link)
    - Bla til mappen %appdata%\Microsoft\teams\ på datamaskinen, og slett alle filene i den mappen.
    - [Last ned og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer om mulig Teams som administrator (høyreklikk på Teams-installasjonsprogrammet og velg "Kjør som administrator" hvis tilgjengelig).

Hvis Teams-klienten din fortsatt krasjer, kan du gjenskape problemet? I så fall:

1. Bruk trinnopptakeren til å ta opp trinnene.
    - Lukk alle unødvendige eller konfidensielle applikasjoner.
    - Start steps recorder og reprodusere problemet mens du er logget inn med den berørte brukerkontoen.
    - [Samle teamloggene som fanger opp de registrerte reprotrinnene](https://docs.microsoft.com/microsoftteams/log-files). **Merk:** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.
    - Samle dump og / eller Feil bøtte info (Windows). Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Legg ved filen i støttesaken.
