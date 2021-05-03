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
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125680"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="dce06-102">Distribuere tillegg for Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="dce06-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="dce06-103">Sentralisert distribusjon er den anbefalte måten å distribuere Office tillegg til brukere og grupper i organisasjonen på.</span><span class="sxs-lookup"><span data-stu-id="dce06-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="dce06-104">Følg fremgangsmåten nedenfor for å distribuere tillegg:</span><span class="sxs-lookup"><span data-stu-id="dce06-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="dce06-105">**Obs!** Hvis du vil installere tillegg for Office som en [enkeltbruker,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)kan du se Vise, administrere og installere tillegg i Office programmer .</span><span class="sxs-lookup"><span data-stu-id="dce06-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="dce06-106">Kontroller også at individuelle Office Store tillegg er aktivert.</span><span class="sxs-lookup"><span data-stu-id="dce06-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="dce06-107">Kontroller at miljøet oppfyller kravene for distribusjon av tillegg ved hjelp av sentralisert distribusjon.</span><span class="sxs-lookup"><span data-stu-id="dce06-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="dce06-108">Hvis du vil ha mer informasjon, kan du se [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="dce06-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="dce06-109">Gå til **Innstillinger**  >  **Integrerte apper** Hent apper i Microsoft 365  >   administrasjonssenteret for å distribuere tillegg.</span><span class="sxs-lookup"><span data-stu-id="dce06-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="dce06-110">Merknader:</span><span class="sxs-lookup"><span data-stu-id="dce06-110">Notes:</span></span> 

- <span data-ttu-id="dce06-111">Integrerte apper krever at administratoren har global administrator eller Exchange administratortillatelser.</span><span class="sxs-lookup"><span data-stu-id="dce06-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="dce06-112">Når du distribuerer tillegg til flere brukere, anbefaler vi å gjøre oppgaver ved hjelp av grupper i stedet for enkeltbrukere.</span><span class="sxs-lookup"><span data-stu-id="dce06-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="dce06-113">Hvis du vil ha mer informasjon, kan du se Vurderinger når du [tilordner](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)et tillegg til brukere og grupper .</span><span class="sxs-lookup"><span data-stu-id="dce06-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="dce06-114">Sentralisert distribusjon støtter ikke brukere i nestede grupper eller grupper som har overordnede grupper.</span><span class="sxs-lookup"><span data-stu-id="dce06-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="dce06-115">Hvis du vil ha mer informasjon, [kan du se Bruker- og gruppetilordninger](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="dce06-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="dce06-116">Kontroller at Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktivert for brukere å logge på.</span><span class="sxs-lookup"><span data-stu-id="dce06-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="dce06-117">Hvis du vil ha mer informasjon, [kan du se Konfigurere appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="dce06-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="dce06-118">Hvis du opplever problemer med distribusjon av tillegg ved hjelp av integrerte apper, kan du prøve å distribuere ved hjelp [av tillegg](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="dce06-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="dce06-119">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="dce06-119">For more information, see:</span></span>

<span data-ttu-id="dce06-120">[Distribuere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrere tillegg i administrasjonssenteret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Bruke PowerShell-cmdleter](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) for sentralisert distribusjon til å administrere tillegg 
 Publisere Office ved hjelp av sentralisert distribusjon via Microsoft 365 [administrasjonssenteret](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Feilsøke: Brukeren ser ikke tillegg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Feilsøke brukerfeil med Office tillegg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="dce06-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>