---
title: Bruke Office distribusjonsverktøyet
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083779"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bruke Office distribusjonsverktøyet (ODT)

Du bruker distribusjonsverktøyet Office (ODT) til å distribuere Office 365 versjoner av Office. Distribusjonsverktøyet Office (setup.exe) kjøres fra kommandolinjen og bruker en XML-konfigurasjonsfil til å bestemme hvilke innstillinger som skal brukes når du distribuerer Office.
  
1. Last ned den nyeste versjonen av Office distribusjonsverktøyet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Bruk [tilpasningsverktøyet Office (OCT)](https://config.office.com) til å velge distribusjonsinnstillingene og opprette xml-konfigurasjonsfilen. Eksporter konfigurasjonsfilen, og plasser den lokalt i den samme mappen der setup.exe befinner seg.

    **Merk:** Office vanligvis oppstår på grunn av feilkonfigurerte eller feilformaterte konfigurasjonsfiler. For å unngå slike problemer anbefaler vi at du bruker tilpasningsverktøyet Office til å opprette konfigurasjonsfilen. Du kan også importere eksisterende konfigurasjonsfiler til tilpasningsverktøyet Office.

3. Bytt fra en hevet ledetekst til plasseringen der setup.exe befinner seg, og kjør distribusjonsverktøyet Office i nedlastingsmodus, og angi konfigurasjonsfilen du nettopp lagret. I dette eksemplet heter konfigurasjonsfilen Configuration.xml:

```setup.exe /download Configuration.xml```

4.Kjør Office distribusjonsverktøyet i konfigureringsmodus, og angi konfigurasjonsfilen.

```setup.exe /configure Configuration.xml```

**Obs!** Du må kjøre dette trinnet fra klientdatamaskinen du vil installere Office, og du må ha lokale administratortillatelser på denne datamaskinen.

Hvis du vil lære mer om Office distribusjonsverktøy for Microsoft 365 Apps for enterprise distribusjonsscenarioer, kan du se Oversikt over Office [distribusjonsverktøy](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Hvis du vil ha mer informasjon om hvordan du bruker Office tilpassingsverktøyet, kan du se Oversikt over Office [tilpassingsverktøy](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
