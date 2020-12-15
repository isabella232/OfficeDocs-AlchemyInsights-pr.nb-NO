---
title: Logge på Microsoft Edge manuelt
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677784"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Logge på Microsoft Edge manuelt

Hvis en bruker ikke automatisk er logget på ved første gangs kjøring, kan brukeren logge på via nett leserens innstillinger eller under meny for identitet manuelt. Hvis du vil administrere pålogging, bruker du følgende policyer:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – for å sikre at en bruker alltid har en arbeids profil i Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – for å begrense pålogging til et sett med klarerte kontoer.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – for å deaktivere pålogging eller for å tvinge brukere til å logge seg på.

