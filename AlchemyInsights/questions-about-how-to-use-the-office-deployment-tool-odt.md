---
title: Spørsmål om hvordan du bruker distribusjons verktøy for Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086165"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørsmål om hvordan du bruker distribusjons verktøy for Office (ODT)

Last ned distribusjons verktøy for Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har lastet ned filen, kjører du den selv ut pakkende kjørbare filen, som inneholder Office Deployment Tool-kjørbare (setupodt.exe) og et eksempel på en konfigurasjons fil (configuration.xml).
  
 **Hvis du vil utelate eller fjerne Microsoft 365-apper for Enterprise-produkter fra klient data maskiner:**
  
Når du installerer Microsoft 365-apper for Enterprise, kan du utelate bestemte produkter. Hvis du vil gjøre det, følger du Fremgangs måten for å installere Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjons filen. Denne konfigurasjons filen installerer for eksempel alle Microsoft 365-appene for Enterprise-produkter bortsett fra Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversikt over distribusjons verktøyet for Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

