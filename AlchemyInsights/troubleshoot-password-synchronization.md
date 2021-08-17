---
title: Feilsøke passordsynkronisering
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105765"
---
# <a name="troubleshoot-password-synchronization"></a>Feilsøke passordsynkronisering

Hvis du vil feilsøke problemer med passordsynkronisering, kan du begynne med å bruke denne AAD-Koble til feilsøkingsoppgaven for å finne ut hvorfor passord ikke synkroniseres. Hvis du vil begynne, går du [til Administrer direkte synkronisering](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Åpne en ny Windows PowerShell økt på Azure AD Koble til-serveren, og velg alternativet **Kjør som administrator.**

2. Kjør Set-ExecutionPolicy RemoteSigned eller Set-ExecutionPolicy Unrestricted.

3. Start Azure AD Koble til-veiviseren.

4. Gå til Flere oppgaver-siden > **Feilsøk**  >  **neste**.

5. Velg **Start** for å åpne feilsøkingsmenyen for PowerShell.

6. Velg **Feilsøk passordsynkronisering**.

    Problemet er vanligvis at et passord ikke synkroniseres for en bestemt brukerkonto.

    **Notater** Passordsynkronisering mislykkes hvis den siste vellykkede passordsynkroniseringen var for en tid siden.

Hvis du vil ha mer hjelp til å feilsøke synkronisering av passord, kan du se Feilsøke synkronisering av hash for [passord med Azure AD Koble til synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)