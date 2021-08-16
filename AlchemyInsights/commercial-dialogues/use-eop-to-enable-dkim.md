---
title: Bruk Exchange Online PowerShell til å aktivere DKIM for et bestemt domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070318"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Bruk Exchange Online PowerShell til å aktivere DKIM for et bestemt domene

Hvis du ikke kan opprette DKIM DNS-postene i administrasjonssenteret, kan du prøve å Exchange Online PowerShell. 

Hvis du vil opprette en DKIM DNS-post Exchange Online PowerShell, utfører du følgende trinn:

1. Åpne Windows PowerShell som administrator, og kjør følgende kommandoer i den beskrevne sekvensen:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Hvis du har problemer med å koble Exchange Online PowerShell, [kan du se Koble til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Når du er koblet til Exchange Online PowerShell, kjører du følgende kommando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Når kommandoen ovenfor er utført, kjører du følgende kommando for å avslutte Exchange Online PowerShell-økten:

    `Remove-PSSession $Session` 



