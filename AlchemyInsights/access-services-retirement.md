---
title: Pensjonering av tilgangstjenester
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938704"
---
# <a name="access-services-retirement"></a>Pensjonering av tilgangstjenester

Som vi opprinnelig kunngjorde i MC97576, i mars 2017, og fortsatte å kommunisere det siste året Access Services avvikles. Den neste fasen i denne prosessen vil være fjerning av Access Web Databases som bruker SharePoint lister som underliggende datalagring.

**Hvordan påvirker dette meg?**

Fra og med juni 2019 slutter vi å opprette nye Access-databaser i SharePoint Online og avslutter tjenesten og eventuelle gjenværende apper innen april 2020.

**Hva må jeg gjøre for å klargjøre denne endringen?**

Vi oppfordrer deg til å opprette en overgangsplan for organisasjonens Access-nettdatabaser. Administratorer kan bruke SharePoint [Access-appskanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som nettstedene bruker.

Det finnes flere måter å overføre data for Access-nettdatabaser på:

- Importere til en lokal Access-database (. ACCDB) eller til en Excel fil.
- Vi anbefaler også å utforske Microsoft PowerApps som en alternativ plattform for å opprette bedriftsløsninger uten kode for nett- og mobilenheter.