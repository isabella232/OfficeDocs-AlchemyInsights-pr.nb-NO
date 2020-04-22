---
title: Tilgang til pensjonering av tjenester
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687267"
---
# <a name="access-services-retirement"></a>Tilgang til pensjonering av tjenester

Som vi opprinnelig annonserte i MC97576, i mars 2017, og fortsatte å kommunisere i løpet av det siste året Access Services blir pensjonert. Den neste fasen i denne prosessen vil være fjerning av Access Web-databaser som bruker SharePoint-lister som underliggende datalagring.

**Hvordan påvirker dette meg?**

Fra juni 2019 vil vi stoppe opprettingen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apper innen april 2020.

**Hva må jeg gjøre for å forberede meg til denne endringen?**

Vi oppfordrer deg til å opprette en overgangsplan for organisasjonens Access-webdatabaser. Administratorer kan bruke [SharePoint Access-appskanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som nettsteder bruker.

Du kan overføre data for Access-webdatabaser på flere måter:

- Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også å utforske Microsoft PowerApps som en alternativ plattform for å opprette no-code forretningsløsninger for web og mobile enheter.