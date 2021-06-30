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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187730"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="5c7eb-102">Teams klient krasjer</span><span class="sxs-lookup"><span data-stu-id="5c7eb-102">Teams client crashing</span></span>

<span data-ttu-id="5c7eb-103">Hvis Teams-klienten krasjer, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="5c7eb-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="5c7eb-104">Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="5c7eb-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="5c7eb-105">Kontroller at alle [Microsoft 365 nettadresser og adresseområder](/microsoftteams/connectivity-issues) er tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="5c7eb-106">Logg på med administratorkontoen for [](/office365/enterprise/view-service-health) leieren, og kontroller instrumentbordet for tjenestetilstand for å bekrefte at det ikke finnes noen avbrudd eller tjenesteforringelse.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="5c7eb-107">Avinstallere og installere Teams-programmet på nytt</span><span class="sxs-lookup"><span data-stu-id="5c7eb-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="5c7eb-108">Bla til mappen %appdata%\Microsoft\Teams\ på datamaskinen, og slett alle filene i denne katalogen.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="5c7eb-109">Last ned og installer [Teams-appen](https://www.microsoft.com/microsoft-teams/download-app), og installer om mulig Teams som administrator (høyreklikk installasjonsprogrammet Teams, og velg Kjør som **administrator** hvis tilgjengelig).</span><span class="sxs-lookup"><span data-stu-id="5c7eb-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="5c7eb-110">Hvis Teams fortsatt krasjer, kan du prøve å reprodusere problemet.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="5c7eb-111">Hvis du kan:</span><span class="sxs-lookup"><span data-stu-id="5c7eb-111">If you can:</span></span>

1. <span data-ttu-id="5c7eb-112">Bruk Trinninnspilling til å registrere trinnene.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="5c7eb-113">Lukk ALLE unødvendige eller konfidensielle programmer.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="5c7eb-114">Start Trinninnspilling, og reproduser problemet mens du er logget på med den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="5c7eb-115">[Samle inn teamloggene som registrerer de innspilte repro-trinnene.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="5c7eb-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="5c7eb-116">**Obs!** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="5c7eb-117">Samle inn informasjon om dumping og/eller feilsamling (Windows).</span><span class="sxs-lookup"><span data-stu-id="5c7eb-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="5c7eb-118">Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer (etter hver kommando trykker du ENTER):</span><span class="sxs-lookup"><span data-stu-id="5c7eb-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="5c7eb-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="5c7eb-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="5c7eb-120">Når tekstfilen er generert og vises på skjermen, lagrer du filen og legger den ved tjenesteforespørselen.</span><span class="sxs-lookup"><span data-stu-id="5c7eb-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
