---
title: Løse problemer med installasjonsprogrammet DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765263"
---
# <a name="fix-dkim-setup-issues"></a>Løse problemer med installasjonsprogrammet DKIM

Hvis du opplever problemer med å aktivere DKIM for det tilpassede domenet, kan du bruke følgende fremgangsmåte:

- De fleste DKIM-installasjonsproblemer knyttet til feil DNS-poster. Kontroller DKIM CNAME-post (**ikke** en TXT-post) er riktig formatert. Hvis du vil ha mer informasjon, se dette [emnet](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Når du oppretter eller oppdaterer DKIM DNS-postene i DNS-vertstjenesten for domenet (vanligvis domeneregistraren din), venter på DNS-poster å overføre.

- Hvis du ikke kan opprette DKIM DNS oppføringer i administrasjonssenteret, kan du erstatte \<CustomDomain\> med det tilpassede domenet (for eksempel contoso.com) og kjøre denne kommandoen i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
