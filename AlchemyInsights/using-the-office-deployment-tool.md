---
title: Bruke distribusjonsverktøyet for Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010876"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="8a9a2-102">Bruke Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="8a9a2-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="8a9a2-103">Du kan bruke Office Deployment Tool (ODT) til å distribuere Office 365-versjoner av Office.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="8a9a2-104">Office Deployment Tool (setup.exe) kjøres fra kommandolinjen og bruker en XML-konfigurasjonsfil til å bestemme hvilke innstillinger som skal brukes når du distribuerer Office.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="8a9a2-105">Last ned den nyeste versjonen av Office Deployment Tool fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="8a9a2-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="8a9a2-106">Bruk [tilpassingsverktøyet for Office (OCT)](https://config.office.com) til å velge distribusjonsinnstillingene og opprette XML-filen for konfigurasjon.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="8a9a2-107">Eksporter konfigurasjonsfilen og plasser den lokalt i samme mappe der setup.exe ligger.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="8a9a2-108">**Merk:** Problemer med Office-installasjon oppstår vanligvis på grunn av feilkonfigurerte eller feilformaterte konfigurasjonsfiler.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="8a9a2-109">Hvis du vil unngå slike problemer, anbefaler vi at du bruker tilpassingsverktøyet for Office til å opprette konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="8a9a2-110">Du kan også importere eksisterende konfigurasjonsfiler til tilpasningsverktøyet for Office.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="8a9a2-111">Fra en hevet ledetekst bytter du til plasseringen der setup.exe befinner seg og kjører Office Deployment Tool i nedlastingsmodus og angir konfigurasjonsfilen du nettopp lagret.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="8a9a2-112">I dette eksemplet heter konfigurasjonsfilen Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="8a9a2-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="8a9a2-113">Kjør Distribusjonsverktøyet for Office i konfigurasjonsmodus, og angi konfigurasjonsfilen.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="8a9a2-114">**Merk:** Du må kjøre dette trinnet fra klientdatamaskinen du vil installere Office på, og du må ha lokale administratortillatelser på den datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="8a9a2-115">Hvis du vil lære mer om hvordan du bruker Office Deployment Tool for microsoft 365 Apps for enterprise deployment scenarios, kan du se [Oversikt over Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="8a9a2-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="8a9a2-116">Hvis du vil ha mer informasjon om hvordan du bruker tilpassingsverktøyet for Office, kan du se [Oversikt over tilpassingsverktøyet for Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="8a9a2-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
