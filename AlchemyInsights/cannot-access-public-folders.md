---
title: Får ikke tilgang til felles mapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341412"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke koble til felles mapper

Hvis tilgang til felles mapper ikke fungerer for enkelte brukere, kan du prøve følgende:

Koble deg til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox-parameteren på problem bruker kontoen for å samsvare med parameteren på en arbeids bruker konto.

Eksempel

Hent post boks WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-post boks ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Vent minst én time før endringen trer i kraft.

Hvis problemet fortsetter, kan du følge [denne Fremgangs måten](https://aka.ms/pfcte) for å feilsøke problemer med tilgang til felles mapper ved hjelp av Outlook.
 
**Slik styrer du hvilke brukere som har tilgang til felles mapper ved hjelp av Outlook**:

1.  Bruke Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $FALSE  
      
    $true: gi brukere tilgang til felles mapper i Outlook  
      
    $false: hindre bruker tilgang til felles mapper i Outlook. Dette er standardverdien.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Obs!** Denne Fremgangs måten kan bare kontrollere tilkoblinger med skrive bords versjonen av Outlook for Windows-klienter. En bruker kan fortsette å få tilgang til felles mapper ved hjelp av OWA eller Outlook for Mac.
 
Hvis du vil ha mer informasjon, kan du se [kunngjørings støtte for kontrollerte tilkoblinger til felles mapper i Outlook](https://aka.ms/controlpf).