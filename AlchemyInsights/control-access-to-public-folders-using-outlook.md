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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032567"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollere tilgang til fellesmapper ved hjelp av Outlook

Slik kontrollerer du hvilke brukere som har tilgang til fellesmapper ved hjelp av Outlook:

1. Bruk `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Gi brukere tilgang til fellesmapper i Outlook  
$false: Hindre brukertilgang til fellesmapper i Outlook. Dette er standardverdien.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Obs! Denne fremgangsmåten kan bare kontrollere tilkoblinger Outlook skrivebord for Windows klienter. Brukere kan fortsette å få tilgang til fellesmapper ved hjelp av OWA eller Outlook for Mac.

Hvis du vil ha mer informasjon, kan du se Kontrollerte tilkoblinger til [fellesmapper i Outlook](https://aka.ms/controlpf) for mer informasjon.
