---
title: Avgang ved pensjon for Access services
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359364"
---
# <a name="access-services-retirement"></a>Avgang ved pensjon for Access services

Vi opprinnelig annonsert i MC97576, i mars 2017, og fortsatte å kommunisere over det siste året er tilgang til tjenester som Pensjonert fra Office 365. Den neste fasen i denne prosessen blir fjerning av Access Web-databaser som bruker SharePoint-lister som deres underliggende datalageret.

**Hvordan påvirker det meg?**

Fra juni 2019, vil vi stoppe oppretting av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apps April 2020.

**Hva må jeg gjøre for å forberede meg for denne endringen?**

Vi oppfordrer deg til å lage en overgang plan for organisasjonens Access-databaser for web. Administratorer kan bruke [SharePoint-Access app skanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-programmer som bruker områder.

Det finnes flere måter å overføre data fra Access web databaser:

- Importerer til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også utforske Microsoft PowerApps som en alternativ plattform til å opprette løsninger uten kode business for web og mobile enheter.