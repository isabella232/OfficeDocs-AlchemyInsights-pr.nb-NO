---
title: Slik deaktiverer du eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704137"
---
# <a name="how-to-disable-external-groups"></a>Slik deaktiverer du eksterne grupper

Eksterne Yammer-meldinger bruker Exchange-transportprotokoller (etr), et sett med proaktiverte kontroller for å hindre at firma informasjon deles. Hvis du vil begrense brukere fra å opprette eksterne grupper, må du konfigurere en Exchange transport regel (ETR) og deretter konfigurere Yammer til å bruke Exchange-transport regelen til å blokkere eksterne meldinger.
  
Når du har opprettet en regel i administrasjons senteret for Exchange Online, følger du denne Fremgangs måten for å angi ETR som skal brukes i Yammer:
  
- Logg på Yammer som en bekreftet administrator, og i **administrasjons senteret for Yammer**går du til C **innhold og sikkerhets \> Innstillinger** for sikkerhet.

- Velg **Gjennomfør Exchange Online Exchange-transporttilbyderen (etr) i Yammer** under **eksterne meldinger**.

- Velg **Lagre**.

Hvis du vil ha mer informasjon, kan du se [deaktivere eksterne meldinger i et Yammer-nettverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  