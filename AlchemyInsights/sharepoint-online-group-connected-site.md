---
title: Legge til en gruppe på et SharePoint-område
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507856"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="d8337-102">Problemer når du oppretter eller en gruppe koblet områder i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d8337-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="d8337-103">Det er noen vanlige problemer som kan oppstå når koblet område å opprette eller opprette en gruppe på nytt.</span><span class="sxs-lookup"><span data-stu-id="d8337-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="d8337-104">Hvis du har slettet en gruppe, og det tilknyttede området og ønsker å opprette et annet område med samme URL-adresse, må du slette det forrige området.</span><span class="sxs-lookup"><span data-stu-id="d8337-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="d8337-105">Last ned [SPO administrasjonskonsoll](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="d8337-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="d8337-106">For mer informasjon om å komme i gang med powershell, kan du se [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="d8337-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="d8337-107">Fjerne webområdet fra slettet områder ved hjelp av [Fjern SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell-cmdleten.</span><span class="sxs-lookup"><span data-stu-id="d8337-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="d8337-108">Hvis du oppretter en gruppe sammenkoblede området og få en advarsel om det finnes allerede en annen gruppe med samme alias, må du kontrollere eksisterende grupper fra [Office 365 fra administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="d8337-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="d8337-109">Tilordnet til å løse problemet, sletter den eksisterende gruppen hvis det ikke lenger er nødvendig eller opprette området med et annet aliasnavn.</span><span class="sxs-lookup"><span data-stu-id="d8337-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="d8337-110">Det finnes ulike måter å opprette og bruke moderne grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8337-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="d8337-111">Du kan koble eksisterende områder til en gruppe for Office 365.</span><span class="sxs-lookup"><span data-stu-id="d8337-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="d8337-112">For mer informasjon, se [koble til en Office 365-gruppe ved hjelp av SharePoint bruker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="d8337-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="d8337-113">Hvis du vil opprette en Office 365-gruppen koblet område, må du opprette et gruppeområde.</span><span class="sxs-lookup"><span data-stu-id="d8337-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="d8337-114">For mer informasjon, kan du se [opprette et teamområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="d8337-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

