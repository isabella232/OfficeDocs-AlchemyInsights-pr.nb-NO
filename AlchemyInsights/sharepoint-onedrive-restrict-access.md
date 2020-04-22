---
title: Begrense tilgang en sharepoint eller onedrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692774"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0069c-102">Begrense tilgang en sharepoint eller onedrive</span><span class="sxs-lookup"><span data-stu-id="0069c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0069c-103">Det er mange måter å begrense tilgangen til SharePoint Online/OneDrive-tjenester på.</span><span class="sxs-lookup"><span data-stu-id="0069c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="0069c-104">Disse ulike tilgangsbegrensningsmetodene er skissert nedenfor.</span><span class="sxs-lookup"><span data-stu-id="0069c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="0069c-105">**Begrensning av tillatelser**</span><span class="sxs-lookup"><span data-stu-id="0069c-105">**Permission Restriction**</span></span>

<span data-ttu-id="0069c-106">I SharePoint Online og OneDrive for Business begrenser vi tilgangen til elementer som områder, filer og mapper ved å bare gi tilgang til de gruppene/personene som skal ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="0069c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="0069c-107">Tilpasse tillatelser for en SharePoint-liste eller et SharePoint-bibliotek</span><span class="sxs-lookup"><span data-stu-id="0069c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="0069c-108">Tilpasse tillatelser for SharePoint-området</span><span class="sxs-lookup"><span data-stu-id="0069c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="0069c-109">Endre tillatelsene for en undermappe</span><span class="sxs-lookup"><span data-stu-id="0069c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="0069c-110">Kontrollere tilgang fra ikke-administrerte enheter</span><span class="sxs-lookup"><span data-stu-id="0069c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="0069c-111">Som SharePoint eller global administrator kan du blokkere eller begrense tilgangen til SharePoint- og OneDrive-innhold fra uadministrerte enheter (de som ikke er hybrid-AD som er koblet til eller kompatibel i Intune).</span><span class="sxs-lookup"><span data-stu-id="0069c-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="0069c-112">**Begrensning av nettverksplassering**</span><span class="sxs-lookup"><span data-stu-id="0069c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="0069c-113">Som IT-administrator kan du kontrollere tilgangen til SharePoint- og OneDrive-ressurser basert på definerte nettverksplasseringer du stoler på.</span><span class="sxs-lookup"><span data-stu-id="0069c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="0069c-114">Dette kalles også stedsbasert policy.</span><span class="sxs-lookup"><span data-stu-id="0069c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="0069c-115">Hvis du vil ha mer informasjon, kan du se [Kontrollere tilgang til SharePoint Online- og OneDrive-data basert på nettverksplassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="0069c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="0069c-116">**Begrensning av områdelås**</span><span class="sxs-lookup"><span data-stu-id="0069c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="0069c-117">I SharePoint Online har du muligheten til å låse en områdesamling, slik at ingen har tilgang.</span><span class="sxs-lookup"><span data-stu-id="0069c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="0069c-118">Dette er angitt via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av egenskapen [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState .</span><span class="sxs-lookup"><span data-stu-id="0069c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="0069c-119">**Begrense brukere fra å opprette områder eller sekundære områder**</span><span class="sxs-lookup"><span data-stu-id="0069c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="0069c-120">Som SharePoint-administrator eller Global administrator kan du la brukerne opprette og administrere sine egne SharePoint-områder, finne ut hva slags områder de kan opprette, og angi plasseringen av områdene.</span><span class="sxs-lookup"><span data-stu-id="0069c-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="0069c-121">Hvis du vil ha mer informasjon, kan du se [Administrere oppretting av område i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="0069c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

