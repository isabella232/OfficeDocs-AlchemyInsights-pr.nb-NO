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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826172"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="87fdc-102">Feilsøke problemer med PST-import</span><span class="sxs-lookup"><span data-stu-id="87fdc-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="87fdc-103">Hvis du importerer i selve Outlook-klienten, kan du se [Løs problemer med import av en Outlook .pst-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="87fdc-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="87fdc-104">Hvis du bruker importtjenesten og den har stanset opp, må du være oppmerksom på at hver PST-fil som du laster opp til Azure Storage-plasseringen ikke må være større enn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="87fdc-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="87fdc-105">PST-filer som er større enn 20 GB, kan påvirke ytelsen til PST-importprosessen.</span><span class="sxs-lookup"><span data-stu-id="87fdc-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="87fdc-106">Hvis du vil kontrollere statusen for en bestemt importjobb, kan du bruke [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="87fdc-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="87fdc-107">Hvis du vil ha fullstendig informasjon om importtjenesten, kan du se [Oversikt over hvordan du importerer organisasjonens PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="87fdc-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
