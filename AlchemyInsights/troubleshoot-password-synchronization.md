---
title: Feilsøke passord synkronisering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664935"
---
# <a name="troubleshoot-password-synchronization"></a>Feilsøke passord synkronisering

Hvis du vil feilsøke problemer med passord synkronisering, starter du med denne oppgaven for feil søking av AAD Connect for å fastslå hvorfor passord ikke synkroniseres. Hvis du vil begynne, kan du gå til [administrere direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren, og velg alternativet **Kjør som administrator** .

2. Kjør set-ExecutionPolicy RemoteSigned eller set-ExecutionPolicy unrestricted.

3. Start vei viseren for Azure AD Connect.

4. Gå til siden for flere aktiviteter > **Feilsøke**  >  **neste**.

5. Velg **Start** for å åpne menyen for feil søking av PowerShell.

6. Velg **Feilsøk passord synkronisering**.

    Problemet er vanligvis at et passord ikke er synkronisert for en bestemt bruker konto.

    **Notater** Passord synkronisering mislykkes hvis den siste vellykkede synkroniseringen av passord var en tid siden.

Hvis du vil ha mer informasjon om feil søking av passord, kan du se [Feilsøke passord nummer synkronisering med Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synkronisering.