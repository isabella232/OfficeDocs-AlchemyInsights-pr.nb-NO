---
title: Spørsmål om hvordan du bruker distribusjonsverktøyet Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959692"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørsmål om hvordan du bruker distribusjonsverktøyet Office (ODT)

Last ned Office distribusjonsverktøyet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har lastet ned filen, kjører du den selvutpakkende kjørbare filen, som inneholder den kjørbare Office-distribusjonsverktøyet (setup.exe) og en eksempelkonfigurasjonsfil (configuration.xml).
  
 **Slik utelater eller fjerner Microsoft 365 Apps for enterprise produkter fra klientdatamaskiner:**
  
Når du installerer Microsoft 365 Apps for enterprise, kan du utelate bestemte produkter. Hvis du vil gjøre dette, følger du fremgangsmåten for å Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjonsfilen. Denne konfigurasjonsfilen installerer for eksempel alle Microsoft 365 Apps for enterprise produkter unntatt Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversikt over Office distribusjonsverktøyet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

