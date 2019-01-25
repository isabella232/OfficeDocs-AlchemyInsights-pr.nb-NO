---
title: Spørsmål om hvordan du bruker Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481923"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørsmål om hvordan du bruker Office Deployment Tool (ODT)

Last ned verktøyet for distribusjon av Office fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Etter at du har lastet ned filen, kan du kjøre den selvutpakkende kjørbare filen som inneholder Office distribusjon av verktøyet for kjørbare (setup.exe) og en eksempel-konfigurasjonsfil (configuration.xml).
  
 **Å utelukke eller fjerne Office 365 ProPlus produkter fra klientdatamaskiner:**
  
Når du installerer Office 365 ProPlus, kan du utelate bestemte produkter. Hvis du vil gjøre dette, følger du trinnene for å installere Office med Office-Søkeverktøyet, men inkluderer ExcludeApp-element i konfigurasjonsfilen. Denne konfigurasjonsfilen installerer for eksempel alle Office 365 ProPlus produktene bortsett fra Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversikt over verktøyet for distribusjon av Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

