---
title: 1065 nedgraderingen EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934893"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Nedgraderingen av EOP utgående IP-adresseområder

Vi har oppdaget et mulig problem med organisasjonen som (Hvis ikke korrigert av oktober 26th, 2018) kan bryte e-postflyt til lokale eller eksterne mål. Som tidligere formidlet for å forenkle behandling av IP-adressen området konsoliderer vi Exchange Online Protection (EOP) IP-adresseområder som brukes til å sende og motta e-post utenfor Office 365. Vår analyse viser at ett eller flere av e-post for eksterne kilder eller mål du har konfigurert i e-post flyt koblinger ikke godtar tilkoblinger fra de IP-adresse områdene vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Utføre en handling før oktober 26th å sikre disse kilder og mål skal godta tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Hvis du vil ha mer informasjon om denne endringen, kan du se Meldingssentral innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Merk**: Hvis du tidligere brukte URL-adresse eller IP-publisering via HTML, XML og RSS-oppdateringer for sluttpunktet, også bør du oppdatere til de nye web-tjenestene for å automatisere disse typene oppdateringer. Hvis du vil ha mer informasjon, kan du se [Office 365 endepunktet kategorier og Office 365-IP-adresse og URL-adressen for webtjenesten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

