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
# <a name="teams-client-crashing"></a><span data-ttu-id="764a3-102">Krasjer Teams-klienten?</span><span class="sxs-lookup"><span data-stu-id="764a3-102">Teams client crashing?</span></span>

<span data-ttu-id="764a3-103">Hvis Teams-klienten krasjer, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="764a3-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="764a3-104">Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="764a3-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="764a3-105">Kontroller at alle [Microsoft 365 URL-adresser og adresseområder er tilgjengelige.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="764a3-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="764a3-106">Logg inn med leieradministratorkontoen din, og sjekk instrumentbordet for [tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for å bekrefte at det ikke finnes noe nedetid eller tjenesteforringelse.</span><span class="sxs-lookup"><span data-stu-id="764a3-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="764a3-107">Avinstallere og installere Teams-programmet på nytt (link)</span><span class="sxs-lookup"><span data-stu-id="764a3-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="764a3-108">Bla til mappen %appdata%\Microsoft\teams\ på datamaskinen, og slett alle filene i den mappen.</span><span class="sxs-lookup"><span data-stu-id="764a3-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="764a3-109">[Last ned og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer om mulig Teams som administrator (høyreklikk på Teams-installasjonsprogrammet og velg "Kjør som administrator" hvis tilgjengelig).</span><span class="sxs-lookup"><span data-stu-id="764a3-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="764a3-110">Hvis Teams-klienten din fortsatt krasjer, kan du gjenskape problemet?</span><span class="sxs-lookup"><span data-stu-id="764a3-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="764a3-111">I så fall:</span><span class="sxs-lookup"><span data-stu-id="764a3-111">If so:</span></span>

1. <span data-ttu-id="764a3-112">Bruk trinnopptakeren til å ta opp trinnene.</span><span class="sxs-lookup"><span data-stu-id="764a3-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="764a3-113">Lukk alle unødvendige eller konfidensielle applikasjoner.</span><span class="sxs-lookup"><span data-stu-id="764a3-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="764a3-114">Start steps recorder og reprodusere problemet mens du er logget inn med den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="764a3-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="764a3-115">[Samle teamloggene som fanger opp de registrerte reprotrinnene](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="764a3-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="764a3-116">**Merk:** Kontroller at du registrerer påloggingsadressen til den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="764a3-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="764a3-117">Samle dump og / eller Feil bøtte info (Windows).</span><span class="sxs-lookup"><span data-stu-id="764a3-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="764a3-118">Start Windows Powershell på maskinen der krasjet oppstår, og kjør følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="764a3-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="764a3-119">Legg ved filen i støttesaken.</span><span class="sxs-lookup"><span data-stu-id="764a3-119">Attach the file to your support case.</span></span>
