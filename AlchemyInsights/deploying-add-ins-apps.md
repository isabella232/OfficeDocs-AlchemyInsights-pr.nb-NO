---
title: Distribuere tillegg for Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233543"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="a40f3-102">Distribuere tillegg for Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="a40f3-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="a40f3-103">Sentralisert distribusjon er den anbefalte måten å distribuere Office tillegg til brukere og grupper i organisasjonen på.</span><span class="sxs-lookup"><span data-stu-id="a40f3-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="a40f3-104">Følg fremgangsmåten nedenfor for å distribuere tillegg:</span><span class="sxs-lookup"><span data-stu-id="a40f3-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="a40f3-105">**Obs!** Hvis du vil installere tillegg for Office som en [enkeltbruker,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)kan du se Vise, administrere og installere tillegg i Office programmer .</span><span class="sxs-lookup"><span data-stu-id="a40f3-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="a40f3-106">Kontroller også at individuelle Office Store tillegg er aktivert.</span><span class="sxs-lookup"><span data-stu-id="a40f3-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="a40f3-107">Hvis du vil ha mer informasjon, kan du se Forhindre tilleggsnedlastinger ved å slå av Office Store på tvers av alle klienter [(unntatt Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="a40f3-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="a40f3-108">Kontroller at miljøet oppfyller kravene for distribusjon av tillegg ved hjelp av sentralisert distribusjon.</span><span class="sxs-lookup"><span data-stu-id="a40f3-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="a40f3-109">Hvis du vil ha mer informasjon, kan du se [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="a40f3-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="a40f3-110">Gå til **Innstillinger**  >  **Integrerte apper** Hent apper i Microsoft 365  >   administrasjonssenteret for å distribuere tillegg.</span><span class="sxs-lookup"><span data-stu-id="a40f3-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="a40f3-111">Merknader:</span><span class="sxs-lookup"><span data-stu-id="a40f3-111">Notes:</span></span> 

- <span data-ttu-id="a40f3-112">Integrerte apper krever at administratoren har global administrator eller Exchange administratortillatelser.</span><span class="sxs-lookup"><span data-stu-id="a40f3-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="a40f3-113">Når du distribuerer tillegg til flere brukere, anbefaler vi å gjøre oppgaver ved hjelp av grupper i stedet for enkeltbrukere.</span><span class="sxs-lookup"><span data-stu-id="a40f3-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="a40f3-114">Hvis du vil ha mer informasjon, kan du se Vurderinger når du [tilordner](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)et tillegg til brukere og grupper .</span><span class="sxs-lookup"><span data-stu-id="a40f3-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="a40f3-115">Sentralisert distribusjon støtter ikke brukere i nestede grupper eller grupper som har overordnede grupper.</span><span class="sxs-lookup"><span data-stu-id="a40f3-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="a40f3-116">Hvis du vil ha mer informasjon, [kan du se Bruker- og gruppetilordninger](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="a40f3-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="a40f3-117">Kontroller at Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktivert for brukere å logge på.</span><span class="sxs-lookup"><span data-stu-id="a40f3-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="a40f3-118">Hvis du vil ha mer informasjon, [kan du se Konfigurere appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="a40f3-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="a40f3-119">Hvis du opplever problemer med distribusjon av tillegg ved hjelp av integrerte apper, kan du prøve å distribuere ved hjelp [av tillegg](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="a40f3-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="a40f3-120">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="a40f3-120">For more information, see:</span></span>

<span data-ttu-id="a40f3-121">[Distribuere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Bruke PowerShell-cmdleter](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) for sentralisert distribusjon til å administrere tillegg 
 Publisere Office ved hjelp av sentralisert distribusjon via Microsoft 365 [administrasjonssenteret](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Feilsøke: Brukeren ser ikke tillegg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Feilsøke brukerfeil med Office tillegg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="a40f3-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>