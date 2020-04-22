---
title: Bruke distribusjonsverktøyet for Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726257"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bruke Office Deployment Tool (ODT)

Du kan bruke Office Deployment Tool (ODT) til å distribuere Office 365-versjoner av Office. Office Deployment Tool (setup.exe) kjøres fra kommandolinjen og bruker en XML-konfigurasjonsfil til å bestemme hvilke innstillinger som skal brukes når du distribuerer Office.
  
1. Last ned den nyeste versjonen av Office Deployment Tool fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Bruk [tilpassingsverktøyet for Office (OCT)](https://config.office.com) til å velge distribusjonsinnstillingene og opprette XML-filen for konfigurasjon. Eksporter konfigurasjonsfilen og plasser den lokalt i samme mappe der setup.exe ligger.

    **Merk:** Problemer med Office-installasjon oppstår vanligvis på grunn av feilkonfigurerte eller feilformaterte konfigurasjonsfiler. Hvis du vil unngå slike problemer, anbefaler vi at du bruker tilpassingsverktøyet for Office til å opprette konfigurasjonsfilen. Du kan også importere eksisterende konfigurasjonsfiler til tilpasningsverktøyet for Office.

3. Fra en hevet ledetekst bytter du til plasseringen der setup.exe befinner seg og kjører Office Deployment Tool i nedlastingsmodus og angir konfigurasjonsfilen du nettopp lagret. I dette eksemplet heter konfigurasjonsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kjør Distribusjonsverktøyet for Office i konfigurasjonsmodus, og angi konfigurasjonsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Merk:** Du må kjøre dette trinnet fra klientdatamaskinen du vil installere Office på, og du må ha lokale administratortillatelser på den datamaskinen.

Hvis du vil lære mer om hvordan du bruker Office Deployment Tool for microsoft 365 Apps for enterprise deployment scenarios, kan du se [Oversikt over Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Hvis du vil ha mer informasjon om hvordan du bruker tilpassingsverktøyet for Office, kan du se [Oversikt over tilpassingsverktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
