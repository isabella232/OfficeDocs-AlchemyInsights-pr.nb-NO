---
title: Løse installasjonsproblemer med DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945940"
---
# <a name="fix-dkim-setup-issues"></a>Løse installasjonsproblemer med DKIM

Hvis du opplever problemer med å aktivere DKIM for det egendefinerte domenet, bruker du følgende fremgangsmåte:

- De fleste installasjonsproblemer med DKIM er relatert til feil DNS-poster. Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Når du har opprettet eller oppdatert DKIM DNS-postene hos DNS-vertstjenesten for domenet (vanligvis domeneregistratoren), venter du på at DNS-postene skal overføres.

- Hvis du ikke kan opprette DKIM DNS-postene i administrasjonssenteret, kan du erstatte med det egendefinerte domenet (for eksempel contoso.com) og kjøre denne kommandoen \<CustomDomain\> [i Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
