---
title: Feilsøke synkronisering av passord
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387886"
---
# <a name="troubleshoot-password-synchronization"></a>Feilsøke synkronisering av passord

Hvis du vil feilsøke problemer med synkronisering av passord, starter du ved hjelp av denne feilsøkingsoppgaven for AAD Connect for å finne ut hvorfor passord ikke synkroniseres. Du begynner ved å gå til [Behandle direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren, og velg alternativet **Kjør som administrator.**

2. Kjør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Ubegrenset.

3. Start azure AD Connect-veiviseren.

4. Gå til siden Flere oppgaver > **Feilsøke**  >  **neste**.

5. Velg **Start** for å åpne feilsøkingsmenyen for PowerShell.

6. Velg **Feilsøke synkronisering av passord**.

    Problemet er vanligvis at et passord ikke synkroniseres for en bestemt brukerkonto.

    **Notater** Synkronisering av passord mislykkes hvis den siste vellykkede synkroniseringen av passord var for en tid siden.

Hvis du vil ha mer hjelp med feilsøking av synkronisering av passord, kan du se [Feilsøke synkronisering av passordhash med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).