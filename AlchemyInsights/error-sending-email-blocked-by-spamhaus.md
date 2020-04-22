---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714267"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Feil under sending av e-post: Klientverten blokkert ved hjelp av Spamhaus

IP-adressen som sendte meldingen, finnes i en blokkeringsliste som eies av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Årsaker til å bli blokkert av Spamhaus inkluderer kompromitterte kontoer, kompromitterte maskiner som deler en offentlig IP-adresse og Internett-leverandørpolicyer (IsP). Mulige reparasjoner er:
  
- For blokkerte innkommende meldinger der du kontrollerer kildens e-postserver, må du finne årsaken og fjerne blokken fra Spamhaus-nettstedet.

- For blokkerte innkommende meldinger der kilde-IP-adressen tilhører noen andre, må adresseeieren fjerne blokken fra Spamhaus-nettstedet. Hvis IP-adressen er på policyblokklisten (PBL), kan eieren tilordne en annen statisk IP-adresse eller fjerne adressen fra PBL.

- For blokkerte utgående meldinger fra domenet som er koblet til Microsoft, kan du få denne feilmeldingen hvis meldingene rutes gjennom en tredjepartstjeneste. Du kan bruke et WHOIS-oppslagsverktøy til å finne eieren av den blokkerte IP-adressen.
