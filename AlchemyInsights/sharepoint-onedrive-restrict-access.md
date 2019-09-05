---
title: Begrens tilgang i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750673"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="3bfc0-102">Begrens tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="3bfc0-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="3bfc0-103">Det er mange måter å begrense tilgangen til SharePoint Online/OneDrive tjenester.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="3bfc0-104">Disse ulike tilgangs Begrensnings metodene er beskrevet nedenfor.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="3bfc0-105">**Tillatelse begrensning**</span><span class="sxs-lookup"><span data-stu-id="3bfc0-105">**Permission Restriction**</span></span>

<span data-ttu-id="3bfc0-106">I SharePoint Online og OneDrive for Business, begrenser vi tilgang til elementer som områder, filer og mapper ved bare å gi tilgang til disse gruppene/enkeltpersoner som skal ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="3bfc0-107">Tilpasse tillatelser for SharePoint-lister eller-biblioteker</span><span class="sxs-lookup"><span data-stu-id="3bfc0-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="3bfc0-108">Tilpasse tillatelser for SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="3bfc0-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="3bfc0-109">Endre tillatelsene for en undermappe</span><span class="sxs-lookup"><span data-stu-id="3bfc0-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="3bfc0-110">Kontrollere tilgang fra ikke-administrerte enheter</span><span class="sxs-lookup"><span data-stu-id="3bfc0-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="3bfc0-111">Som en SharePoint eller global administrator i Office 365, kan du blokkere eller begrense tilgangen til SharePoint-og OneDrive-innhold fra ikke-administrerte enheter (de som ikke er kombinert AD eller kompatibel i Intune).</span><span class="sxs-lookup"><span data-stu-id="3bfc0-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="3bfc0-112">**Begrensning av nettverksplassering**</span><span class="sxs-lookup"><span data-stu-id="3bfc0-112">**Network Location Restriction**</span></span>

<span data-ttu-id="3bfc0-113">Som IT-administrator kan du styre tilgangen til SharePoint-og OneDrive-ressurser basert på definerte nettverksplasseringer du stoler på.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="3bfc0-114">Dette er også kjent som stedsbasert policy.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-114">This is also known as location-based policy.</span></span> <span data-ttu-id="3bfc0-115">Hvis du vil ha mer informasjon, kan du se [kontrollere tilgangen til SharePoint Online og OneDrive-data basert på nettverksplassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="3bfc0-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="3bfc0-116">**Begrensning av område lås**</span><span class="sxs-lookup"><span data-stu-id="3bfc0-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="3bfc0-117">I SharePoint Online har du muligheten til å låse en områdesamling, slik at ingen har tilgang til dem.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="3bfc0-118">Dette angis via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-egenskapen.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="3bfc0-119">**Hindre brukere i å opprette områder eller sekundære områder**</span><span class="sxs-lookup"><span data-stu-id="3bfc0-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="3bfc0-120">Som en SharePoint-administrator eller en global administrator for Office 365 kan du la brukerne opprette og administrere sine egne SharePoint-områder, bestemme hva slags områder de kan opprette og angi plasseringen av områdene.</span><span class="sxs-lookup"><span data-stu-id="3bfc0-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="3bfc0-121">Hvis du vil ha mer informasjon, kan du se [Behandle områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="3bfc0-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

