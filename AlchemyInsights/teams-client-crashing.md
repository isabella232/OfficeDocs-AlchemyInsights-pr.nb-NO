---
title: Krasjer Teams-klienten?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826280"
---
# <a name="teams-client-crashing"></a>Krasjer Teams-klienten?

Hvis Teams-klienten krasjer, kan du prøve følgende:

- Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontroller at alle Nettadresser og adresseområder for [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgjengelige.

- Logg på med administratorkontoen for [](https://docs.microsoft.com/office365/enterprise/view-service-health) leieren, og kontroller instrumentbordet for tjenestetilstand for å bekrefte at det ikke finnes noen avbrudd eller tjenesteforringelse.

- Avinstallere og installere Teams-programmet på nytt (kobling)
    - Bla til mappen %appdata%\Microsoft\teams\ på datamaskinen, og slett alle filene i denne katalogen.
    - [Last ned og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer om mulig Teams som administrator (høyreklikk på Teams-installasjonsprogrammet, og velg Kjør som administrator hvis tilgjengelig).

Hvis Teams-klienten fremdeles krasjer, kan du reprodusere problemet? Hvis det er det:

1. Bruk Trinninnspilling til å registrere trinnene.
    - Lukk ALLE unødvendige eller konfidensielle programmer.
    - Start Trinninnspilling, og reproduser problemet mens du er logget på med den berørte brukerkontoen.
    - [Samle inn teamloggene som registrerer de innspilte repro-trinnene.](https://docs.microsoft.com/microsoftteams/log-files) **Obs!** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.
    - Samle inn informasjon om dumping og/eller feilsamling (Windows). Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Legg ved filen i støttesaken.
