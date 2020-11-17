---
title: Opprette en gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088909"
---
# <a name="create-a-group"></a><span data-ttu-id="4fe92-102">Opprette en gruppe</span><span class="sxs-lookup"><span data-stu-id="4fe92-102">Create a group</span></span>

<span data-ttu-id="4fe92-103">Dette emnet beskriver opprettelse av grupper.</span><span class="sxs-lookup"><span data-stu-id="4fe92-103">This topic describes group creation.</span></span>

<span data-ttu-id="4fe92-104">**Tillatelse til å opprette en gruppe**</span><span class="sxs-lookup"><span data-stu-id="4fe92-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="4fe92-105">Kontroller at du har tillatelse til å opprette en ny gruppe.</span><span class="sxs-lookup"><span data-stu-id="4fe92-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="4fe92-106">Globale administratorer kan deaktivere opprettelse av grupper i Azure-portalen eller tilgangs panelet.</span><span class="sxs-lookup"><span data-stu-id="4fe92-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="4fe92-107">Du trenger kanskje en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.</span><span class="sxs-lookup"><span data-stu-id="4fe92-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="4fe92-108">**Behandle tillatelser for opprettelse av grupper**</span><span class="sxs-lookup"><span data-stu-id="4fe92-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="4fe92-109">Globale administratorer kan behandle tillatelser for opprettelse av grupper (for sikkerhetsrelaterte årsaker) eller Office 365-grupper som er opprettet i Azure-portalen eller tilgangs panelet, ved å velge alternativene brukere kan opprette sikkerhets grupper i Azure-portaler eller brukere kan opprette Office 365-grupper i Azure-portaler i **alle grupper**  >  **Generelt (innstillinger)**.</span><span class="sxs-lookup"><span data-stu-id="4fe92-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="4fe92-110">Du kan også begrense opprettelsen av grupper for å velge en gruppe med brukere hvis du har en Azure Active Directory P1 Premium-lisens.</span><span class="sxs-lookup"><span data-stu-id="4fe92-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="4fe92-111">**Deaktivere velkommen varsling for nye medlemmer i Office 365-gruppen**</span><span class="sxs-lookup"><span data-stu-id="4fe92-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="4fe92-112">Velkommens varselet som sendes til brukere som er lagt til i Office 365-grupper, kan deaktiveres ved å angi **UnifiedGroupWelcomeMessageEnabled** til Usann i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4fe92-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="4fe92-113">Lær mer om denne innstillingen [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4fe92-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

