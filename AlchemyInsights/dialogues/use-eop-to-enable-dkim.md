---
title: Bruke Exchange Online PowerShell til å aktivere DKIM for et bestemt domene
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525238"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Bruke Exchange Online PowerShell til å aktivere DKIM for et bestemt domene

Hvis du ikke kan opprette DKIM DNS-postene i administrasjonssenteret, kan du prøve å bruke Exchange Online PowerShell. 

Gjør følgende for å opprette en DKIM DNS-post ved hjelp av Exchange Online PowerShell:

1. Åpne Windows PowerShell som administrator, og kjør følgende kommandoer i den beskrevne sekvensen:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Hvis du har problemer med å koble til Exchange Online PowerShell, kan du se [Koble til Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Når du er koblet til Exchange Online PowerShell, kjører du følgende kommando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Når kommandoen ovenfor er utført, kjører du følgende kommando for å avslutte Exchange Online PowerShell-økten:

    `Remove-PSSession $Session` 



