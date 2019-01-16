---
title: 1065 nedgraderingen EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302951"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Nedgraderingen av EOP utgående IP-adresseområder

Vi har oppdaget et mulig problem med organisasjonen som (Hvis ikke korrigert av oktober 26th, 2018) kan bryte e-postflyt til lokale eller eksterne mål. Som tidligere formidlet for å forenkle behandling av IP-adressen området konsoliderer vi Exchange Online Protection (EOP) IP-adresseområder som brukes til å sende og motta e-post utenfor Office 365. Vår analyse viser at ett eller flere av e-post for eksterne kilder eller mål du har konfigurert i e-post flyt koblinger ikke godtar tilkoblinger fra de IP-adresse områdene vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Utføre en handling før oktober 26th å sikre disse kilder og mål skal godta tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Hvis du vil ha mer informasjon om denne endringen, kan du se Meldingssentral innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Merk**: Hvis du tidligere brukte URL-adresse eller IP-publisering via HTML, XML og RSS-oppdateringer for sluttpunktet, også bør du oppdatere til de nye web-tjenestene for å automatisere disse typene oppdateringer. Hvis du vil ha mer informasjon, kan du se [Office 365 endepunktet kategorier og Office 365-IP-adresse og URL-adressen for webtjenesten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

