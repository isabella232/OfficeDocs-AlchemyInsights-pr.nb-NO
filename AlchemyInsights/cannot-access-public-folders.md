---
title: Får ikke tilgang til fellesmapper
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819521"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke koble til fellesmapper

Hvis tilgang til fellesmapper ikke fungerer for enkelte brukere, kan du prøve følgende:

Koble til EXO PowerShell, og konfigurer DefaultPublicFolderMailbox-parameteren på den problematiske brukerkontoen slik at den samsvarer med parameteren på en fungerende brukerkonto.

Eksempel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Vent minst én time før endringen trer i kraft.

Hvis problemet forblir, følger du [denne](https://aka.ms/pfcte) fremgangsmåten for å feilsøke problemer med tilgang til fellesmapper ved hjelp av Outlook.
 
**Slik kontrollerer du hvilke brukere som har tilgang til fellesmapper ved hjelp av Outlook:**

1.  Bruk Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Gi brukere tilgang til fellesmapper i Outlook  
      
    $false: Hindre brukertilgang til fellesmapper i Outlook. Dette er standardverdien.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Obs!** Denne fremgangsmåten kan bare kontrollere tilkoblinger med Outlook-skrivebord for Windows-klienter. En bruker kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.
 
Hvis du vil ha mer informasjon, kan du [se Annonsere støtte for kontrollerte tilkoblinger til fellesmapper i Outlook](https://aka.ms/controlpf).