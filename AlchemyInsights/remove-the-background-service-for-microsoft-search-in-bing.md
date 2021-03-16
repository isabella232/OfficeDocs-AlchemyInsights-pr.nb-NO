---
title: Fjerne bakgrunnstjenesten for Microsoft Search i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816333"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="b1c57-102">Fjerne bakgrunnstjenesten for Microsoft Search i Bing</span><span class="sxs-lookup"><span data-stu-id="b1c57-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="b1c57-103">Hvis du vil fjerne bakgrunnstjenesten for Microsoft Search i Bing, kan du prøve følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="b1c57-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="b1c57-104">Hvis du vil gå tilbake til de opprinnelige innstillingene for søkemotoren, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="b1c57-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="b1c57-105">a.</span><span class="sxs-lookup"><span data-stu-id="b1c57-105">a.</span></span> <span data-ttu-id="b1c57-106">Bytt **av veksleknappen Bruk [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Bing som standard søkemotor**.</span><span class="sxs-lookup"><span data-stu-id="b1c57-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="b1c57-107">b.</span><span class="sxs-lookup"><span data-stu-id="b1c57-107">b.</span></span> <span data-ttu-id="b1c57-108">[Gå til administrasjonssenteret for Microsoft 365,](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) og fjern innstillingen som påvirker alle brukerne i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b1c57-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="b1c57-109">Hvis du vil fjerne bakgrunnstjenesten fra en enkelt enhet, gjør du følgende oppgaver:</span><span class="sxs-lookup"><span data-stu-id="b1c57-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="b1c57-110">a.</span><span class="sxs-lookup"><span data-stu-id="b1c57-110">a.</span></span> <span data-ttu-id="b1c57-111">Velg **Kontrollpanel > programmer > programmer og funksjoner**.</span><span class="sxs-lookup"><span data-stu-id="b1c57-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="b1c57-112">b.</span><span class="sxs-lookup"><span data-stu-id="b1c57-112">b.</span></span> <span data-ttu-id="b1c57-113">Høyreklikk Microsoft **Søk i Bing** under listen over installerte programmer, og klikk deretter **Avinstaller**.</span><span class="sxs-lookup"><span data-stu-id="b1c57-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="b1c57-114">Hvis du vil fjerne bakgrunnstjenesten fra flere enheter i organisasjonen, logger du på som administrator og kjører følgende kommando i et skript:</span><span class="sxs-lookup"><span data-stu-id="b1c57-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
