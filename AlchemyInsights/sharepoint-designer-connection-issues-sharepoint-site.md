---
title: Tilkoblings problemer i SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727180"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="353d8-102">Tilkoblings problemer i SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="353d8-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="353d8-103">Hvis SharePoint Designer har tilkoblings problemer til SharePoint-nettsteder, kan du prøve følgende vanlige løsninger.</span><span class="sxs-lookup"><span data-stu-id="353d8-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="353d8-104">Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [oppdateringen fra August 2, 2016 for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="353d8-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="353d8-105">Trinn 2: Fjern de lokale hurtig buffer filene:</span><span class="sxs-lookup"><span data-stu-id="353d8-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="353d8-106">Lukk SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="353d8-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="353d8-107">På den lokale data maskinen fjerner du alle filene som ble funnet i hver av følgende mapper.</span><span class="sxs-lookup"><span data-stu-id="353d8-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="353d8-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="353d8-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="353d8-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="353d8-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="353d8-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="353d8-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="353d8-111">Åpne SharePoint Designer 2013, og skriv inn kontoen på nytt for å se om det fungerer.</span><span class="sxs-lookup"><span data-stu-id="353d8-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="353d8-112">Trinn 3: [Aktiver moderne godkjenning for Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="353d8-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="353d8-113">Trinn 4: administratorer må **tillate egen definert skript** i innstillingene for administrasjons senteret for SharePoint for å tillate SharePoint Designer-tilkoblingen.</span><span class="sxs-lookup"><span data-stu-id="353d8-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="353d8-114">Se [tillate eller hindre egen definert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="353d8-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


