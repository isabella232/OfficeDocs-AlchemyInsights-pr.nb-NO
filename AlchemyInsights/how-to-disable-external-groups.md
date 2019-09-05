---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739502"
---
# <a name="how-to-disable-external-groups"></a>Slik deaktiverer du eksterne grupper

Yammer eksterne meldinger bruker Exchange transport Rules (ETRs), et sett med proaktive kontroller for å hindre at firmainformasjon blir delt. For å begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transport-regel (ETR), og deretter konfigurere Yammer til å bruke Exchange transport-regelen til å blokkere eksterne meldinger.
  
Når du har opprettet en regel i Exchange Online administrasjonssenteret, følger du denne fremgangsmåten for å angi ETR skal brukes i Yammer:
  
- Logg på Yammer som en verifisert admin, og i **administrasjonssenteret for Yammer**, gå til C- **innhold og sikkerhets \> innstillinger for sikkerhet.**

- Under **eksterne meldinger**velger **du Gjennomfør Exchange Online Exchange transport Rules (ETRs) i Yammer.**

- Velg **Lagre**.

Hvis du vil ha mer informasjon, kan du se [deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  