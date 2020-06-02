---
title: Tilkoblingsproblemer for SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511553"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="a1fea-102">Tilkoblingsproblemer for SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="a1fea-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="a1fea-103">Hvis SharePoint Designer har tilkoblingsproblemer til SharePoint-områder, kan du prøve følgende vanlige løsninger.</span><span class="sxs-lookup"><span data-stu-id="a1fea-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="a1fea-104">Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [2 August 2016 oppdatering for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="a1fea-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="a1fea-105">Trinn 2: Tøm de lokale bufferfilene:</span><span class="sxs-lookup"><span data-stu-id="a1fea-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="a1fea-106">Lukk SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a1fea-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="a1fea-107">Fjern alle filene i hver av følgende mapper på den lokale datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="a1fea-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="a1fea-108">%APPDATA%\Microsoft\Web-servertillegg\hurtigbuffer</span><span class="sxs-lookup"><span data-stu-id="a1fea-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="a1fea-109">%APPDATA%Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="a1fea-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="a1fea-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="a1fea-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="a1fea-111">Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om den fungerer.</span><span class="sxs-lookup"><span data-stu-id="a1fea-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="a1fea-112">Trinn 3: [Aktiver moderne godkjenning for Office-2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a1fea-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="a1fea-113">Trinn 4: Administratorer må **tillate egendefinert skript** i administrasjonssenteret for SharePoint for å tillate SharePoint Designer-tilkoblingen.</span><span class="sxs-lookup"><span data-stu-id="a1fea-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="a1fea-114">Se [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a1fea-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


