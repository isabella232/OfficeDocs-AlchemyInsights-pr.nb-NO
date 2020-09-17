---
title: Bruke distribusjons verktøy for Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794920"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bruke distribusjons verktøy for Office (ODT)

Du bruker distribusjons verktøy for Office (ODT) til å distribuere Office 365-versjoner av Office. Distribusjons verktøy for Office (setup.exe) kjøres fra kommando linjen og bruker en XML-fil for konfigurasjon til å finne ut hvilke innstillinger som skal brukes når du distribuerer Office.
  
1. Last ned den nyeste versjonen av distribusjons verktøyet for Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Bruk [tilpasnings verktøyet for Office](https://config.office.com) for å velge distribusjons innstillingene og opprette XML-filen for konfigurasjonen. Eksporter konfigurasjons filen, og plasser den lokalt i samme mappe som setup.exe finnes i.

    **Obs!** Problemer med Office-installasjonen forekommer vanligvis på grunn av feil kon figurerte eller malformattede konfigurasjons filer. Vi anbefaler at du bruker tilpasnings verktøyet for Office til å opprette konfigurasjons filen for å unngå slike problemer. Du kan også importere eksisterende konfigurasjons filer til tilpasnings verktøyet for Office.

3. Gå til plasseringen der setup.exe befinner seg i en hevet lede tekst, og Kjør distribusjons verktøyet for Office i Download Mode, og angi konfigurasjons filen du nettopp lagret. I dette eksemplet kalles konfigurasjons filen Configuration.xml:

```setup.exe /download Configuration.xml```

4. Kjør distribusjons verktøyet for Office i konfigurerings modus, og angi konfigurasjons filen.

```setup.exe /configure Configuration.xml```

**Obs!** Du må kjøre dette trinnet fra klient data maskinen du vil installere Office på, og du må ha lokale administrator tillatelser på denne data maskinen.

Hvis du vil lære mer om hvordan du bruker distribusjons verktøy for Office for Microsoft 365-appene for distribusjon av bedrifts distribusjon, kan du se [Oversikt over distribusjons verktøyet for Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Hvis du vil ha mer informasjon om hvordan du bruker tilpasnings verktøyet for Office, kan du se [Oversikt over tilpasnings verktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
