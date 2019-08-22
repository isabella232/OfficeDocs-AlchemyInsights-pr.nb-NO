---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559886"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="ba78b-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="ba78b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="ba78b-103">Det er mange måter å begrense tilgang til SharePoint Online/OneDrive tjenester.</span><span class="sxs-lookup"><span data-stu-id="ba78b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="ba78b-104">Disse ulike metoder for begrensningen beskrives nedenfor.</span><span class="sxs-lookup"><span data-stu-id="ba78b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="ba78b-105">**Begrensning av tilgang**</span><span class="sxs-lookup"><span data-stu-id="ba78b-105">**Permission Restriction**</span></span>

<span data-ttu-id="ba78b-106">I SharePoint Online og OneDrive for bedrifter begrense vi tilgang til elementer, for eksempel områder, filer og mapper ved å bare gi tilgang til de grupper/personene som skal ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="ba78b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="ba78b-107">Tilpasse tillatelser for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="ba78b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="ba78b-108">Tilpasse SharePoint-områdetillatelser</span><span class="sxs-lookup"><span data-stu-id="ba78b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="ba78b-109">Endre tillatelsene for en undermappe</span><span class="sxs-lookup"><span data-stu-id="ba78b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="ba78b-110">Kontrollere tilgang fra ikke-administrerte enheter</span><span class="sxs-lookup"><span data-stu-id="ba78b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="ba78b-111">SharePoint eller global admin i Office 365, kan du sperre eller begrense tilgang til innhold i SharePoint og OneDrive fra ikke-administrerte enheter (de ikke hybrid Annonse sammenføyde eller kompatibel i Intune).</span><span class="sxs-lookup"><span data-stu-id="ba78b-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="ba78b-112">**Nettverk plasseringen begrensning**</span><span class="sxs-lookup"><span data-stu-id="ba78b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="ba78b-113">Som en IT-administrator, kan du styre tilgang til SharePoint- og OneDrive ressurser basert på definerte nettverksplasseringer som du stoler på.</span><span class="sxs-lookup"><span data-stu-id="ba78b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="ba78b-114">Dette er også kjent som sted-basert policy.</span><span class="sxs-lookup"><span data-stu-id="ba78b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="ba78b-115">Hvis du vil ha mer informasjon, se [kontrollere tilgang til SharePoint Online og OneDrive data basert på nettverksplasseringen](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="ba78b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="ba78b-116">**Lås områdebegrensningen**</span><span class="sxs-lookup"><span data-stu-id="ba78b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="ba78b-117">Du har muligheten til å låse en områdesamling, slik at ingen har tilgang til i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ba78b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="ba78b-118">Dette angis via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState-egenskapen.</span><span class="sxs-lookup"><span data-stu-id="ba78b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="ba78b-119">**Hindre brukere i å opprette områder eller sekundære områder**</span><span class="sxs-lookup"><span data-stu-id="ba78b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="ba78b-120">Du kan la brukerne opprette og administrere sine egne SharePoint-områder, finne ut hvilke områder de kan opprette, som en SharePoint-administrator eller en global administrator for Office 365 og angi plasseringen av områdene.</span><span class="sxs-lookup"><span data-stu-id="ba78b-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="ba78b-121">Hvis du vil ha mer informasjon, kan du se [Behandle områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="ba78b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

