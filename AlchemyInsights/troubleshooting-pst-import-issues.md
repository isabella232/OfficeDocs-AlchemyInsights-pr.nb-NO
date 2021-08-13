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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972428"
---
# <a name="troubleshooting-pst-import-issues"></a>Feilsøke problemer med PST-import

- Hvis du importerer i selve Outlook-klienten, kan du se Løse problemer med å importere en [Outlook PST-fil](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Hvis du bruker Importtjeneste og den står fast, må du være oppmerksom på at hver PST-fil som du laster opp Azure Storage plasseringen, ikke skal være større enn 20 GB. PST-filer som er større enn 20 GB, kan påvirke ytelsen til PST-importprosessen. Hvis du vil ha mer informasjon om feilsøking av jobber som står fast, kan [du se Problemer som påvirker PST-importjobber](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Hvis du vil bekrefte statusen for en bestemt importjobb, bruker du [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Hvis du vil ha mer informasjon om importtjenesten, kan du se Oversikt over [import av organisasjonens PST-filer](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
