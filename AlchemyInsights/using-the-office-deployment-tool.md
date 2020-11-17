---
title: Bruke distribusjons verktøy for Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085841"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="434f9-102">Bruke distribusjons verktøy for Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="434f9-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="434f9-103">Du bruker distribusjons verktøy for Office (ODT) til å distribuere Office 365-versjoner av Office.</span><span class="sxs-lookup"><span data-stu-id="434f9-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="434f9-104">Distribusjons verktøy for Office (setupodt.exe) kjøres fra kommando linjen og bruker en XML-fil for konfigurasjon til å finne ut hvilke innstillinger som skal brukes når du distribuerer Office.</span><span class="sxs-lookup"><span data-stu-id="434f9-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="434f9-105">Last ned den nyeste versjonen av distribusjons verktøyet for Office fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="434f9-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="434f9-106">Bruk [tilpasnings verktøyet for Office](https://config.office.com) for å velge distribusjons innstillingene og opprette XML-filen for konfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="434f9-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="434f9-107">Eksporter konfigurasjons filen, og plasser den lokalt i samme mappe som setupodt.exe finnes i.</span><span class="sxs-lookup"><span data-stu-id="434f9-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="434f9-108">**Obs!** Problemer med Office-installasjonen forekommer vanligvis på grunn av feil kon figurerte eller malformattede konfigurasjons filer.</span><span class="sxs-lookup"><span data-stu-id="434f9-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="434f9-109">Vi anbefaler at du bruker tilpasnings verktøyet for Office til å opprette konfigurasjons filen for å unngå slike problemer.</span><span class="sxs-lookup"><span data-stu-id="434f9-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="434f9-110">Du kan også importere eksisterende konfigurasjons filer til tilpasnings verktøyet for Office.</span><span class="sxs-lookup"><span data-stu-id="434f9-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="434f9-111">Gå til plasseringen der setupodt.exe befinner seg i en hevet lede tekst, og Kjør distribusjons verktøyet for Office i Download Mode, og angi konfigurasjons filen du nettopp lagret.</span><span class="sxs-lookup"><span data-stu-id="434f9-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="434f9-112">I dette eksemplet kalles konfigurasjons filen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="434f9-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="434f9-113">4. Kjør distribusjons verktøyet for Office i konfigurerings modus, og angi konfigurasjons filen.</span><span class="sxs-lookup"><span data-stu-id="434f9-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="434f9-114">**Obs!** Du må kjøre dette trinnet fra klient data maskinen du vil installere Office på, og du må ha lokale administrator tillatelser på denne data maskinen.</span><span class="sxs-lookup"><span data-stu-id="434f9-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="434f9-115">Hvis du vil lære mer om hvordan du bruker distribusjons verktøy for Office for Microsoft 365-appene for distribusjon av bedrifts distribusjon, kan du se [Oversikt over distribusjons verktøyet for Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="434f9-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="434f9-116">Hvis du vil ha mer informasjon om hvordan du bruker tilpasnings verktøyet for Office, kan du se [Oversikt over tilpasnings verktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="434f9-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
