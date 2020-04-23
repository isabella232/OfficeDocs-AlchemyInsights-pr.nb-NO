---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720777"
---
# <a name="how-to-disable-external-groups"></a>Slik deaktiverer du eksterne grupper

Yammer eksterne meldinger bruker Exchange Transport Rules (ETRs), et sett med proaktive kontroller for å hindre at firmainformasjon deles. Hvis du vil begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transportregel (ETR), og deretter konfigurere Yammer til å bruke Exchange Transport-regelen til å blokkere eksterne meldinger.
  
Når du har opprettet en regel i administrasjonssenteret for Exchange Online, følger du denne fremgangsmåten for å angi at ETR skal brukes i Yammer:
  
- Logg på Yammer som en bekreftet administrator, og gå til **C-innstillinger for \> innholds- og sikkerhetssikkerhet** i **Yammer.**

- Under **Eksterne meldinger**velger du **Fremhev Exchange Online Exchange Transport Rules (ETRs) i Yammer.**

- Velg **Lagre**.

Hvis du vil ha mer informasjon, kan du se [Deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  