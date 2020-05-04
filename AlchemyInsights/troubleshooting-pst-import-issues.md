---
title: Feilsøke problemer med PST-import
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991376"
---
# <a name="troubleshooting-pst-import-issues"></a>Feilsøke problemer med PST-import

- Hvis du importerer i selve Outlook-klienten, kan du se [Løs problemer med import av en Outlook .pst-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Hvis du bruker importtjenesten og den har stanset opp, må du være oppmerksom på at hver PST-fil som du laster opp til Azure Storage-plasseringen ikke må være større enn 20 GB. PST-filer som er større enn 20 GB, kan påvirke ytelsen til PST-importprosessen.

- Hvis du vil kontrollere statusen for en bestemt importjobb, kan du bruke [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Hvis du vil ha fullstendig informasjon om importtjenesten, kan du se [Oversikt over hvordan du importerer organisasjonens PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
