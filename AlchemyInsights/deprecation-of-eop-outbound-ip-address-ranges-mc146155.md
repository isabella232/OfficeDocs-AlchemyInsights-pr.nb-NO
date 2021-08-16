---
title: 1065 Avvikling av utgående IP-adresseområder for EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031271"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Avvikling av utgående IP-adresseområder for EOP

Vi har oppdaget et potensielt problem med organisasjonen som (hvis ikke rettet innen 26. oktober 2018) kan bryte e-postflyten til dine lokale eller eksterne mål. Som tidligere kommunisert, for å forenkle administrasjon av IP-adresseområde, konsoliderer vi IP-adresseområder for Exchange Online Protection (EOP) som brukes til å sende og motta e-post utenfor Microsoft 365. Vår analyse indikerer at én eller flere av de eksterne e-postkildene eller -målene du har konfigurert i e-postflytkoblinger, ikke godtar tilkoblinger fra IP-adresseområder som vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Handle før 26. oktober for å sikre at disse kildene og destinasjonene godtar tilkoblinger til og fra alle [publiserte IP-adresser for EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Hvis du vil ha mer informasjon om denne endringen, kan du se Meldingssenter-innlegg [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Obs!** Hvis du tidligere har brukt IP- eller URL-publisering via HTML, XML og RSS for endepunktoppdateringer, bør du også overføre til de nye nettjenestene for å automatisere disse typene oppdateringer. Hvis du vil ha mer [informasjon, Microsoft 365 endepunktkategorier og Microsoft 365 IP-adresse og nettadresse-nettjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
