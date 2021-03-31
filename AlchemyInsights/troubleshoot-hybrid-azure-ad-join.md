---
title: Feilsøk Hybrid Azure AD-sammenføyning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401916"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="11b55-102">Feilsøk Hybrid Azure AD-sammenføyning</span><span class="sxs-lookup"><span data-stu-id="11b55-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="11b55-103">Sterkt anbefalt: kontroller at en enhet får tilgang til endepunkter for enhetsregistrering under systemkontoen ved å bruke skriptet [Test tilkobling for enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="11b55-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="11b55-104">Dersom det er første gang du konfigurerer enhetsregistreringer, husk å se gjennom [Introduksjon til enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) for å lære hvordan du får enheter under kontroll av Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="11b55-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="11b55-105">Dersom du registrerer enheter i Azure Active Directory direkte og melder dem inn i Intune, påse at du har [konfigurert Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og har [lisensieringen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) på plass først.</span><span class="sxs-lookup"><span data-stu-id="11b55-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="11b55-106">Påse at du er autorisert til å utføre operasjoner i Azure Active Directory og lokalt Active Directory.</span><span class="sxs-lookup"><span data-stu-id="11b55-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="11b55-107">Bare en global administrator i Azure Active Directory kan behandle innstillinger for enhetsregistreringer.</span><span class="sxs-lookup"><span data-stu-id="11b55-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="11b55-108">I tillegg, dersom du konfigurerer automatiske registreringer in det lokale Active Directory, må du være administrator for Active Directory og AD FS (hvis gjeldende).</span><span class="sxs-lookup"><span data-stu-id="11b55-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="11b55-109">Hvis du vil ha flere detaljer om hvordan du løser potensielle problemer med hybrid-sammenføyning, kan du se [Feilsøk hybrid-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for konfigurering av hybrid Azure AD-sammenføyde og behandle enheter med Azure Active Directory-portal, se [Konfigurere hybrid Azure AD-sammenføyde (lokalt domene-sammenføyde) enheter](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) og [Behandle enheter med Azure-portalen](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="11b55-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="11b55-110">For å løse vanlige problemer med Hybrid Azure Active Directory (AD), se [Hybrid Azure AD-sammenføyning - vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="11b55-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
