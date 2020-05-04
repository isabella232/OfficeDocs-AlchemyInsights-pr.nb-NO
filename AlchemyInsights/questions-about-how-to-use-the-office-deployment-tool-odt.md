---
title: Spørsmål om hvordan du bruker Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010759"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørsmål om hvordan du bruker Office Deployment Tool (ODT)

Last ned verktøyet for distribusjon av Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har lastet ned filen, kjører du den selvutpakkende kjørbare filen, som inneholder den kjørbare filen Office Deployment Tool (setup.exe) og en eksempelkonfigurasjonsfil (configuration.xml).
  
 **Slik utelater eller fjerner du Microsoft 365 Apps for enterprise-produkter fra klientdatamaskiner:**
  
Når du installerer Microsoft 365 Apps for enterprise, kan du ekskludere bestemte produkter. Hvis du vil gjøre dette, følger du fremgangsmåten for å installere Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjonsfilen. Denne konfigurasjonsfilen installerer for eksempel alle Microsoft 365-apper for bedriftsprodukter unntatt Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversikt over distribusjonsverktøyet for Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

