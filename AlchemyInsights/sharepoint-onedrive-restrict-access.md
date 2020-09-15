---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700464"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c725b-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="c725b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c725b-103">Det er mange måter å begrense tilgang til SharePoint Online/OneDrive-tjenester på.</span><span class="sxs-lookup"><span data-stu-id="c725b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="c725b-104">Disse forskjellige Begrensnings metodene for tilgang er angitt nedenfor.</span><span class="sxs-lookup"><span data-stu-id="c725b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="c725b-105">**Tillatelses begrensning**</span><span class="sxs-lookup"><span data-stu-id="c725b-105">**Permission Restriction**</span></span>

<span data-ttu-id="c725b-106">I SharePoint Online og OneDrive for Business begrenser vi tilgang til elementer som nett steder, filer og mapper ved bare å gi tilgang til disse gruppene/enkelt personene som skal ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="c725b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="c725b-107">Tilpasse tillatelser for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="c725b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="c725b-108">Tilpasse tillatelser for SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="c725b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="c725b-109">Endre tillatelsene for en under mappe</span><span class="sxs-lookup"><span data-stu-id="c725b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="c725b-110">Kontrollere tilgang fra ikke-administrerte enheter</span><span class="sxs-lookup"><span data-stu-id="c725b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="c725b-111">Som en SharePoint-eller global administrator kan du blokkere eller begrense tilgang til SharePoint og OneDrive-innhold fra ikke-administrerte enheter (som ikke er hybride AD-sammenføyd eller kompatible i Intune).</span><span class="sxs-lookup"><span data-stu-id="c725b-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="c725b-112">**Nettverks plasserings begrensning**</span><span class="sxs-lookup"><span data-stu-id="c725b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="c725b-113">Som IT-administrator kan du kontrollere tilgang til SharePoint-og OneDrive-ressurser basert på definerte nettverks plasseringer du stoler på.</span><span class="sxs-lookup"><span data-stu-id="c725b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="c725b-114">Dette er også kjent som steds BAS ert policy.</span><span class="sxs-lookup"><span data-stu-id="c725b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="c725b-115">Hvis du vil ha mer informasjon, kan du se [kontrollere tilgang til SharePoint Online-og OneDrive-data basert på nettverks plassering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="c725b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="c725b-116">**Begrensninger for område lås**</span><span class="sxs-lookup"><span data-stu-id="c725b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="c725b-117">I SharePoint Online har du muligheten til å låse en nettsteds samling, så ingen har tilgang til den.</span><span class="sxs-lookup"><span data-stu-id="c725b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="c725b-118">Dette angis via PowerShell og [administrasjons grensesnittet for SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjelp av [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-egenskapen.</span><span class="sxs-lookup"><span data-stu-id="c725b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="c725b-119">**Begrense brukere fra å opprette områder eller sekundære områder**</span><span class="sxs-lookup"><span data-stu-id="c725b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="c725b-120">Som en SharePoint-administrator eller global administrator kan du la brukerne opprette og administrere sine egne SharePoint-nettsteder, bestemme hvilke typer områder de kan opprette, og angi plasseringen av områdene.</span><span class="sxs-lookup"><span data-stu-id="c725b-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="c725b-121">Hvis du vil ha mer informasjon, kan du se [Behandle område oppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="c725b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

