---
title: Avvikling av enkel godkjenning i Exchange PowerShell
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069253"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Avvikling av enkel godkjenning i Exchange PowerShell

Hvis du vil ha mer informasjon om hvordan du kobler til Exchange Online PowerShell uten å bruke enkel godkjenning, [kan du gå hit](https://aka.ms/exops-docs). PowerShell V2-modulen bruker ikke enkel godkjenning.

Vær oppmerksom på at enkel godkjenning fremdeles må aktiveres på klientdatamaskinen.
Den nye PowerShell V2-modulen bruker moderne godkjenning for å opprette en kobling for å aktivere alle REST-baserte V2-cmdleter. I tillegg til V2-cmdlet-er kan du også få tilgang til eldre eksterne PowerShell-cmdleter (RPS) som krever opprettelse av en ekstern PowerShell-økt. Hvis du vil opprette en RPS-økt på Windows-maskinen, må WinRM BasicAuth være aktivert på klientmaskinen, selv om modulen bruker moderne godkjenning-mekanisme til å godkjenne til tjenesten. Samlebåndet for enkel WinRM-godkjenning brukes til å transportere moderne godkjenningstokener. Hvis enkel WinRM-godkjenning deaktiveres på klientdatamaskinen, vil nye V2-cmdlet-er fortsette å fungere (men de eldre RPS-cmdletene vil ikke gjøre det).
