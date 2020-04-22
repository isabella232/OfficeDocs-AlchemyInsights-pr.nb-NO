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
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698067"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="07d98-102">Spørsmål om hvordan du bruker Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="07d98-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="07d98-103">Last ned verktøyet for distribusjon av Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="07d98-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="07d98-104">Når du har lastet ned filen, kjører du den selvutpakkende kjørbare filen, som inneholder den kjørbare filen Office Deployment Tool (setup.exe) og en eksempelkonfigurasjonsfil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="07d98-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="07d98-105">**Slik utelater eller fjerner du Microsoft 365 Apps for enterprise-produkter fra klientdatamaskiner:**</span><span class="sxs-lookup"><span data-stu-id="07d98-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="07d98-106">Når du installerer Microsoft 365 Apps for enterprise, kan du ekskludere bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="07d98-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="07d98-107">Hvis du vil gjøre dette, følger du fremgangsmåten for å installere Office med ODT, men inkluderer ExcludeApp-elementet i konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="07d98-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="07d98-108">Denne konfigurasjonsfilen installerer for eksempel alle Microsoft 365-apper for bedriftsprodukter unntatt Publisher:</span><span class="sxs-lookup"><span data-stu-id="07d98-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="07d98-109">Oversikt over distribusjonsverktøyet for Office</span><span class="sxs-lookup"><span data-stu-id="07d98-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

