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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="517bc-102">Spørsmål om hvordan du bruker distribusjons verktøy for Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="517bc-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="517bc-103">Last ned distribusjons verktøy for Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="517bc-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="517bc-104">Når du har lastet ned filen, kjører du den selv ut pakkende kjørbare filen, som inneholder Office Deployment Tool-kjørbare (setupodt.exe) og et eksempel på en konfigurasjons fil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="517bc-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="517bc-105">**Hvis du vil utelate eller fjerne Microsoft 365-apper for Enterprise-produkter fra klient data maskiner:**</span><span class="sxs-lookup"><span data-stu-id="517bc-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="517bc-106">Når du installerer Microsoft 365-apper for Enterprise, kan du utelate bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="517bc-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="517bc-107">Hvis du vil gjøre det, følger du Fremgangs måten for å installere Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjons filen.</span><span class="sxs-lookup"><span data-stu-id="517bc-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="517bc-108">Denne konfigurasjons filen installerer for eksempel alle Microsoft 365-appene for Enterprise-produkter bortsett fra Publisher:</span><span class="sxs-lookup"><span data-stu-id="517bc-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="517bc-109">Oversikt over distribusjons verktøyet for Office</span><span class="sxs-lookup"><span data-stu-id="517bc-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

