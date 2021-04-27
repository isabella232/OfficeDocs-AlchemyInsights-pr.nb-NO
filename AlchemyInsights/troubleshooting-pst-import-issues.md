---
title: Feilsøke problemer med PST-import
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
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059824"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="1e4d9-102">Feilsøke problemer med PST-import</span><span class="sxs-lookup"><span data-stu-id="1e4d9-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="1e4d9-103">Hvis du importerer i selve Outlook-klienten, kan du se [Løse problemer med å importere en Outlook PST-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="1e4d9-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="1e4d9-104">Hvis du bruker Importtjeneste og den står fast, må du være oppmerksom på at hver PST-fil som du laster opp til Azure Storage-plasseringen, ikke skal være større enn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="1e4d9-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="1e4d9-105">PST-filer som er større enn 20 GB, kan påvirke ytelsen til PST-importprosessen.</span><span class="sxs-lookup"><span data-stu-id="1e4d9-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="1e4d9-106">Hvis du vil ha mer informasjon om feilsøking av jobber som står fast, kan [du se Problemer som påvirker PST-importjobber](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="1e4d9-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="1e4d9-107">Hvis du vil bekrefte statusen for en bestemt importjobb, bruker du [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="1e4d9-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="1e4d9-108">Hvis du vil ha mer informasjon om importtjenesten, kan du se Oversikt over [import av organisasjonens PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1e4d9-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
