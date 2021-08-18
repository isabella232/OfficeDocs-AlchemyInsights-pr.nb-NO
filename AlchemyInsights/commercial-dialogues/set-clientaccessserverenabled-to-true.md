---
title: Angi ClientAccessServerEnabled til True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320365"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Angi ClientAccessServerEnabled til True

Hvis du ikke kan åpne en kryptert e-postmelding og i stedet ser et **rpmsg-vedlegg,** utfører du følgende trinn:

1. Koble til å Exchange Online PowerShell.

    **Obs!** Hvis du vil koble Exchange Online PowerShell, må du logge på med en global administrator eller Exchange administratorkonto.

   a. Åpne Windows PowerShell, og kjør deretter følgende kommando:`$UserCredential = Get-Credential`
   b. I dialogboksen **Windows PowerShell legitimasjonsforespørsel** skriver du inn jobb- eller skolekontoen og passordet, c. Klikk **OK**. 

2. Kjør følgende kommando for å opprette en ny økt:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Utfør denne kommandoen:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kjør `Get-IRMConfiguration` kommando.

4. Kontroller **ClientAccessServerEnabled-innstillingen.** 

    a. Hvis **ClientAccessServerEnabled-innstillingen** er satt til **False**, kjører du følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tips:** Lukk alltid PowerShell-økten med følgende kommando: `Remove-PSSession $Session`

Hvis du vil ha mer informasjon, [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

