---
title: Avvikling av enkel godkjenning i Exchange PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015698"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Avvikling av enkel godkjenning i Exchange PowerShell

Hvis du vil ha mer informasjon om hvordan du kobler til Exchange Online PowerShell uten å bruke enkel godkjenning, [kan du gå hit](https://aka.ms/psbasicauth).

Vær oppmerksom på at enkel godkjenning fremdeles må aktiveres på klientdatamaskinen.
Den nye PowerShell V2-modulen bruker moderne godkjenning for å opprette en kobling for å aktivere alle REST-baserte V2-cmdleter. I tillegg til V2-cmdlet-er kan du også få tilgang til eldre eksterne PowerShell-cmdleter (RPS) som krever opprettelse av en ekstern PowerShell-økt. Hvis du vil opprette en RPS-økt på Windows-maskinen, må WinRM BasicAuth være aktivert på klientmaskinen, selv om modulen bruker moderne godkjenning-mekanisme til å godkjenne til tjenesten. Samlebåndet for enkel WinRM-godkjenning brukes til å transportere moderne godkjenningstokener. Hvis enkel WinRM-godkjenning deaktiveres på klientdatamaskinen, vil nye V2-cmdlet-er fortsette å fungere (men de eldre RPS-cmdletene vil ikke gjøre det).
