---
title: Slette eller gjenopprette programmer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014905"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="2e4b2-102">Slette eller gjenopprette programmer</span><span class="sxs-lookup"><span data-stu-id="2e4b2-102">Delete or restore applications</span></span>

<span data-ttu-id="2e4b2-103">**Slik sletter du et program fra Azure ad-leieren**:</span><span class="sxs-lookup"><span data-stu-id="2e4b2-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="2e4b2-104">Velg **virksomhets programmer** i **Azure ad-portalen**.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="2e4b2-105">Finn og Velg programmet du vil slette.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="2e4b2-106">Velg **Egenskaper** i delen **Behandle** i ruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="2e4b2-107">Velg **Slett**, og velg deretter **Ja** for å bekrefte at du vil slette appen fra Azure ad-leieren din.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="2e4b2-108">Hvis du vil ha mer informasjon om hvordan du sletter en app, kan du se [hurtigst Art: slette et program fra Azure Active Directory-leieren (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="2e4b2-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="2e4b2-109">I PowerShell fjerner [Fjern-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) -cmdleten program-proxy-konfigurasjoner fra et bestemt program i Azure Active Directory, og kan slette programmet fullstendig hvis det er angitt.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="2e4b2-110">Du kan **gjenopprette et slettet program** ved hjelp av PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2e4b2-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="2e4b2-111">Når programmet du vil gjenopprette, er identifisert, kan du gjenopprette det ved hjelp av [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="2e4b2-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
