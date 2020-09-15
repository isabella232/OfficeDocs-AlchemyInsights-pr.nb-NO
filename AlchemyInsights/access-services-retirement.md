---
title: Pensjon for tilgangs tjenester
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698691"
---
# <a name="access-services-retirement"></a>Pensjon for tilgangs tjenester

Som det opprinnelig ble kunngjort i MC97576, i mars 2017, og fortsetter å kommunisere over det siste året Access Services blir trukket tilbake. Den neste fasen i denne prosessen vil være fjerning av Access-webdatabaser som bruker SharePoint-lister som underliggende data lagring.

**Hvordan påvirker dette meg?**

Fra og med juni 2019 vil vi stoppe opprettelsen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apper etter april 2020.

**Hva må jeg gjøre for å klargjøre for denne endringen?**

Vi oppfordrer deg til å opprette en overgangs plan for organisasjonens web databaser for tilgang. Administratorer kan bruke [SharePoint Access app-skanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som nett steder bruker.

Det finnes flere måter å overføre data i Access Web databaser på:

- Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.
- Vi anbefaler også å utforske Microsoft PowerApps som en alternativ plattform for å opprette gratis bedrifts løsninger for nett og mobile enheter.