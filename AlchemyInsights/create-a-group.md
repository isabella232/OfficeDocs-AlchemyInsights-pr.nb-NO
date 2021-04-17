---
title: Opprette en gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816365"
---
# <a name="create-a-group"></a><span data-ttu-id="2363a-102">Opprette en gruppe</span><span class="sxs-lookup"><span data-stu-id="2363a-102">Create a group</span></span>

<span data-ttu-id="2363a-103">Dette emnet beskriver oppretting av grupper.</span><span class="sxs-lookup"><span data-stu-id="2363a-103">This topic describes group creation.</span></span>

<span data-ttu-id="2363a-104">**Tillatelse til å opprette en gruppe**</span><span class="sxs-lookup"><span data-stu-id="2363a-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="2363a-105">Kontroller at du er autorisert til å opprette en ny gruppe.</span><span class="sxs-lookup"><span data-stu-id="2363a-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="2363a-106">Globale administratorer kan deaktivere oppretting av grupper i Azure-portalen eller Access Panel.</span><span class="sxs-lookup"><span data-stu-id="2363a-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="2363a-107">Du må kanskje ha en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.</span><span class="sxs-lookup"><span data-stu-id="2363a-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="2363a-108">**Behandle opprettelsestillatelser for grupper**</span><span class="sxs-lookup"><span data-stu-id="2363a-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="2363a-109">Globale administratorer kan administrere opprettelsestillatelser for grupper (av sikkerhetsrelaterte årsaker) eller Office 365-grupper som er opprettet i Azure-portalen eller accesspanelet, ved å velge «Brukere kan opprette sikkerhetsgrupper i Azure-portaler» eller «Brukere kan opprette Office 365-grupper i Azure Portals»-alternativer i Alle grupper Generelt  >  **(Innstillinger)**.</span><span class="sxs-lookup"><span data-stu-id="2363a-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="2363a-110">Du kan også begrense oppretting av grupper til å velge en gruppe brukere hvis du har en Azure Active Directory P1 Premium-lisens.</span><span class="sxs-lookup"><span data-stu-id="2363a-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="2363a-111">**Deaktivere velkomstvarsel for nye Medlemmer i Office 365-gruppen**</span><span class="sxs-lookup"><span data-stu-id="2363a-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="2363a-112">Velkomstvarselet som sendes til brukere som er lagt til i Office 365-grupper, kan deaktiveres ved å angi **UnifiedGroupWelcomeMessageEnabled** til False i Powershell.</span><span class="sxs-lookup"><span data-stu-id="2363a-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="2363a-113">Finn ut mer om denne innstillingen [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="2363a-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

