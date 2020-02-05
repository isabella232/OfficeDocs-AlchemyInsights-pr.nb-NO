---
title: Legge til en gruppe på et SharePoint-område
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770360"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="852f8-102">Problemer når du oppretter et gruppetilkoblet område i SharePoint</span><span class="sxs-lookup"><span data-stu-id="852f8-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="852f8-103">Noen vanlige problemer oppstod når du oppretter eller oppretter et gruppetilkoblet område på nytt.</span><span class="sxs-lookup"><span data-stu-id="852f8-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="852f8-104">Hvis du har slettet en gruppe og det tilkoblede området og ønsker å opprette et annet nettsted med samme URL-adresse, må du fjerne det forrige nettstedet permanent.</span><span class="sxs-lookup"><span data-stu-id="852f8-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="852f8-105">Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="852f8-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="852f8-106">Hvis du vil ha mer informasjon om hvordan du kommer i gang med Powershell, kan du se [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="852f8-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="852f8-107">Fjern området fra slettede områder ved hjelp av cmdleten [Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="852f8-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="852f8-108">Powershell er pålagt å slette gruppeområder permanent.</span><span class="sxs-lookup"><span data-stu-id="852f8-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="852f8-109">Hvis du oppretter et gruppetilkoblet område og mottar en advarsel: Det finnes allerede en **annen gruppe med samme alias,** kontrollerer du de eksisterende gruppene fra Office [365 fra administrasjonssenteret](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="852f8-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="852f8-110">Hvis du vil løse problemet, sletter du den eksisterende gruppen hvis den ikke lenger er nødvendig eller oppretter området med et annet alias tilordnet.</span><span class="sxs-lookup"><span data-stu-id="852f8-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="852f8-111">Det finnes forskjellige måter å opprette og bruke moderne grupper med SharePoint på.</span><span class="sxs-lookup"><span data-stu-id="852f8-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="852f8-112">Du kan koble eksisterende områder til en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="852f8-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="852f8-113">Hvis du vil ha mer informasjon, kan du se [Koble til en Office 365-gruppe ved hjelp av SharePoint-brukergrensesnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="852f8-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="852f8-114">Hvis du vil opprette et Office 365-gruppetilkoblet område, må du opprette et [gruppeområde](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="852f8-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
