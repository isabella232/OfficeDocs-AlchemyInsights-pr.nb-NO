---
title: Ved hjelp av verktøyet for distribusjon av Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531584"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="85e6f-102">Ved hjelp av Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="85e6f-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="85e6f-103">Du kan bruke Office Deployment Tool (ODT) til å distribuere Office 365-versjoner av Office.</span><span class="sxs-lookup"><span data-stu-id="85e6f-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="85e6f-104">Distribusjonsverktøy for Office (setup.exe) kjøres fra kommandolinjen, og bruker en XML-konfigurasjonsfil for å avgjøre hvilke innstillinger som skal brukes når du distribuerer Office.</span><span class="sxs-lookup"><span data-stu-id="85e6f-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="85e6f-105">Last ned den nyeste versjonen av verktøyet for distribusjon av Office fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="85e6f-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="85e6f-106">Bruk [Office Customization Tool (OCT)](https://config.office.com) til å velge innstillinger for distribusjon og opprette XML-konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="85e6f-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="85e6f-107">Eksporter konfigurasjonsfilen, og plassere den lokalt på den samme mappen der det ligger på setup.exe.</span><span class="sxs-lookup"><span data-stu-id="85e6f-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="85e6f-108">**Merk:** Office-installasjonen problemene vanligvis oppstår forfaller til feilkonfigurert eller malformatted-konfigurasjonsfiler.</span><span class="sxs-lookup"><span data-stu-id="85e6f-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="85e6f-109">Hvis du vil unngå slike problemer, anbefaler vi at du bruker tilpasningsverktøyet for Office til å opprette konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="85e6f-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="85e6f-110">Du kan også importere eksisterende konfigurasjonsfiler til tilpasningsverktøyet for Office.</span><span class="sxs-lookup"><span data-stu-id="85e6f-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="85e6f-111">Fra en hevet ledetekst, gå til plasseringen der setup.exe ligger og kjøre verktøyet for distribusjon av Office i nedlastingsmodus og angi konfigurasjonsfilen du nettopp lagret.</span><span class="sxs-lookup"><span data-stu-id="85e6f-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="85e6f-112">I dette eksemplet heter konfigurasjonsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="85e6f-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="85e6f-113">Kjør verktøyet for distribusjon av Office i konfigurere modus og angi konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="85e6f-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="85e6f-114">**Merk:** Du må kjøre dette trinnet fra klientdatamaskinen som du vil installere Office, og du må ha lokale administratortillatelser på datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="85e6f-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="85e6f-115">Hvis du vil vite mer om hvordan du bruker Office distribusjonsverktøy for Office 365 ProPlus distribusjonsscenarier, kan du se [Oversikt over verktøyet for distribusjon av Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="85e6f-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="85e6f-116">Hvis du vil ha mer informasjon om hvordan du bruker tilpasningsverktøyet for Office, kan du se [Oversikt over tilpasningsverktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="85e6f-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
