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
# <a name="teams-client-crashing"></a><span data-ttu-id="35f43-102">Krasjer Teams-klienten?</span><span class="sxs-lookup"><span data-stu-id="35f43-102">Teams client crashing?</span></span>

<span data-ttu-id="35f43-103">Hvis Teams-klienten krasjer, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="35f43-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="35f43-104">Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="35f43-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="35f43-105">Kontroller at alle Nettadresser og adresseområder for [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="35f43-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="35f43-106">Logg på med administratorkontoen for [](https://docs.microsoft.com/office365/enterprise/view-service-health) leieren, og kontroller instrumentbordet for tjenestetilstand for å bekrefte at det ikke finnes noen avbrudd eller tjenesteforringelse.</span><span class="sxs-lookup"><span data-stu-id="35f43-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="35f43-107">Avinstallere og installere Teams-programmet på nytt (kobling)</span><span class="sxs-lookup"><span data-stu-id="35f43-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="35f43-108">Bla til mappen %appdata%\Microsoft\teams\ på datamaskinen, og slett alle filene i denne katalogen.</span><span class="sxs-lookup"><span data-stu-id="35f43-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="35f43-109">[Last ned og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer om mulig Teams som administrator (høyreklikk på Teams-installasjonsprogrammet, og velg Kjør som administrator hvis tilgjengelig).</span><span class="sxs-lookup"><span data-stu-id="35f43-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="35f43-110">Hvis Teams-klienten fremdeles krasjer, kan du reprodusere problemet?</span><span class="sxs-lookup"><span data-stu-id="35f43-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="35f43-111">Hvis det er det:</span><span class="sxs-lookup"><span data-stu-id="35f43-111">If so:</span></span>

1. <span data-ttu-id="35f43-112">Bruk Trinninnspilling til å registrere trinnene.</span><span class="sxs-lookup"><span data-stu-id="35f43-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="35f43-113">Lukk ALLE unødvendige eller konfidensielle programmer.</span><span class="sxs-lookup"><span data-stu-id="35f43-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="35f43-114">Start Trinninnspilling, og reproduser problemet mens du er logget på med den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="35f43-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="35f43-115">[Samle inn teamloggene som registrerer de innspilte repro-trinnene.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="35f43-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="35f43-116">**Obs!** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="35f43-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="35f43-117">Samle inn informasjon om dumping og/eller feilsamling (Windows).</span><span class="sxs-lookup"><span data-stu-id="35f43-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="35f43-118">Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="35f43-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="35f43-119">Legg ved filen i støttesaken.</span><span class="sxs-lookup"><span data-stu-id="35f43-119">Attach the file to your support case.</span></span>
