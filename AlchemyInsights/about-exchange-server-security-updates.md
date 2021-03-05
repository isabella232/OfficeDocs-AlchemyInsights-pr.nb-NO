---
title: Sikkerhetsoppdateringer for Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481949"
---
# <a name="about-exchange-server-security-updates"></a>Sikkerhetsoppdateringer for Exchange Server

Microsoft har utgitt en serie med kritiske sikkerhetsoppdateringer for Exchange Server lokalt. De berørte serverversjonene er alle oppdateringsnivåer for Exchange Server 2010, 2013, 2016 og 2019. Exchange Online påvirkes IKKE, men hvis du har noen lokale Exchange-servere på grunn av hybridkonfigurasjon, er de potensielt sårbare.

Hvis du vil oppdatere de lokale serverne, må du kjøre minst følgende versjoner av Exchange:

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 eller CU 18
- Exchange Server 2019 CU 8 eller CU 7

Se følgende kunngjøring om plasseringen av løsninger: [Utgitt: Sikkerhetsoppdateringer for Exchange Server 2021 mars 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Viktige merknader:**

Installasjon av oppdateringer vil ikke fungere hvis de lokale serverne ikke kjører nødvendige Exchange-versjoner, i henhold til listen ovenfor.

Hvis du installerer oppdateringer manuelt, kan du lese delen «Kjente problemer» i oppdatering av KB-artikler for viktig informasjon. Sikkerhetsoppdateringer MÅ kjøres fra hevet CMD/PowerShell-ledetekst!
