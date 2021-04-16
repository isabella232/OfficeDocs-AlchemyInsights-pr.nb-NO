---
title: Kryptering med transportregler
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813877"
---
# <a name="encryption-with-transport-rules"></a>Kryptering med transportregler

I [administrasjonssenteret for Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) kan du bruke funksjoner for Office-meldingskryptering (OME) i e-postflytreglene dine for å utløse meldingskryptering. Velg alternativet **Bruk Office 365-meldingskryptering og rettighetsbeskyttelse** i Transportregel-betingelsen.

- Hvis du vil ha mer informasjon, kan du se [Definere regel for postflyt for å kryptere](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- I PowerShell bruker du [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities)-cmdleten og setter *ApplyOME*-parameteren til $true.
