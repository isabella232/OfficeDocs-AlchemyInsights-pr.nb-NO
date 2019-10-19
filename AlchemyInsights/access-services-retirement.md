---
title: Avgang av tilgang til tjenester
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747793"
---
# <a name="access-services-retirement"></a>Avgang av tilgang til tjenester

Som vi opprinnelig annonsert i MC97576, i mars 2017, og fortsatte å kommunisere det siste året Access Services blir pensjonert fra Office 365. Den neste fasen i denne prosessen vil være fjerning av Access Web databaser som bruker SharePoint-lister som underliggende datalagring.

**Hvordan påvirker dette meg?**

Starter juni 2019, vil vi stoppe opprettelsen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende programmer innen april 2020.

**Hva må jeg gjøre for å forberede meg på denne endringen?**

Vi oppfordrer deg til å opprette en overgangsplan for organisasjonens Access Web databaser. Administratorer kan bruke [program skanneren for SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som områdene bruker.

Det er flere måter å overføre Access Web databaser data:

- Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også at du utforsker Microsoft PowerApps som en alternativ plattform for å opprette forretningsløsninger uten kode for nett-og mobilenheter.