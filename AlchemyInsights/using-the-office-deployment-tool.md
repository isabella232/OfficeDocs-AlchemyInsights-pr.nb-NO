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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085841"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bruke distribusjons verktøy for Office (ODT)

Du bruker distribusjons verktøy for Office (ODT) til å distribuere Office 365-versjoner av Office. Distribusjons verktøy for Office (setupodt.exe) kjøres fra kommando linjen og bruker en XML-fil for konfigurasjon til å finne ut hvilke innstillinger som skal brukes når du distribuerer Office.
  
1. Last ned den nyeste versjonen av distribusjons verktøyet for Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Bruk [tilpasnings verktøyet for Office](https://config.office.com) for å velge distribusjons innstillingene og opprette XML-filen for konfigurasjonen. Eksporter konfigurasjons filen, og plasser den lokalt i samme mappe som setupodt.exe finnes i.

    **Obs!** Problemer med Office-installasjonen forekommer vanligvis på grunn av feil kon figurerte eller malformattede konfigurasjons filer. Vi anbefaler at du bruker tilpasnings verktøyet for Office til å opprette konfigurasjons filen for å unngå slike problemer. Du kan også importere eksisterende konfigurasjons filer til tilpasnings verktøyet for Office.

3. Gå til plasseringen der setupodt.exe befinner seg i en hevet lede tekst, og Kjør distribusjons verktøyet for Office i Download Mode, og angi konfigurasjons filen du nettopp lagret. I dette eksemplet kalles konfigurasjons filen Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Kjør distribusjons verktøyet for Office i konfigurerings modus, og angi konfigurasjons filen.

```setupodt.exe /configure Configuration.xml```

**Obs!** Du må kjøre dette trinnet fra klient data maskinen du vil installere Office på, og du må ha lokale administrator tillatelser på denne data maskinen.

Hvis du vil lære mer om hvordan du bruker distribusjons verktøy for Office for Microsoft 365-appene for distribusjon av bedrifts distribusjon, kan du se [Oversikt over distribusjons verktøyet for Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Hvis du vil ha mer informasjon om hvordan du bruker tilpasnings verktøyet for Office, kan du se [Oversikt over tilpasnings verktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
