---
title: Legge til en gruppe på et SharePoint-område
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771217"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="5b16a-102">Problemer når du oppretter et tilkoblet nettsted i SharePoint</span><span class="sxs-lookup"><span data-stu-id="5b16a-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="5b16a-103">Noen vanlige problemer som oppstår når du oppretter eller gjen opprettet et gruppe tilkoblet nettsted.</span><span class="sxs-lookup"><span data-stu-id="5b16a-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="5b16a-104">Hvis du har slettet en gruppe og det tilkoblede nettstedet og vil opprette et annet nettsted med samme URL-adresse, må du fjerne det forrige nettstedet for godt.</span><span class="sxs-lookup"><span data-stu-id="5b16a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="5b16a-105">Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="5b16a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="5b16a-106">Hvis du vil ha mer informasjon om hvordan du kommer i gang med PowerShell, kan du se [komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="5b16a-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="5b16a-107">Fjern nettstedet fra Slettede nett steder ved hjelp av PowerShell-cmdleten [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="5b16a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="5b16a-108">PowerShell kreves for å slette gruppe nett steder permanent.</span><span class="sxs-lookup"><span data-stu-id="5b16a-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="5b16a-109">Hvis du oppretter et gruppe tilkoblet nettsted og mottar en advarsel: **en annen gruppe med samme alias finnes allerede**, kan du kontrollere de eksisterende gruppene fra [administrasjons senteret for Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="5b16a-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="5b16a-110">Hvis du vil løse problemet, sletter du den eksisterende gruppen hvis den ikke lenger er nødvendig, eller oppretter nettstedet med et annet alias tilordnet.</span><span class="sxs-lookup"><span data-stu-id="5b16a-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="5b16a-111">Det finnes ulike metoder for å opprette og bruke moderne grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5b16a-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="5b16a-112">Du kan koble eksisterende områder til en Microsoft 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="5b16a-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="5b16a-113">Hvis du vil ha mer informasjon, kan du se [Koble til en Microsoft 365-gruppe ved å bruke SharePoint-brukergrensesnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="5b16a-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="5b16a-114">Hvis du vil opprette et område i en Microsoft 365-gruppe som er tilkoblet, må du opprette et [gruppe område](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="5b16a-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
