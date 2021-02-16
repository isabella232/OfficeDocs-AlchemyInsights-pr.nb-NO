---
title: Gruppepolicy
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256782"
---
# <a name="group-policy"></a><span data-ttu-id="73c37-102">Gruppepolicy</span><span class="sxs-lookup"><span data-stu-id="73c37-102">Group policy</span></span>

<span data-ttu-id="73c37-103">Innstillinger for bruker- og datamaskinobjekter i Azure Active Directory Domain Services (Azure AD DS) behandles ofte ved hjelp av gruppepolicyobjekter (GPOs).</span><span class="sxs-lookup"><span data-stu-id="73c37-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="73c37-104">Azure AD DS inneholder innebygde GPOs for AADDC-brukere og AADDC-datamaskinbeholdere.</span><span class="sxs-lookup"><span data-stu-id="73c37-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="73c37-105">Du kan tilpasse disse innebygde gruppepolicyobjektene for å konfigurere gruppepolicy etter behov for miljøet.</span><span class="sxs-lookup"><span data-stu-id="73c37-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="73c37-106">Medlemmer av administratorgruppen for Azure AD DC har administrasjonsrettigheter for gruppepolicyer i Azure AD DS-domenet, og kan også opprette egendefinerte GPO-er og organisasjonsenheter (OUs).</span><span class="sxs-lookup"><span data-stu-id="73c37-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="73c37-107">Hvis du vil ha mer informasjon om hvilken gruppepolicy det er og hvordan den fungerer, kan du se [Oversikt over gruppepolicy.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="73c37-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="73c37-108">I et hybridmiljø synkroniseres ikke gruppepolicyer som er konfigurert i et lokalt AD DS-miljø, til Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="73c37-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="73c37-109">Hvis du vil definere konfigurasjonsinnstillinger for brukere eller datamaskiner i Azure AD DS, redigerer du et av standard gruppepolicyobjektene eller oppretter et egendefinert gruppepolicyobjekt.</span><span class="sxs-lookup"><span data-stu-id="73c37-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="73c37-110">Denne artikkelen [Administrere gruppepolicy viser](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) deg hvordan du installerer verktøyene for gruppepolicybehandling, hvordan du redigerer de innebygde gpoene, og hvordan du oppretter egendefinerte GPOs.</span><span class="sxs-lookup"><span data-stu-id="73c37-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



