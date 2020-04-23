---
title: Løse problemer med DKIM-oppsett
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717571"
---
# <a name="fix-dkim-setup-issues"></a>Løse problemer med DKIM-oppsett

Hvis det oppstår problemer med å aktivere DKIM for det egendefinerte domenet, bruker du følgende trinn:

- De fleste installasjonsproblemer med DKIM er relatert til feil DNS-poster. Kontroller at DKIM CNAME-posten (**ikke** en TXT-post) er riktig formatert. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Når du har opprettet eller oppdatert DKIM DNS-postene dine på DNS-vertstjenesten for domenet ditt (vanligvis domeneregistratoren), venter du på at DNS-postene skal overføres.

- Hvis du ikke kan opprette DKIM DNS-postene i \<administrasjonssenteret, kan du erstatte CustomDomain\> med det egendefinerte domenet `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`(for eksempel contoso.com) og kjøre denne kommandoen i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
