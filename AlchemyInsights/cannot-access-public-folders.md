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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996639"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke koble til fellesmapper

Hvis tilgang til fellesmapper ikke fungerer for enkelte brukere, kan du prøve følgende:

Koble til til EXO PowerShell og konfigurere DefaultPublicFolderMailbox-parameteren på den problematiske brukerkontoen slik at den samsvarer med parameteren på en fungerende brukerkonto.

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
      
**Obs!** Denne fremgangsmåten kan bare kontrollere tilkoblinger med Outlook skrivebord for Windows klienter. En bruker kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.
 
Hvis du vil ha mer informasjon, kan du se Annonsere støtte for kontrollerte tilkoblinger til [fellesmapper i Outlook](https://aka.ms/controlpf).