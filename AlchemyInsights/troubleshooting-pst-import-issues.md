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
# <a name="troubleshooting-pst-import-issues"></a>Feilsøke problemer med PST-import

- Hvis du importerer i selve Outlook-klienten, kan du se [Løse problemer med å importere en Outlook PST-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Hvis du bruker Importtjeneste og den står fast, må du være oppmerksom på at hver PST-fil som du laster opp til Azure Storage-plasseringen, ikke skal være større enn 20 GB. PST-filer som er større enn 20 GB, kan påvirke ytelsen til PST-importprosessen. Hvis du vil ha mer informasjon om feilsøking av jobber som står fast, kan [du se Problemer som påvirker PST-importjobber](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Hvis du vil bekrefte statusen for en bestemt importjobb, bruker du [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Hvis du vil ha mer informasjon om importtjenesten, kan du se Oversikt over [import av organisasjonens PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
