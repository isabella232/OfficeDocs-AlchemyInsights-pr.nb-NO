---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387858"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Feil under sending av e-post: klient-vert som er blokkert ved hjelp av Spamhaus

IP-adressen som sendte meldingen, er på en blokkeringsliste som eies av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). For blir blokkert av Spamhaus årsaker utsatt kontoer utsatt maskiner som deler en offentlig IP-adresse og retningslinjer for Internett-leverandør (ISP). Det er mulig reparasjoner:
  
- Du må finne årsaken og fjerne blokkeringen fra webområdet Spamhaus for blokkerte innkommende meldinger til Office 365 der du kan kontrollere e-kildeserveren.

- For blokkerte innkommende meldinger til Office 365 der kildens IP-adresse tilhører noen andre, må eieren av adressen du kan fjerne blokkeringen fra webområdet Spamhaus. Hvis IP-adressen på policyen Block liste (PBL), kan eieren tilordner en annen statisk IP-adresse eller fjerne adressen fra PBL.

- For blokkerte utgående meldinger fra Office 365-domenet, kan du få denne feilmeldingen hvis meldingene rutes via en 3 part. Du kan bruke et verktøy for WHOIS-oppslag til å finne den blokkerte IP-adresse eieren.
