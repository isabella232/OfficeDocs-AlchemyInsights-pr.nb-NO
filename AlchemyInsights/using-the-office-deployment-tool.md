---
title: Ved hjelp av verktøyet for distribusjon av Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423192"
---
# <a name="using-the-office-deployment-tool-odt"></a>Ved hjelp av Office Deployment Tool (ODT)

Du kan bruke Office Deployment Tool (ODT) til å distribuere Office 365-versjoner av Office. Distribusjonsverktøy for Office (setup.exe) kjøres fra kommandolinjen, og bruker en XML-konfigurasjonsfil for å avgjøre hvilke innstillinger som skal brukes når du distribuerer Office.
  
1. Last ned den nyeste versjonen av verktøyet for distribusjon av Office fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Bruk [Office Customization Tool (OCT)](https://config.office.com) til å velge innstillinger for distribusjon og opprette XML-konfigurasjonsfilen. Eksporter konfigurasjonsfilen, og plassere den lokalt på den samme mappen der det ligger på setup.exe. 
    
    **Merk:** Office-installasjonen problemene vanligvis oppstår forfaller til feilkonfigurert eller malformatted-konfigurasjonsfiler. Hvis du vil unngå slike problemer, anbefaler vi at du bruker tilpasningsverktøyet for Office til å opprette konfigurasjonsfilen. Du kan også importere eksisterende konfigurasjonsfiler til tilpasningsverktøyet for Office. 
    
3. Fra en hevet ledetekst, gå til plasseringen der setup.exe ligger og kjøre verktøyet for distribusjon av Office i nedlastingsmodus og angi konfigurasjonsfilen du nettopp lagret. I dette eksemplet heter konfigurasjonsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kjør verktøyet for distribusjon av Office i konfigurere modus og angi konfigurasjonsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Merk:** Du må kjøre dette trinnet fra klientdatamaskinen som du vil installere Office, og du må ha lokale administratortillatelser på datamaskinen. 
    
Hvis du vil vite mer om hvordan du bruker Office distribusjonsverktøy for Office 365 ProPlus distribusjonsscenarier, kan du se [Oversikt over verktøyet for distribusjon av Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Hvis du vil ha mer informasjon om hvordan du bruker tilpasningsverktøyet for Office, kan du se [Oversikt over tilpasningsverktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

