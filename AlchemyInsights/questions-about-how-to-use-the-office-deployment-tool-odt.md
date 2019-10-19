---
title: Spørsmål om hvordan du bruker Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553549"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørsmål om hvordan du bruker Office Deployment Tool (ODT)

Last ned Office Deployment Tool fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har lastet ned filen, kjører du den kjørbare selvutpakkende filen som inneholder Office Deployment Tool kjørbar fil (Setup. exe) og et eksempel på en konfigurasjonsfil (Configuration. XML).
  
 **Slik ekskluderer eller fjerner du Office 365 ProPlus-produkter fra klientdatamaskiner:**
  
Når du installerer Office 365 ProPlus, kan du ekskludere bestemte produkter. Hvis du vil gjøre dette, følger du fremgangsmåten for å installere Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjonsfilen. Denne konfigurasjonsfilen installerer for eksempel alle Office 365 ProPlus-produkter unntatt Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversikt over distribusjonsverktøyet for Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

