---
title: Teams klient krasjer
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890347"
---
# <a name="teams-client-crashing"></a>Teams klient krasjer

Hvis Teams-klienten krasjer, kan du prøve følgende:

- Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontroller at alle [Microsoft 365 nettadresser](https://docs.microsoft.com/microsoftteams/connectivity-issues) og adresseområder er tilgjengelige.

- Logg på med administratorkontoen for [](https://docs.microsoft.com/office365/enterprise/view-service-health) leieren, og kontroller instrumentbordet for tjenestetilstand for å bekrefte at ingen avbrudd eller tjenestereduksjon finnes.

- Avinstallere og installere Teams-programmet på nytt
    - Bla til mappen %appdata%\Microsoft\Teams\ på datamaskinen, og slett alle filene i denne katalogen.
    - Last ned og installer [Teams-appen](https://www.microsoft.com/microsoft-teams/download-app), og installer om mulig Teams som administrator (høyreklikk installasjonsprogrammet for Teams, og velg Kjør som **administrator** hvis tilgjengelig).

Hvis Teams fortsatt krasjer, kan du prøve å reprodusere problemet. Hvis du kan:

1. Bruk Trinninnspilling til å registrere trinnene.
    - Lukk ALLE unødvendige eller konfidensielle programmer.
    - Start Trinninnspilling, og reproduser problemet mens du er logget på med den berørte brukerkontoen.
    - [Samle inn teamloggene som registrerer de innspilte repro-trinnene.](https://docs.microsoft.com/microsoftteams/log-files) **Obs!** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.
    - Samle inn informasjon om dumping og/eller feilsamling (Windows). Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer (etter hver kommando trykker du ENTER):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Når tekstfilen er generert og vises på skjermen, lagrer du filen og legger den ved tjenesteforespørselen. 
