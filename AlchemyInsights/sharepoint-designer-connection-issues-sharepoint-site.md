---
title: SharePoint Designer-tilkoblingsproblemer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508432"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="5b57f-102">SharePoint Designer-tilkoblingsproblemer</span><span class="sxs-lookup"><span data-stu-id="5b57f-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="5b57f-103">Hvis SharePoint Designer er problemer med tilkoblingen til SharePoint-områder, kan du prøve følgende vanlige løsninger.</span><span class="sxs-lookup"><span data-stu-id="5b57f-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="5b57f-104">Trinn 1: Kontroller at SharePoint Designer 2013 er oppdatert med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) og [2. August 2016 oppdatering for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="5b57f-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="5b57f-105">Trinn 2: Fjerne lokal hurtigbuffer-filer:</span><span class="sxs-lookup"><span data-stu-id="5b57f-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="5b57f-106">Lukk SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5b57f-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="5b57f-107">Fjerne alle filer som finnes i hver av følgende mapper på den lokale datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="5b57f-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="5b57f-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="5b57f-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="5b57f-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="5b57f-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="5b57f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="5b57f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="5b57f-111">Åpne SharePoint Designer 2013, og Skriv inn kontoen på nytt for å se om det fungerer.</span><span class="sxs-lookup"><span data-stu-id="5b57f-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="5b57f-112">Trinn 3: [Aktiver moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5b57f-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="5b57f-113">Trinn 4: Administratorer må **Tillate egendefinert skript** i administrasjonssenteret for SharePoint-innstillingene til å tillate SharePoint Designer-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="5b57f-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="5b57f-114">Se [Tillat eller forby egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="5b57f-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


