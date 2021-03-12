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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749982"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Angi ClientAccessServerEnabled til True

Hvis du ikke kan åpne en kryptert e-postmelding og i stedet ser et **rpmsg-vedlegg,** utfører du følgende trinn:

1. Koble til Exchange Online PowerShell.

> [!NOTE]
> Hvis du vil koble til Exchange Online PowerShell, må du logge på med en global administrator- eller Exchange-administratorkonto.

   a. Åpne Windows PowerShell, og kjør deretter følgende kommando: `$UserCredential = Get-Credential`
b. Skriv inn jobb- eller skolekontoen og passordet ditt i dialogboksen Legitimasjonsforespørsel for **Windows PowerShell,** c. Klikk **OK**. 

2. Kjør følgende kommando for å opprette en ny økt:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Kjør følgende kommando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kjør `Get-IRMConfiguration` kommando.

4. Kontroller **ClientAccessServerEnabled-innstillingen.** 

    a. Hvis **ClientAccessServerEnabled-innstillingen** er satt til **False**, kjører du følgende cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Lukk alltid PowerShell-økten med følgende kommando: `Remove-PSSession $Session`

Hvis du vil ha mer informasjon, kan du [se Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

