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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051110"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="a4d18-102">Problemer når du oppretter eller grupperer tilkoblede områder i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a4d18-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="a4d18-103">Det er et par vanlige problemer som oppstår når du oppretter eller gjenoppretter en gruppe koblet området.</span><span class="sxs-lookup"><span data-stu-id="a4d18-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="a4d18-104">Hvis du har slettet en gruppe og det tilkoblede området og ønsker å opprette et annet område med samme NETTADRESSE, må du fjerne det forrige området permanent.</span><span class="sxs-lookup"><span data-stu-id="a4d18-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="a4d18-105">Last ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="a4d18-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="a4d18-106">Hvis du vil ha mer informasjon om hvordan du kommer i gang med PowerShell, se [komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="a4d18-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="a4d18-107">Fjern området fra Slettede områder ved hjelp av [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdleten.</span><span class="sxs-lookup"><span data-stu-id="a4d18-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="a4d18-108">Hvis du oppretter et tilkoblet Gruppeområde og mottar en advarsel en annen gruppe med samme alias finnes allerede, kan du kontrollere de eksisterende gruppene fra [Office 365 fra administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="a4d18-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="a4d18-109">Du kan løse problemet ved å slette den eksisterende gruppen hvis den ikke lenger er nødvendig, eller opprette området med et annet alias tilordnet.</span><span class="sxs-lookup"><span data-stu-id="a4d18-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="a4d18-110">Det finnes ulike måter å opprette og bruke moderne grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a4d18-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="a4d18-111">Du kan koble eksisterende områder til en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="a4d18-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="a4d18-112">Hvis du vil ha mer informasjon, kan [du se koble en Office 365-gruppe ved hjelp av SharePoint-ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="a4d18-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="a4d18-113">Hvis du vil opprette et tilkoblet område for Office 365-gruppen, må du opprette et gruppeområde.</span><span class="sxs-lookup"><span data-stu-id="a4d18-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="a4d18-114">Hvis du vil ha mer informasjon, kan du se [opprette et gruppeområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="a4d18-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

