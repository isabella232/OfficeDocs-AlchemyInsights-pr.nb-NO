---
title: Kontrollere tilgang til fellesmapper ved hjelp av Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816749"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollere tilgang til fellesmapper ved hjelp av Outlook

Slik kontrollerer du hvilke brukere som har tilgang til fellesmapper ved hjelp av Outlook:

1. Bruk `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Gi brukere tilgang til fellesmapper i Outlook  
$false: Hindre brukertilgang til fellesmapper i Outlook. Dette er standardverdien.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Obs! Denne fremgangsmåten kan bare kontrollere tilkoblinger med Skrivebordsversjonen av Outlook for Windows-klienter. Brukere kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.

Hvis du vil ha mer informasjon, kan du se Kontrollerte tilkoblinger til [fellesmapper i Outlook](https://aka.ms/controlpf) hvis du vil ha mer informasjon.
