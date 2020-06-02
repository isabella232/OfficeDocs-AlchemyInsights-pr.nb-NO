---
title: Løs problemer med DKIM-oppsett
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506783"
---
# <a name="fix-dkim-setup-issues"></a>Løs problemer med DKIM-oppsett

Hvis det oppstår problemer med å aktivere DKIM for det egendefinerte domenet, bruker du følgende trinn:

- De fleste problemer med DKIM-installasjoner er knyttet til feil DNS-poster. Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Når du har opprettet eller oppdatert DKIM DNS-postene på DNS-vertstjenesten for domenet ditt (vanligvis domeneregistratoren), venter du på dns-postene for å overføre.

- Hvis du ikke kan opprette DKIM DNS-postene i administrasjonssenteret, kan du erstatte \<CustomDomain\> med det egendefinerte domenet (for eksempel contoso.com) og kjøre denne kommandoen i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
