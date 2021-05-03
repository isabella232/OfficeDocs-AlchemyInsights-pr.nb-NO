---
title: Feilsøking av importtjenestejobben sitter fast
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125488"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Feilsøking av importtjenestejobben sitter fast

Hvis du har problemer med å importere tjenestejobber som står fast eller mislykkes, kan du undersøke og prøve følgende:

- Se gjennom størrelsen på PST-filen. Den maksimale anbefalte størrelsen på en PST-fil for import er 20 GB.

- Hvis du mistenker at elementer er hoppet over på grunn av korrupsjon, kjører du Scanpst.exe å diagnostisere og rette feil i PST-filer.

- Hvis du ser feilmeldingen «MapiExceptionShutoffQuotaExceeded» under importen, må du kontrollere at målpostboksen har tilstrekkelig kapasitet til å importere de ønskede PST-filene.

Hvis du vil ha mer informasjon om feilsøking av problemer med PST-importjobber, kan du se [Feilsøke problemer med PST-importjobber](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Hvis du vil ha informasjon om hvordan du løser problemer når du importerer PSTer til Outlook, kan du se Løse problemer med å importere en [Outlook PST-fil (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)