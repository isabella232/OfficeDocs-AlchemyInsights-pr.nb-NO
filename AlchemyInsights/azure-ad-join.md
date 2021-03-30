---
title: Azure Active Directory-sammenføyning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405054"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="cd678-102">Azure Active Directory-sammenføyning</span><span class="sxs-lookup"><span data-stu-id="cd678-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="cd678-103">Hvis du konfigurerer enhetsregistreringer for første gang, må du kontrollere at du har gjennomgått Innføring i enhetsbehandling i [Azure Active Directory](/azure/active-directory/devices/overview) som veileder deg om hvordan du får enheter under kontrollen til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd678-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="cd678-104">Hvis du registrerer enheter i Azure AD direkte og registrerer dem i Intune, må du kontrollere at [](/mem/intune/fundamentals/licenses-assign) du har konfigurert [Intune](/mem/intune/enrollment/device-enrollment) og ha lisensiering på plass først.</span><span class="sxs-lookup"><span data-stu-id="cd678-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="cd678-105">Kontroller at du er autorisert til å utføre operasjoner i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd678-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="cd678-106">Bare en global administrator i Azure AD kan administrere innstillinger for enhetsregistreringer.</span><span class="sxs-lookup"><span data-stu-id="cd678-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="cd678-107">Hvis du vil gjøre implementering av Azure AD-sammenføyning, kan [du se Planlegge Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="cd678-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="cd678-108">Hvis du vil ha mer informasjon om hvordan du løser vanlige problemer med Azure AD-sammenføyning, kan du se Vanlige spørsmål om [Azure Ad Join](/azure/active-directory/devices/faq) og for Windows 10 pro-enheter i Kan ikke bli med i Windows [10 Pro-maskinen](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)til Azure AD – Må oppgradere til – Microsoft Community .</span><span class="sxs-lookup"><span data-stu-id="cd678-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
